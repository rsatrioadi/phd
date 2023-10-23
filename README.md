# Start Here

This repository decribes and links to the works related to my PhD project. The working title is “Automated Software Architecture Explanation.” For a little more information, I'd like to subtitle it “Generating and Presenting Software Architectural Knowledge from Implementation.” By the way, this is Satrio Adi Rukmono from the Eindhoven University of Technology (TU/e). My supervisors are [Michel Chaudron](https://research.tue.nl/en/persons/michel-rv-chaudron) and [Lina Ochoa](../../../../lmove).

## Background

This project was sparked from a “moonshot” challenge of automated answering of software developer's questions. It describes an intelligent agent that holds knowledge of a software system, sourced from various artefacts including requirements, design, code, tests, logs, and communications. This agent can then answer questions related to various roles in software development. For example, a software engineer may ask, “What caused this defect?” while a security engineer may ask, “Which security mechanisms are used?” We imagine the different difficulty levels of questions, with the “easiest” ones being: finding things in the system, and in increasing difficulty: explaining, diagnosing, and synthesizing solution to specific problems.

In the PhD project, the scope of knowledge is limited to architectural knowledge, extracted from implementation (i.e., source code) and maybe a little design document.

## Building Blocks

To approach the automated explanation, we envision three broad categories of tools: knowledge extractors, knowledge analyzers, and knowledge presenters. A common knowledge representation bridges the three categories. They work together in an (eco)system to serve the goal of generating and presenting knowledge. The flow of collaboration is illustrated in the figure below:

![Building blocks.](/figures/building-blocks.svg)

TODO: add a structure view for the building blocks.

1. Knowledge extractors

    The knowledge extractors take, as inputs, software development artefacts, which in the PhD scope is a software system implementation. They then perform analyses on the artefacts to produce a knowledge instance about the software system. The produced knowledge is ideally represented in the common representation. (This category may include existing software analysis tools; one can then build a conversion layer to format the analysis result in the common representation.)

2. Knowledge analyzers

    The knowledge analyzers perform analysis and knowledge enrichment on the existing knowledge instances. In other words, they act upon the knowledge extracted by the knowledge extractors and potentially other sources of knowledge to gain more knowledge and augment/update the existing knowledge instance.

3. Knowledge presenters

    The knowledge presenters are the user-facing parts of the whole (eco)system. The general idea is that they generate human-comprehensible presentation of the knowledge extracted and augmented by the other abovementioned tools. It can be as simple as generating a static view (e.g., a diagram/picture, a natural-language passage) of the knowledge, an interactive visualization, or a complex conversational user interface.

4. Knowledge representation

    To facilitate a common way knowledge is represented and used, we decided to use **labeled property graph** (LPG) as the preferred structure. As a short description: a labeled property graph is a graph in which its nodes and edges have _labels_ (somewhat like a “type” in programming terminology) and key-value pairs of _properties_. Since nodes and edges have types, we can then define what types of edges can exist between two nodes in a “graph schema”.

   TODO: connect with the notion of ontology

## Studies and Experiments

### Knowledge Representation

Our knowledge representation is outlined in [Enabling Analysis and Reasoning on Software Systems through Knowledge Graph Representation (MSR'23)](https://doi.org/10.1109/MSR59073.2023.00029). Below is an excerpt describing the requirements for the representation:

-    **R1: Abstract & Concrete.** We want our knowledge representation to support an abstract view that is free from implementation details so as to enable architecture-level analysis. This means the representation does not have to be back-convertible into source code. For example, our representation should not differentiate whether a data-structure is a struct, class, or record. At the same time, we want to be able to support relating high level views to concrete implementation level.

-    **R2: Rich in relational information.** Dependency graphs are commonly used in software analyses. These are often based on method/function calls. However, there are many other types of relationships between code fragments other than invocations. We want our knowledge representation to capture, for example, specialization and composition information.

-    **R3: Language-agnostic.** We want the knowledge representation not to be bound to a single programming language. We imagine the reasoning should be generic and apply to different implementation languages. However, for this work, we set our scope to include only class-based object-oriented software systems.

-    **R4: Handles partial and evolving knowledge.** From the models we find in practice, we know that knowledge about a system may be incomplete, yet still sufficient to enable basic types of analyses or reasoning. We want our representation to be able to capture such partial knowledge. This contrasts with classical modeling methods from the area of Formal Methods that require complete models of a system before any reasoning can be done.

-    **R5: Supports multiple knowledge sources.** Software knowledge may come from diverse sources such as source code, architecture documents, or UML models. We want to accumulate this different types of knowledge from different kinds of sources in a single representation.

-    **R6: Enrichable.** In addition to supporting different defined data sources, our knowledge representation should also be flexible enough for possible integration with emerging types of knowledge. For example, when classes are classified into role stereotypes [3], it should be possible to use this new information in an analysis pipeline.

Based on the requirements, we describe our LPG schemas for source code structure:

- LPG schema for detailed structure knowledge

    ![Expanded LPG schema.](/figures/expanded.svg)

    With the node labels defined as:

    * **_Structure_**: a class-type, including what languages may call structs, records, enumerations, etc. (The definitions of and _Structure_’s relations to _Type_ and _Primitive_ are therefore trivial for people familiar with object orientation.)
    * **_Container_**: anything in the language/platform that contains Structures or allows organization of Structures, e.g., package, directory, module, or namespace. _Structure_ extends _Container_ because some programming languages allow nested classes.    
    * **_Variable_** is self-explanatory; however, we point out that it includes what languages may call field, attribute, property, function/method parameter, etc.
    * **_Script_**: a code expression or a block of statements; lines of code that produce value or make effects.
    * **_Operation_**: a kind of _Script_ that is identified with a signature (name and parameters) and return type.    
    * **_Constructor_**: a kind of _Operation_ whose sole purpose is the creation of a _Structure_ instance. We consider a _Constructor_’s return type to be the _Structure_ that it creates, even though, e.g., Java considers constructors to have no return type.
    
    And the edge labels as follows:
    
    * **_specializes_** is for inheritance, including Java’s extends and implements keywords, mixins, etc.    
    * **_invokes_** denotes invocations. A _Script_ that does not have a signature (i.e., not an _Operation_) cannot be referred to, and therefore invoked by, another _Script_. An example is field initializers.
    * **_instantiates_** is a convenience edge that can be derived from other terms in the graph. _M instantiates S_ when _Structure S_ has a _Constructor C_ that is invoked by _Script M_.
    * The other edge types **_contains_**, **_type_**, **_returnType_**, **_hasVariable_**, **_hasScript_**, and **_hasParameter_** should be self-explanatory.

- LPG schema for abstract structure knowledge

    ![Compacted LPG schema.](/figures/compacted.svg)

    When a detailed LPG is available, an abstracted version can be derived by applying the following definitions of edges and then removing _Variable_ and _Script_ nodes (and consequently their connected edges):

    * _S **holds** T_ when _Structure S_ has a variable of _Type T_.
    * _S **accepts** T_ when _Structure S_ has an operation that has a parameter of _Type T_.
    * _S **returns** T_ when _Structure S_ has an operation with return _Type T_.
    * _S **constructs** T_ when _Structure S_ has a script that instantiates _Structure T_.
    * _S **calls** T_ when _Structure S_ has a script that calls an operation of _Structure T_. It is what is usually considered in a “dependency graph”.
    * _S **accesses** T_ when _Structure S_ has a script that directly access a field of _Structure T_.
 
    Finally, an example of an LPG that complies to the abstract schema:

    <!-- ![An instance of the strategy design pattern in JHotDraw.](/figures/strategy-jhotdraw.svg) -->
    <img src="/figures/strategy-jhotdraw.svg" width=600 alt="An instance of the strategy design pattern in JHotDraw." />

### Knowledge Extractors

#### Knowledge graph extractors

The above [MSR'23](https://doi.org/10.1109/MSR59073.2023.00029) paper also presents [javapers](../../../javapers). It takes a directory of Java source files (up to source level 16) and performs static analysis to extract knowledge graph instances that comply with our graph schemas. It supports extracting both the abstracted and detailed knowledge graph instances. It leverages the [Spoon](https://spoon.gforge.inria.fr/) library.

Javapers can provide the LPG in either XML, JSON, or CSV format. The JSON format complies with [Cytoscape](https://js.cytoscape.org/)'s format. It looks like this:

```
{ "elements": {
    "nodes": [
      { "data": {
          "id": <node_id>,
          "labels": [<node_label1>, ...],
          "properties": { <key1>: <value1>, ... } } },
      ... ],
    "edges": [
      { "data": {
          "id": <edge_id>,
          "source": <src_node_id>,
          "target": <tgt_node_id>,
          "label": <edge_label>,
          "properties": { <key1>: <value1>, ... } } },
      ... ] } }
```

The [neo4j-support](../../../javapers/tree/main/neo4j-support) folder in the javapers repository provides a way to import the LPG in JSON into a [Neo4j](https://neo4j.com/) graph database. You can then perform analyses with [Cypher queries](https://neo4j.com/docs/getting-started/cypher-intro/).

There are two other tools that can potentially be used for knowledge extractors in our ecosystem: [Rascal](https://www.rascal-mpl.org/) and [srcML](https://www.srcml.org/)+[srcType](../../../../srcML/srcType). In particular, [Matteo Asuni](../../../../matteasu) during his excursion at TU/e did the initial work for converting a Rascal [M3 model for C++](https://www.rascal-mpl.org/docs/Packages/Clair/API/lang/cpp/M3/) into our graph schema. Both Rascal and srcML enable higher-level extraction supporting diverse programming languages. We would like to utilize them to have LPG extractors for other programming languages.

### Knowledge Analyzers

#### Role stereotype classifiers

Our journal paper [Role stereotypes in software designs and their evolution (JSS vol.189)](https://doi.org/10.1016/j.jss.2022.111296) describes our effort to classify (Java) classes into role stereotypes. But first: **Role stereotypes** are abstract characterisations of the responsibilities of the building blocks of software applications. The role a class plays within a software system reflects its design intention. [Wirfs-Brock](https://www.wikidata.org/wiki/Q967529) introduced the following six role stereotypes: **_Information Holder_**, which knows information; **_Structurer_**, which maintains object relationships; **_Service Provider_**, which offers computing services; **_Coordinator_**, which delegates tasks to others; **_Controller_**, which directs other’s actions; and **_Interfacer_**, which transforms information. While these stereotypes were introduced in a “forward” way during design, we instead apply this notion retroactively—given the source code of a class, which role stereotype best describes it?

The original classifier was constructed by performing machine learning on static features of the class' source code. In his master's thesis, [Ka Yip Fung](../../../../Mboopi) improved the accuracy of the classifier by including dynamic features acquired by the means of run-time profiling. He extracted the features based on the call tree generated by [JProfiler](https://www.ej-technologies.com/products/jprofiler/overview.html).

We believe role stereotype information can be used to fine-tune smell detections. For example, the threshold of how many attributes a class should have must be different between an Information Holder and a Service Provider. This remains an open research question for now.

#### Software component summarization

In [Achieving High-Level Software Component Summarization via Hierarchical Chain-of-Thought Prompting and Static Code Analysis (ICoDSE'23)](icodse.org) (presented on September '23, proceedings pending) we presented an approach for automated software component summarization, combining static analysis with the emerging capabilities of a Large Language Model (LLM). In short, we use LLM to generate summaries of individual Java methods from their source code and then gather the summaries of all methods under a class to then generate a summary of that class. Analogously, we gather the summaries of all classes under a package to then generate a summary of that package.

A showcase for this technique is shown [here](/jhotdraw-summaries.md). Everything in that page is generated from pure source code, i.e., discarding any sorts of comments. An evaluation for this technique is currently being planned.

#### Deductive software architecture recovery

### Knowledge Presenters

#### Visualization efforts

One way that knowledge can be presented is trough (interactive) visualization. We have a visualization tool that takes as input the JSON-formatted LPG. It is developed using the Cytoscape javascript library. It is live and can be interacted with [here](https://rsatrioadi.github.io/classviz/?p=jhotdraw-trc-sum-rs).

Currently, we are actively developing visualization tools to help software developers understand the structure of a complex software system. We are focusing on having two levels of abstractions: a high level that should display something like 15 to 20 abstract “components” that we can use to zoom-in (and zoom back out) to a more detailed level.

#### What is a good software architecture explanation?

Ultimately, the goal of this PhD project is to provide a software architecture explanation based on the knowledge we can discover from the implementation of the software system. However, a big question remains before we can actually generate an explanation: **_What is a (good) software architecture explanation?_** To answer this, our initial approach involved conducting observation studies during software architecture explanation sessions. However, our efforts encountered challenges, as many companies declined participation due to confidentiality concerns. We managed to conduct a single observation session with an open-source project, which provided limited insights. To ensure a more robust study, we subsequently designed an interview-based approach.

Our interview study targets individuals involved in situations necessitating software architecture explanations, such as onboarding and offboarding. We employ convenience sampling to recruit participants, reaching out to industry contacts (mainly) for explainers and master students as well as recent graduates for explainees. Interviews are conducted in English, transcribed semi-automatically, and anonymized for privacy. Separate question sets were prepared for architecture explainers and explainees, focusing on the context and the explanation process itself.

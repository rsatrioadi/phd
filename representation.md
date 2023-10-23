#### A knowledge graph representation for software structure

[↑ back](/README.md)

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
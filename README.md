# Start Here

This repository decribes and links to the works related to my PhD project. The working title is “Automated Software Architecture Explanation.” For a little more information, I'd like to subtitle it “Generating and Presenting Software Architectural Knowledge from Implementation.” 

By the way, this is Satrio Adi Rukmono from the Eindhoven University of Technology (TU/e). My supervisors are [Michel Chaudron](https://research.tue.nl/en/persons/michel-rv-chaudron) and [Lina Ochoa](../../../../lmove).

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

## Studies, Experiments, Tools, etc.

### On Knowledge Representation

- [A knowledge graph representation for software structure](/representation.md)

### On Knowledge Extraction

- [Knowledge graph extractors](/extractors.md)

### On Knowledge Analysis

- [Role stereotype classifiers](/classifiers.md)
- [Software component summarization](/summarizer.md)
- [Deductive software architecture recovery](/deductive-sar.md)

### On Knowledge Presentation

- [Visualization efforts](/viz.md)
- [UML or Box-and-Line?](/uml-bnl.md)
- [What is a good software architecture explanation?](/expl-interviews.md)
  

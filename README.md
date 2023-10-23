# Start Here

This repository decribes and links to the works related to my PhD project. The working title is “Automated Software Architecture Explanation.” For a little more information, I'd like to subtitle it “Generating and Presenting Software Architectural Knowledge from Implementation.” By the way, this is Satrio Adi Rukmono from TU Eindhoven. My supervisors are Michel Chaudron and Lina Ochoa.

## Background

This project was sparked from a “moonshot” challenge of automated answering of software developer's questions. It describes an intelligent agent that holds knowledge of a software system, sourced from various artefacts including requirements, design, code, tests, logs, and communications. This agent can then answer questions related to various roles in software development. For example, a software engineer may ask, “What caused this defect?” while a security engineer may ask, “Which security mechanisms are used?” We imagine the different difficulty levels of questions, with the “easiest” ones being: finding things in the system, and in increasing difficulty: explaining, diagnosing, and synthesizing solution to specific problems.

In the PhD project, the scope of knowledge is limited to architectural knowledge, extracted from implementation (i.e., source code) and maybe a little design document.

## Building Blocks

To approach the automated explanation, we envision three broad categories of tools: knowledge extractors, knowledge analyzers, and knowledge presenters. A common knowledge representation bridges the three categories. This is all illustrated in the figure below:

![Building blocks.](/building-blocks.svg)

1. Knowledge extractors

    The knowledge extractors take, as inputs, software development artefacts, which in the scope of the PhD project is a software system implementation. They then perform analyses on the artefacts to produce a knowledge about the software system. The produced knowledge is ideally represented in the common representation. (This category may include existing software analysis tools; one can then build a conversion layer to format the analysis result in the common representation.)

2. Knowledge analyzers

3. Knowledge presenters

4. Knowledge representation

## Studies and Experiments

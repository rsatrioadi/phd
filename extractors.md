### Knowledge graph extractors

[↑ back](/README.md)

The previously mentioned [MSR'23](https://doi.org/10.1109/MSR59073.2023.00029) paper also presents [javapers](../../../javapers). It takes a directory of Java source files (up to source level 16) and performs static analysis to extract knowledge graph instances that comply with our graph schemas. It supports extracting both the abstracted and detailed knowledge graph instances. It leverages the [Spoon](https://spoon.gforge.inria.fr/) library.

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

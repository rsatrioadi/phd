### Visualization efforts

[↑ back](/README.md)

One way that knowledge can be presented is trough (interactive) visualization. We have a visualization tool that takes as input the JSON-formatted LPG. It is developed using the [Cytoscape](https://js.cytoscape.org) javascript library. It is live and can be interacted with [here](https://rsatrioadi.github.io/classviz/?p=jhotdraw-trc-sum-rs). This particular showcase presents the structure of a Java project [JHotDraw](../../../jhotdraw/tree/5.1-clean) and also includes the following analysis results:

1. Role stereotypes (as described [here](/classifiers.md)) in the form of node colors.
2. Trace information from dynamic analysis (also as described [here](/classifiers.md)) in the “Features” tab.
3. Automatically generated summaries (as described [here](/summarizer.md)) as shown in the “infobox” on the lower right corner of the screen when you hover over nodes.

We are actively developing visualization tools to help software developers understand the structure of a complex software system. We are focusing on having two levels of abstractions: a high level that should display something like 15 to 20 abstract “components” that we can use to zoom-in (and zoom back out) to a more detailed level.

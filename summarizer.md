### Software component summarization

In [Achieving High-Level Software Component Summarization via Hierarchical Chain-of-Thought Prompting and Static Code Analysis (ICoDSE'23)](/rukmono-icodse23.pdf) (presented on September '23, proceedings pending) we presented an approach for automated software component summarization, combining static analysis with the emerging capabilities of a Large Language Model (LLM). In short, we use LLM to generate summaries of individual Java methods from their source code and then gather the summaries of all methods under a class to then generate a summary of that class. Analogously, we gather the summaries of all classes under a package to then generate a summary of that package.

<!-- ![Summarization cycle.](/figures/sum_cycle.svg) -->
<img src="/figures/sum_cycle.svg" width=300 alt="Summarization cycle." />

(In the figure, _operation_ is synonymous with _method_, _module_ with _class_, and _component_ with _package_.)

A showcase for this technique is shown [here](/jhotdraw-summaries.md). Everything in that page is generated from pure source code, i.e., discarding any sorts of comments. An evaluation for this technique is currently being planned.

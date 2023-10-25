### Deductive software architecture recovery

[↑ back](/README.md)

We submitted a paper to ICSE-NIER'24 titled [Deductive Software Architecture Recovery via Chain-of-thought Prompting](/deductive-sar.pdf) (currently under review). Diverse techniques have been proposed for recovering software architecture from a system's  implementation. These existing approaches are *inductive* (bottom-up), i.e., the system's architecture is reconstructed only from facts specified at the source-code level. We envision a *deductive* (top-down) approach, which uses an architectural model as a high-level blueprint to classify source code units into architectural components. The approach is outlined below:

1. **Reference Architecture Definition**
   1. **Select the reference architecture.** It is intended to come from one of the system's architects or engineers. However, it may suffice to select one of the common reference architecture, e.g., the *layered architecture*.
   2. **Define the architectural components.** For example, in a layered architecture, the components may include *Presentation* Layer, *Application Services* Layer, *Domain Services* Layer, and *Technical Services* Layer.
   3. **Define component & interaction indicators.**  For example, classes from the Presentation Layer in an Android application may contain methods that *“set the attributes of UI components (e.g., the text of a TextView)”*, *“notify listeners about user events (e.g., button clicks or list item selections)”*, or *“perform validation on user input”*.
2. **Code Units Classification**
   1. **Evaluate code units against all indicators** of all architectural components. We leave the details of the indicator compliance analysis non-specific. However, the idea of deductive SAR is sparked and made effective by transformer-based language models, specifically via the chain-of-thought prompting technique. So one way to do it is simply by asking an LLM whether a code unit satisfies each indicator or not.
   2. **Aggregate the classification results.** Once we have the individual, low-level code units evaluated and classified, the next step is to aggregate the information to further classify the more abstract composition of code units. For example, if in the previous step, the classification is performed on methods, in this step, we aggregate that information to classify classes. This can then cascade into higher abstraction levels to construct a complete picture of the system's architecture.

As this is a New Idea submission, at this stage it notably lacks evaluation. We are still refining the technique and plan to design an evaluation in the coming months.

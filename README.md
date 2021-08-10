# Clean CaDET dataset

This repository contains the code smell dataset represented in the paper "Towards a systematic approach to manual annotation of code smells," submitted for consideration in _Expert Systems with Applications_ journal.

We annotated code snippets (methods or classes) for the presence and severity of two code smells: Long Method and God Class. We selected the annotated code snippets randomly from 8 open-source C# projects. A minimum of two annotators independently assigned the code smell severity. In cases of disagreement, the third annotator independently annotated the code snippet. Our dataset contains 3494 annotated instances (with a total of 8202 annotations). 

The datasheet of our dataset contains instances (code snippets) with the following information:
- Code Snippet ID – the full name of the code snippet. For classes, this is the package/namespace name followed by the class name. The full name of inner classes also contains the names of any outer classes (e.g., namespace.subnamespace.outerclass.innerclass). For functions, this is the full name of the class and the function’s signature (e.g., namespace.class.method(param1Type, param2Type)).
- Link – The GitHub link to the code snippet, including the commit and the start and end LOC.
- Code Smell – code smell for which the code snippet is examined.
- Project Link – the link to the version of the code repository that was annotated.
- Individual annotations – the severity score determined by each annotator.
- Final severity – a single severity score calculated using the algorithm described below.
- Metrics – a list of metrics for the code snippet, calculated by our platform https://github.com/Clean-CaDET/platform.

We create two sheets for each code smell. The first sheet contains the above-listed information, while the second sheet contains the heuristics given by each annotator. The second sheet is presented for completeness, and we believe that researchers will benefit primarily from the first sheet for each smell.

_Note: For now, we only provide a sample of the dataset. We will publish the full dataset upon completing our machine learning experiments._


# Table of Contents
0. [Abstract]
1. [Main FAIRification Objectives](#Main%20FAIRification%20Objectives)
2. [Graphical Overview of the FAIRification Recipe Objectives](#Graphical%20Overview%20of%20the%20FAIRification%20Recipe%20Objectives)
3. [FAIRification Objectives, Inputs and Outputs](#FAIRification%20Objectives,%20Inputs%20and%20Outputs)
4. [Capability & Maturity Table](#Capability%20&%20Maturity%20Table)
5. [Table of Data Standards](#Table%20of%20Data%20Standards)
6. [Executable Code in Notebook](#Executable%20Code%20in%20Notebook)
7. [How to create workflow figures](#How%20to%20create%20workflow%20figures)
8. [License](#License)

---

## Abstract

The FASTQ format is a popular format for storing sequences (i.e. letters representing nucleotides in a piece of DNA) and their corresponding quality scores. However, FASTQ files can exhibit a large variety of variants=dialects, or might get corrupted during file transfers. It is thus important to check the conformance of a given FASTQ file to a specific expectation of "how it should look like", e.g. to ensure compatibility with a given tool. This recipe will outline how a FASTQ file can be checked locally, i.e. without transferring it out of the borders of a certain local computer environment.

___


## Graphical Overview of the FAIRification Recipe Objectives

[![](https://mermaid.ink/img/eyJjb2RlIjoiZ3JhcGggVERcbkF7UmVxdWlyZW1lbnRzIGZ1bGZpbGxlZD99IC0tPnxZZXN8IEJbQXBwbHkgdGhpcyByZWNpcGVdXG5BIC0tPnxOb3wgRChTVE9QKVxuQiAtLT4gQyhGQVNUUSBmaWxlIHZhbGlkYXRpb24gb3V0cHV0KVxuIiwibWVybWFpZCI6eyJ0aGVtZSI6ImRlZmF1bHQifSwidXBkYXRlRWRpdG9yIjpmYWxzZX0)](https://mermaid-js.github.io/mermaid-live-editor/#/edit/eyJjb2RlIjoiZ3JhcGggVERcbkF7UmVxdWlyZW1lbnRzIGZ1bGZpbGxlZD99IC0tPnxZZXN8IEJbQXBwbHkgdGhpcyByZWNpcGVdXG5BIC0tPnxOb3wgRChTVE9QKVxuQiAtLT4gQyhGQVNUUSBmaWxlIHZhbGlkYXRpb24gb3V0cHV0KVxuIiwibWVybWFpZCI6eyJ0aGVtZSI6ImRlZmF1bHQifSwidXBkYXRlRWRpdG9yIjpmYWxzZX0)

<div class="mermaid">
graph TD
A{Requirements fulfilled?} -->|Yes| B[Apply this recipe]
A -->|No| D(STOP)
B --> C(FASTQ file validation output)
</div>

___

## Capability & Maturity Table

| Capability  | Initial Maturity Level | Final Maturity Level  |
| :------------- | :------------- | :------------- |
| Interoperability | minimal | repeatable |

----

## FAIRification Objectives, Inputs and Outputs

| Actions.Objectives.Tasks  | Input | Output  |
| :------------- | :------------- | :------------- |
| [Format Validation](http://edamontology.org/operation_0336)  | [FASTQ file](https://fairsharing.org/FAIRsharing.r2ts5t)  | [report](http://edamontology.org/data_2048)  |


## Table of Data Standards

| Data Formats  |
| :------------- |
| [FASTQ](https://fairsharing.org/FAIRsharing.r2ts5t)  |
___


## Executable Code in Notebook


```python
import isatools
import json
import pandas as pd
import holoview
```

___

## Authors:

| Name | Affiliation  | orcid | CrediT role  |
| :------------- | :------------- | :------------- |:------------- |
| Robert T. Giessmann |  Bayer AG | [0000-0002-0254-1500](https://http://orcid.org/0000-0002-0254-1500) | Writing - Original Draft |

___


## License:

<a href="https://creativecommons.org/licenses/by/4.0/"><img src="https://mirrors.creativecommons.org/presskit/buttons/80x15/png/by-sa.png" height="20"/></a>

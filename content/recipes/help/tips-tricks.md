(fcb-help-tips)=
# Tips and tricks 


## Main Objectives

The main purpose of this recipe is:

> to provide tips and tricks to styling Markdown Documents, styling Mermaid Flowcharts and creating Markdown tables.
> 


---
## 1. HackMD help and Documentation

If you are new the Markdown and HackMD, you may find the following to link quite valuable in getting you off the ground

1. [HackMD feature](https://hackmd.io/s/features)

Consider this a reference point as it really provides excellent basis for a successfull interaction with HackMD and Markdown.

2. [MarkDown syntax](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

There are many such references online. This one is actually pretty good.

3. [Emoji for Markdown cheatsheet](https://github.com/ikatyang/emoji-cheat-sheet)

For instance, if you'd like add a `warning` site, you can do th e following:

```:warning:```
which should be rendered as this sign:

:warning:

## 2. Styling Mermaid Flowchart:

you can check the [mermaid documentation](https://mermaid-js.github.io/mermaid/#/examples) 

We however provide some help with examples below

### Problem 1: My text is long and the box becomes huge

use an html `<br>` tag to add a new line in the box, like so:

```
subgraph one
  A(Building <br> Data <br> Catalogue):::box


  classDef box font-family:avenir,font-size:14px,fill:#2a9fc9,stroke:#222,color:#fff,stroke-width:1px
  end

```

### Problem 2: how to change font, box color?

Use styling for the element using the `classDef` following by a short-name for this style.
The mermaid element (boxes) can then be suffixed with that short-name using the triple colon `:::` as syntax marker.

```
subgraph one
  A(Building <br> Data <br> Catalogue):::box

  classDef box font-family:avenir,font-size:14px,fill:#2a9fc9,stroke:#222,color:#fff,stroke-width:1px
  end

```
### Problem 3: how to change the color of the connectors?

Use the `linkStyle` element.
:warning: make sure to provide the right number of connector as comma separated integers. If you get an error, it is often down to a discrepancy on this parameter.

The other argument are regular `CSS` like styling.

```
subgraph one
 A(Building <br> Data <br> Catalogue):::box
 A-->|define curation policies| B(Curation <br> Policies):::box

 linkStyle 0 stroke:#2a9fc9,stroke-width:1px,color:#2a9fc9,font-family:avenir;
```

## Problem 4: Struggling with Markdown Table


Formatting table can be a painful process. 

| Data Formats  | Terminologies | Models  |
| :------------- | :------------- | :------------- |
| [FASTQ](https://fairsharing.org/FAIRsharing.r2ts5t)  | [LOINC](https://fairsharing.org/FAIRsharing.2mk2zb)  | [SRA XML](https://fairsharing.org/FAIRsharing.q72e3w)  |
| [DICOM](https://fairsharing.org/FAIRsharing.b7z8by)  | [Human Phenotype Ontology](https://fairsharing.org/FAIRsharing.kbtt7f)  | [OMOP](https://fairsharing.org/FAIRsharing.qk984b)  |


To cut on the hardship, simply using the following online [Markdown table generator](https://www.tablesgenerator.com/markdown_tables)

![](/images/Pek2BoQ.png)

The component is intuitive to use and support copy and pate from say Excel for instance. Do the necessary tuning and then hit the `Generate` button to produce the Table in MarkDown format. 
Then, click on the green 'copy to clipboard button', go back to your markdown editor or HackMD and paste.

job done!

## Problem 5: How to resize images or figures:

When using HackMD, images can be inserting using the common toolbar and these are uploaded to imgur and the markdown looks like this:

```bash
![](/images/yI8TRNM.png)
```

but sizing is not properly supported which leads to rendering issues.

To solve the issue, the `best` course of action is to use an HTML `div` tag, which can be styled at will, as shown below:

```HTML
<div> <img 
src="/images/yI8TRNM.png" 
alt="drawing" 
style="width:750px;" 
border="1px solid black" 
align="top" />
</div>
```

Adjust the `width` element to resize the image to something satisfying. 


---

## How to create workflow figures

one may use the following **[mermaid](https://mermaid-js.github.io/mermaid/#/)** syntax:

```
graph LR;
    A[Data Acquisition] -->B(Raw Data)
    B --> C{FAIR by Design}
    C -->|Yes| D[Standard Compliant Data]
    C -->|No| E[Vendor locked Data]
```

---



## Authors:

| Name                                                                                                                                                                            | Orcid                                                                                                         | Affiliation              | Type                                                                              |                                                              Elixir Node                                                              | Credit Role
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|--------------------------|-----------------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------:|:----------------:|
| <div class="firstCol"><a target="_blank" href='https://github.com/proccaserra'><img class='avatar-style' src='https://avatars.githubusercontent.com/proccaserra'></img><div class="d-block">Philippe Rocca-Serra</div></a>  </div>         | <a target="_blank" href='https://orcid.org/0000-0001-9853-5668'><i class='fab fa-orcid fa-2x text--orange'></i></a> | University of Oxford     | <i class="fas fa-graduation-cap fa-1x text--orange" alt="Academic"></i> | <img class='elixir-style' src='/the-fair-cookbook/_static/images/logo/Elixir/ELIXIR-UK.svg' ></img> | Writing - Original Draft|
| <div class="firstCol"><a target="_blank" href='https://github.com/susannasansone'><img class='avatar-style' src='https://avatars.githubusercontent.com/susannasansone'></img><div class="d-block">Susanna-Assunta Sansone</div></a> </div> | <a target="_blank" href='https://orcid.org/0000-0001-5306-5690'><i class='fab fa-orcid fa-2x text--orange'></i></a> | University of Oxford     | <i class="fas fa-graduation-cap fa-1x text--orange" alt="Academic"></i> | <img class='elixir-style' src='/the-fair-cookbook/_static/images/logo/Elixir/ELIXIR-UK.svg' ></img> | Writing - Review & Editing, Funding acquisition

---



## License:

This page is released under the Creative Commons 4.0 BY license.

<a href="https://creativecommons.org/licenses/by/4.0/"><img src="https://mirrors.creativecommons.org/presskit/buttons/80x15/png/by.png" height="20"/></a>

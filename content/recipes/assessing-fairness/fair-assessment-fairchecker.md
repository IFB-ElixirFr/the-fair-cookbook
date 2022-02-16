(fcb-assess-fair-automatic-evaluator)=
# FAIR-Checker tool


````{panels_fairplus}
:identifier_text: ??
:identifier_link: ??
:difficulty_level: ??
:recipe_type: hands_on
:reading_time_minutes: ??
:intended_audience: principal_investigator, data_manager, data_scientist  
:has_executable_code: yeah
:recipe_name: FAIR-Checker tool
```` 

## Abstract

FAIR-Checker is a web tool to mine and analyze machine readable metadata found in web pages.

In this recipe, you will learn how to use FAIR-Checker to i) evaluate FAIR maturity indicators for your web resource, ii) inspect the metadata content of your resource. Finally, in iii) you will go through an executable Jupyter notebook intended to demonstrate how RDF metadata can be extracted and queried. This may allow you to extend computational assessments for your specific community needs. 


## Ingredients
	
| Ingredient | Type| Comment|
|:-----| :----|:-----|
|[HTTP1.1 protocol](https://tools.ietf.org/html/rfc2616)| data communication protocol | |
|[RDF/Linked Data](https://www.w3.org/standards/semanticweb/data)| model | |
|[identifiers.org](https://identifiers.org/)|identifier resolution service||
|[BioPortal](http://bioportal.bioontology.org/)|BioPortal registry||
|[Linked Open Vocabulary](http://)|||
|[Ontology Lookup Service](http://)|||
|[FAIR-Checker](https://fair-checker.france-bioinformatique.fr)|FAIR-Checker live instance || 
|[FAIREvaluator](https://W3id.org/AmIFAIR)|FAIR assessment||
|[FAIRShake](https://fairshake.cloud/)| FAIR assessment||



| Actions.Objectives.Tasks  | Input | Output  |
| :------------- | :------------- | :------------- |
| <!-- TODO add a link to corresponding document -->  | <!-- TODO add a link to corresponding document --> | <!-- TODO add a link to corresponding document --> |
| <!-- TODO add a link to corresponding document -->  | <!-- TODO add a link to corresponding document --> | <!-- TODO add a link to corresponding document --> |
| <!-- TODO add a link to corresponding document -->  | <!-- TODO add a link to corresponding document --> | <!-- TODO add a link to corresponding document --> |
| <!-- TODO add a link to corresponding document -->  | <!-- TODO add a link to corresponding document --> | <!-- TODO add a link to corresponding document --> |
| <!-- TODO add a link to corresponding document -->  | <!-- TODO add a link to corresponding document --> | <!-- TODO add a link to corresponding document --> |
| <!-- TODO add a link to corresponding document -->  | <!-- TODO add a link to corresponding document --> | <!-- TODO add a link to corresponding document --> |




## Objectives
FAIR-Checker leverages Semantic Web  technologies (RDF, SPARQL, SHACL) to mine and analyze machine readable metadata found in web pages.

This tool has two main facets:
- the **“Check”** module, targeting any user, allows them to execute a list of tests and get a synthetic estimation of the FAIRness of their resource, as well as technical recommendations to improve it.
- the **“Inspect”** module, targeting metadata experts, and allowing them to i) explore and verify if it conforms to community-defined standards (domain ontologies or Schema.org extensions such as Bioschemas) and ii)  identify missing or non-standard metadata to improve  resource FAIRness.


## Step by Step metadata checking

### The "Check" module

#### Providing a resource identifier and launching the FAIR assessment
- Provide the identifier of your web resource. Please note that FAIR-Checker only accepts URLs or DOI as identifiers. This ensures that the F1A principle is automatically verified (Your resource has a unique identifier). Note also that examples of web resources are provided below the text field.

- Launch evaluation by clicking on the "Test All Metrics" button. This will launch the execution of 13 individual tests described in the table below (Description button provides more information about eah test).




```{figure} ./assets/fair-checker-url.png
---
width: 800px
name: providing a URL for FAIR assessment
alt: providing a URL to for FAIR assessment
---
the [FAIR-Checker](https://https://fair-checker.france-bioinformatique.fr) home page
```

<!-- TODO --> 

#### Understanding the evaluation results 
- When the tests are completed 

## Step by Step metadata inspecting

### The "Inspect" module
<!--TODO--> 
#### Retrieving embedded metadata
<!--TODO--> 
#### Enriching metadata from public Knowledge Graphs
<!--TODO--> 
#### Assessing used ontologies
<!--TODO--> 
#### Evaluating candidate Bioschemas profiles
<!--TODO--> 

## Step by Step metadata inspecting in Python 
In this section we will provide code snippets to showcase how these assesment are computed. 

## Conclusion


## Reference

```{footbibliography}
```


## Authors

````{authors_fairchecker}
Thomas: Writing - Original Draft & Review & Editing
Marie-Dominique: Writing - Original Draft & Review & Editing
Alban: Writing - Original Draft & Review & Editing
````

---

## License

````{license_fairchecker}
CC-BY-4.0
````


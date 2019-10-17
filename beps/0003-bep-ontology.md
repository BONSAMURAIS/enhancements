# BEP-0003 BONSAI Ontology

| | |
| - | - |
| Number | 3 |
| Title | BONSAI Ontology |
| Status | Draft |
| Type | Guidelines |
| Proposed By | [Agneta Ghose](mailto:agneta@plan.aau.dk), [Bo Weidema](mailto:bo.weidema@bonsai.uno), [Elias Azzi](mailto:eazzi@kth.se), [Matteo Lissandrini](mailto:matteo@cs.aau.dk), [Massimo Pizzol](mailto:massimo@plan.aau.dk)
| Editor | [Massimo Pizzol](mailto:massimo@plan.aau.dk)|
| Created | 2019-03-12 |
| Last updated | 2019-03-24 |
| Version | 1 |

## Abstract

The issue under discussion is the schema to be used for the BONSAI ontology and specifically for the BONSAI hackathon. 


## Motivation

The ontology for BONSAI is currently incomplete and need to be improved to a minimum but operational level. 

## Proposal

After the discussion among members of the ontology and RDF working group an ontology [schema](https://docs.google.com/presentation/d/10Kd3zQEFPMEl7qB29xP65JGsNa9IKF8DvEg4SeiTKno/edit#slide=id.g5454c3adff_0_0) is proposed with an example. 

The ontology schema by [Janowicz et al.](http://geog.ucsb.edu/~jano/LCA_pattern.pdf) (_A minimal ontology pattern for life cycle assessment data_) and by [Yan et al.](https://geog.ucsb.edu/~jano/stscope_ontology.pdf) (_An Ontology For Specifying Spatiotemporal Scopes in Life Cycle Assessment_) have been a source of inspiration in drafting the BONSAI schema.

### Rationale

In drafting the ontology, these general principles were followed:

- Limit as much as possible the number of ontologies we refer to
- Keep track and limits as much as possible the introduction of new terms in the vocabulary
- Avoid making fixed choices, like sign nomenclatures, that are only useful in specific contexts.
- It is good practice for a model to stay as close to reality as possible
- Do not introduce unneccesary (obligatory) classifications

This lead to the decision to make the BONSAI ontology general enough to be operational and usable in different domains of industrial ecology, without adhering excessively to a specific framework (e.g. the LCA framework). 


In terms of issues specific to RDF format, it was agreed to:
 
- Use purl.org as namespacing for the part of the ontology that is BONSAI-specific, considered good in the long-term, when bonsai becomes public
- Use OM ontology instead of QUDT
- Use xsd:dateTime adding hh:mm to the date.
- Use the provo Ontology
- Use geonames
- Consider the ontology for time: https://www.w3.org/TR/owl-time/
- Consider https://www.w3.org/TR/2017/NOTE-eo-qb-20170928/ for raster data

### Alternatives

Ideas that were not ultimately selected 

- Using “input” and “output” subclasses has been discussed. Common agreement was that using such subclasses is redundant when there is already a predicate like _b:isInputOf_. The subclasses allow making elegant queries, semantically speaking. But the same result can be obtained without them using the predicates. This was considered closer to a human way of thinking. The subclasses were abandoned in favour of keeping a parsimonious model with predicates only.

-  The sign and necessity of a reference flow was discussed. Unclear aspects: if it should be a class, subclass, or property; if it should always be output or could be input; if it can be determined automatically; if it is necessary to obtain square matrices. It was clarified that mathematically it can be both positive and negative, but the convention choice has implications (e.g. the LCA community might have a different preference than the IO community). In some cases can be determined automatically. It was nevertheless decided to maintain it in order to avoid information loss when importing from / exporting to LCA/IO format and in order to facilitate the understanding of causality between activities.

- It was discusses whether environmental exchanges and waste flows should be included in the schema, for example by creating a specific class. It was argued that wastes, by-products and emissions do not need to be distinguished. These can be identified with automatic procedures from the information already in the ontology or using external data (for example, a separate list of biosphere flows). Therefore, their specification was deemed  not strictly necessary and left out of the ontology.

- For RDF format, replacing _schema:Place_ with geonames. [The way Place is defined](https://schema.org/Place) was considered strange and not helpful for our use case

### Open Issues

The _"property"_ between different flows e.g. the fact that a specific value of emission is calculated for a specific period of time like one year is an important element that is currently missing in the ontology (at the time of writing). It is important because:

- is often implicit or assumed information;
- is essential to allow the combination and integration of data from different sources (e.g. all exiobase data refer to a one-year period but ecoinvent data refer to different period depending on the dataset).

### Non-Goals

NN

### Test plan

The usefulness of the ontology will b e tested in practice at the hackathon. 

## Discussion

Links to places  where the BEP has been discussed by the community:

- [Minutes of the group meetings](https://github.com/BONSAMURAIS/BONSAI-ontology-RDF-framework)
- [Email correspondence of the ontology group](https://bonsai.groups.io/g/hackathon2019/topic/start_of_the_ontology/30225132?p=,,,20,0,0,0::recentpostdate%2Fsticky,,,20,2,0,30225132)
- [Nomenclature for "flow objects"](https://bonsai.groups.io/g/main/topic/ontology_can_we_come_up_with/30878645?p=,,,20,0,0,0::recentpostdate%2Fsticky,,,20,2,0,30878645)

## Previous Versions

NN

## Copyright

To the extent possible under law, **Massimo Pizzol** has waived all copyright and related or neighboring rights to Bonsai Enhancement Proposal **3 BONSAI (BEP) Ontology**. This work is published from: **Denmark**.

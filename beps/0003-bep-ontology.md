# BEP-0003 BONSAI (BEP) Ontology

| | |
| - | - |
| Number | 1 |
| Title | BONSAI (BEP) Ontology |
| Status | Proposed |
| Type | Guidelines |
| Proposed By | [Massimo Pizzol](massimo@plan.aau.dk)|
| Editor | |
| Created | 2019-03-12 |
| Last updated | 2019-03-12 |
| Version | 1 |

## Abstract

The issue under discussion is the schema to be used for the BONSAI ontology and specifically for the BONSAI hackathon. 


## Motivation

The ontology for BONSAI is currently incomplete and need to be improved to a minimum but operational level. 

## Proposal

After the discussion among members of the #ontology working group a schema (**link to final schema to be added**) is proposed with an example. The schema is based on the works of [Janowicz et al.](http://geog.ucsb.edu/~jano/LCA_pattern.pdf) (_A minimal ontology pattern for life cycle assessment data_) and [Yan et al.](https://geog.ucsb.edu/~jano/stscope_ontology.pdf) (_An Ontology For Specifying Spatiotemporal Scopes in Life Cycle Assessment_)

### Rationale

It was decided to:

- Use OM ontology instead of QUDT
- Use xsd:dateTime requires to add hh:mm to the date.
- Keep track and limits as much as possible the introduction of new terms in the vocabulary
- Limit as much as possible the number of ontologies we refer to
- Use the provo Ontology
- Use geonames
- Consider the ontology for time: https://www.w3.org/TR/owl-time/
- Consider https://www.w3.org/TR/2017/NOTE-eo-qb-20170928/ for raster data

Mandatory. Describe why particular design decisions were made.

### Pros and Cons

Optional. May be free-form text or bullet lists

### Alternatives

Mandatory. Ideas that were not ultimately selected

- replacing schema:Place with geonames. The way Place is defined (https://schema.org/Place) is weird and not helpful for our use case
- Not using the “input” and “output” subclasses has been discussed. Seemed redundant when there is already a property _b:isInputOf_. But using them is useful for filtering activities later on. 
-  The sign and necessity of a reference flow.
Not clear if it should be a class, subclass, or property. Pro/contra missing.
Not clear if it should always be output or could be input. It was clarified that mathematically it can be both but the convention choice has implications (e.g. Input-output experts like it output and positive). 

Problem: According to Matteo having ref flow both input and output is problematic in the schema. Reason still not clear though.

Leaving the reference flow out implies information loss when importing from / exporting to LCA/IO format and without it we can’t determine causality, but it makes the ontology less complex.

- Environmental exchanges and waste flows initially missing in the draft schema, how to include them:
It was suggested to either 1) create a class “Substance” (or other meaningful name) similar to class “Product” or  2) remove class “Product” and just keep class “Flow” that would be valid for both environmental and product exchanges. It was argued that _“Wastes, by-products and emissions do not need to be distinguished.”_ and therefore point 1 was abandoned.


### Open Issues

Optional. Relevant issues or questions not governed or resolved by this BEP

### Non-Goals

Optional. Listing non-goals helps to focus discussion and make progress

### Test plan

Mandatory. How can one show the usefulness of the proposal in practice?

## Discussion

A comprehensive bullet list of link to where the BEP has been discussed by the community, such as the BONSAI mailing list, and Github pull requests and issues.

## Previous Versions

(Bullet list of all previous versions with links)

## Copyright


To the extent possible under law, **Massimo Pizzol** has waived all copyright and related or neighboring rights to Bonsai Enhancement Proposal **3 BONSAI (BEP) Ontology**. This work is published from: **Denmark**.

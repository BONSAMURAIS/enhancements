# BEP-0003 BONSAI (BEP) Ontology

| | |
| - | - |
| Number | 1 |
| Title | BONSAI (BEP) Ontology |
| Status | Proposed |
| Type | Guidelines |
| Proposed By | [Massimo Pizzol](massimo@plan.aau.dk), [Romain Sacchi](r_s@me.com) |
| Editor | |
| Created | 2019-03-12 |
| Last updated | 2019-03-12 |
| Version | 1 |

## Abstract

The issue under discussion is the schema to be used for the BONSAI ontology and specifically for the BONSAI hackathon. 


## Motivation

The ontology for BONSAI is currently incomplete and need to be improved to a minimum but operational level. 

## Proposal

Initial discussion among  #ontology sub-group member, and working group schema proposed with an example 
Draft incomplete and all choices up to discussion.


### Rationale

- Based on the works of Janowicz et al. (_A minimal ontology pattern for life cycle assessment data_) and Yan et al. (_An Ontology For Specifying Spatiotemporal Scopes in Life Cycle Assessment_)






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

## BEP metadata

The BEP header table should contain the following:

* Number: Integer number, also used in the filename. Self-assigned ascending integers starting from 1.
* Title: This is the title of the KEP. Keep it simple and descriptive.
* Status: One of:
    * draft: Incomplete proposal being worked on by the authors and editor
    * proposed: Complete proposal open for discussion by the community, or being voted on
    * deferred: Complete proposal not currently under public discussion
    * accepted
    * rejected
    * withdrawn
    * superseded
* Type: One of:
    * Software features: Describes a new feature or implementation for BONSAI.
    * Guidelines: Provides general guidelines or information to the BONSAI community, but does not propose a new feature.
* Proposed by: Name and email of proposer
* Editor: Name and email of editor
* Created: Date in YYYY-MM-DD format
* Last updated: Date in YYYY-MM-DD format
* Version: Ascending integer number starting from 1
* Replaces: **Optional** row if this BEP replaces an existing proposal
* Superseded by: **Optional** row if this BEP has itself been replaced

Note that the BEP process is governed by [BEP 3: BONSAI project community governance structure].

## Discussion

A comprehensive bullet list of link to where the BEP has been discussed by the community, such as the BONSAI mailing list, and Github pull requests and issues.

## Previous Versions

(Bullet list of all previous versions with links)

## Copyright


To the extent possible under law, **Massimo Pizzol** has waived all copyright and related or neighboring rights to Bonsai Enhancement Proposal **3 BONSAI (BEP) Ontology**. This work is published from: **Denmark**.

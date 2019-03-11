# BEP-0003 BONSAI project community governance structure

| | |
| - | - |
| Number | 3 |
| Title | BONSAI project community governance structure |
| Status | Draft |
| Proposed By | [Chris Mutel](chris.mutel@bonsai.uno ) |
| Editor | |
| Created | 2019-03-09 |
| Last updated | 2019-03-09 |
| Version | 1 |

## Abstract

The BONSAI project brings together a large number of people from different communities, backgrounds, perspectives, and motivations. We want to be a resource for the community, and a reflection of the community. As such, the decision making process needs to be open, accessible, and transparent.

This BEP proposes that decisions be made by a consensus model. Specifically, each major decision should be documented in a BONSAI enhancement proposal (BEP) document, and be accepted by two-thirds of the BONSAI community.

## Motivation

Other industrial ecology databases serve as community resources, but are controlled by a few people or institutions. In general, their decision-making processes exclude outside opinions or options, are poorly communicated, and not clearly documented. As a result, we observe the following:

* It is difficult or impossible to combine datasets from multiple databases
* It is impossible to understand the detailed chain of calculations from raw data to numbers present in the database
* The vast majority of data published in reports or scientific articles do not end up in databases

In short, no database belongs to the community, and therefore the community has no agency or responsibility for the current state of affairs. The only way out of this vicious cycle is to build a community database controlled by the community from the ground up. A formal, documented, and consensus-based decision-making process is one way to realize community control.

## Proposal

### The BONSAI project

The BONSAI project is governed by the people contributing to the broader BONSAI proposal, and is not under the control of the legal entity BONSAI non-profit organization (hereafter BNPO), founded in Denmark, and owner of the website https://bonsai.uno. The BNPO supports BONSAI, and as a legal entity can receive donations and grants; the BONSAI project is a collection of people, data, software, and computer systems which fulfill the vision of an innovative and open industrial ecology footprinting database. Similarly, the BONSAI project has no formal role in the BNPO, except as explicitly stated by the statues of the BNPO.

Membership in the BONSAI project is indicated by subscription to the [BONSAI mailing list](https://bonsai.groups.io/g/main/topics), and is open to everyone.

### BONSAI enhancement proposals (BEPs)

In cases where multiple opinions or options are possible, decisions should be made by BONSAI project members via a BONSAI enhancement proposal (BEP). This document does not explicitly give guidelines on what does or does not require a BEP, but assumes that the participants act in good faith and with community spirit. It is expected that BEPs will be required for the following:

* System modeling choices
* Inclusion of large new databases
* Methodological questions, especially regarding allocation, space, and time
* Ontology and vocabulary choices
* Data formats and licensing

One or more authors may create a BEP by forking the [Github repo](https://github.com/BONSAMURAIS/enhancements) and adapting a copy of the [BEP template](https://github.com/BONSAMURAIS/enhancements/blob/master/beps/0001-bep-template.md). Once a BEP is considered complete by the authors, it enters the public discussion phase. The authors must find an editor with whom they do not have a close personal relationship. The editor is not an advocate for the BEP, but is responsible for administering the BEP until a vote is finished. The editor role is heavily based on [editors in the PEP process](https://www.python.org/dev/peps/pep-0001/#pep-editor-responsibilities-workflow). After an editor is assigned, authors should not directly modify the BEP document themselves. However, authors may withdraw the BEP at any time.

When an editor accepts their role, they should:

* Add their name to the metadata.
* Check that the BEP is ready. The format should be followed, the language should be clear, the ideas should be completely developed. The editor does not need to agree with the proposal.
* Merge the BEP pull request to the [Github repo](https://github.com/BONSAMURAIS/enhancements).
* If the BEP is not ready, provide specific feedback to the authors in an issue, and request a pull request.
* When the BEP is ready, change the status to `proposed`, send an email to the BONSAI mailing list with the hashtag BEPXXXX (replacing XXXX with the correct number), and then add a link the resulting mailing list discussion to the `Discussion` section of the BEP.

Editor roles can be transferred.

### BEP voting

When the editor has decided that productive discussion and debate on the BEP has finished, they may call for a vote via a poll on the BONSAI mailing list. The poll should have two options: yes and no. For a BEP to be accepted, two-thirds (rounding down) of the participants must vote yes. In addition, at least half of the BONSAI project members active (defined as posting to the mailing list or committing code to a repository in the BONSAMURAIS organization) within the last six months (i.e. a quorum) must vote. The voting period will last for two weeks, but can be extended to four weeks by the editor at their discretion.

BEPs which fail to achieve a quorum is given the status `deferred`. A BEP which fails to get a two-thirds vote is given the status `rejected`.

### BEP retirement or replacement

A BEP can include language replacing an existing BEP, in which case the editor of the new BEP should change the status of the older BEP to `superseded`.

A BEP may be retired following the initiation of a vote by the current editor and the same voting rules in the initial BEP voting procedure.

### Rationale

Enhancement proposals as formal specifications for new software were pioneered by the Python software foundation with [Python Enhancement Proposals (PEPs)](https://www.python.org/dev/peps/), and are now [widely used](http://lmgtfy.com/?q=enhancement+proposals). The BONSAI enhancement proposal (BEP) template, proposed in [BEP 1](https://github.com/BONSAMURAIS/enhancements/blob/master/beps/0001-bep-template.md), builds on the [PEP template](https://www.python.org/dev/peps/pep-0012/) and [another enhancement proposal template](https://www.nengo.ai/enhancement-proposals/001-template.html). It not only requires a detailed description of the problem to be addressed and the proposed solution, but also the alternatives considered, issues not solved by the proposal, and other pros and cons of the proposal.

### Pros and Cons

* Consensus-based model let's everyone have an equal vote
* Consensus-based model should reflect the opinions of the broader community
* Consensus-based model can stifle radical ideas and is slower than more exclusive leadership
* BEPs make people think about alternatives and how their theoretical ideas can be tested
* BEPs and archived votes allow a complete record of community decision making
* BEPs could be excessively bureaucratic for smaller decisions

### Alternatives

The Python foundation did not choose a consensus-based approach, but went with a board of core contributors. A small group of experts could make quicker and perhaps better technical decisions, though there is no clear evidence for this last assertion.

Another alternative would be to leave decisions to the BNPO Board, though this would probably not lead to a community spirit or investment in BONSAI.

### Open Issues

* Some discussion items or software ideas may not be effectively communicated via BEPs.
* A completely open system may be subject to abuse by internet trolls or others not in accordance with the BONSAI vision.
* A small group of people will still need control of the Github website and other communication media. The process for selecting these people is not specified.
* It may be impossible to get a definitive answer to a controversial subject using a consensus-based approach.
* Some terms are not precisely defined, e.g. active members.

### Non-Goals

This document is not intended to be final or complete; it is anticipated that substantial changes may be necessary in the future.

### Test plan

The BEP structure and process will be tested before and during the 2019 hackathon.

## Discussion

None yet.

## Previous Versions

None yet.

## Copyright

To the extent possible under law, Chris Mutel has waived all copyright and related or neighboring rights to Bonsai Enhancement Proposal 3: BONSAI project community governance structure. This work is published from: Switzerland.

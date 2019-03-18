# BEP-0004 BONSAI communication strategy

| | |
| - | - |
| Number | 4 |
| Title | BONSAI knowledge management and communication strategy |
| Status | Draft |
| Type | Guidelines |
| Proposed By | [Tom Millross](https://github.com/tmillross/) |
| Editor |  |
| Created | 2019-03-12 |
| Last updated | 2019-03-18 |
| Version | 2 |

## Abstract

The goal of this effort is to organise the Bonsai mediums such that interested people can quickly navigate to the most up-to-date information which is relevant for them. This way they are more likely to properly understand the project without unnecessary struggle. Once they have this understanding, their path toward meaningful contributions will be clearly guided from the [getting-started page](https://github.com/BONSAMURAIS/bonsai/wiki/Getting-started).

## Motivation

There are currently too many communication channels separate places for digitally documenting/storing our combined knowledge. It is  hard for newcomers to get started, and for active participants to know where each type of information should reside.

As of the writing of this proposal, there are the following:

* The bonsai.uno website
* The 'main' mailing list on groups.io and the hackathon sub-group
* BONSAMURAIS organization on Github, plus repositories
* A slack workspace
* A google docs folder _(recently deprecated)_
* A LinkedIn company and closed group _(recently deprecated)_

## Proposal

This BEP proposes guidelines for knowledge management and communication. A specific use-case for each of three mediums is described: the Web-page, mailing list, and GitHub (with sub-sections). 

The scope of this proposal is limited to written, publicly accessible knowledge and communication mediums. Private communications including video/phone calls, personal emails, and messenging applications are beyond scope. Source code management, documentation and version control are also not covered.

All action points already discussed publicly and committed-to-acting-upon by Michele De Rosa ([here])https://bonsai.groups.io/g/main/message/13_) are excluded. Discussions regarding LinkedIn (at a board meeting) and Google Docs ([here](https://bonsai.groups.io/g/main/topic/30174153?p=,,,20,0,0,0::recentpostdate,,,20,2,0,0&allview=1)) have already been completed (with the decision to deprecate their usage), and are hence also omitted from this proposal.

### The website bonsai.uno

The web page currently has the following pages:

* Landing page, https://bonsai.uno/: Brief introduction, buttons for downloading short presentation and contributing, links to subpages
* Challenge and vision, https://bonsai.uno/challenge-vision/: A global challenge, a global vision
* Organization, https://bonsai.uno/organisation/: Description as NPO, links to statutes, minutes, board
* Strategy work plan, https://bonsai.uno/strategy-work-plan/: Graphic of data flow, links to many working groups
* 10 specific working group detail pages under https://bonsai.uno/strategy-work-plan/
* Contribute, https://bonsai.uno/contribute/: Form to give donations or become a member
* Subpages for contributing: https://bonsai.uno/contribute/payment/, https://bonsai.uno/contribute/donation/

Proposed action (in addition to [these](https://bonsai.groups.io/g/main/message/13_)): 
The BONSAI web page source code should be made public as a Github repo under the BONSAMURAIS organization, enabling updates via pull requests.

### GitHub
GitHub offers a variety of integrated functionality which we propose to use in a conventional way. This section first describes the top-level information architecture concepts: 'organisations' & 'repositories'. Then the suggested use of specific tools and functionality within these: 'community health files', 'wikis', 'issues', 'projects' and 'project boards'.

#### Organisation (Bonsamurais)
There is only one existing Bonsai organisation on GitHub. No others should be made.

#### Repositories
_Guidance on when to create/merge/delete repositories is beyond the scope of this BEP_.

#### Community health files (including readmes)
https://help.github.com/en/articles/creating-a-default-community-health-file-for-your-organization

As the first thing people see when navigating the GitHub website; each repository should have a clear Readme.Md which describes the repo's purpose. Further examples and recommendations can be researched [here](https://github.com/matiassingers/awesome-readme)

#### Wikis (only 1: within the 'Bonsai' repository)
Only the repository _[bonsai](https://github.com/BONSAMURAIS/bonsai)_ should have the Wiki functionality enabled. 
All other repositories should link to content in this wiki, where appropriate.
The Wiki should not be used for task management, as the interface does not effectively support this use-case.


More information about GitHub wikis is available [here](https://help.github.com/en/articles/about-wikis).

_Potential overlap between the Wiki and pending Software Documentation is beyond the scope of this BEP_.

#### Issues
#### Projects
#### Project boards
#### Suggested 'notification' settings

The wiki becomes the primary destination for up-to-date information, with only stable information on the website (plus eventually the web-apps).

Use the Github 'Projects' functionality for task management.

* When tasks relate to specific repos, use the 'projects' in those.
* For higher-level tasks or ones that presently lack repositories, use the top-level Bonsai organisation 'projects'

Update the wiki front-page (or make a dedicated page) with the outcome of this discussion.

a.       use this as the general "contributing guidelines" (or similar) for the organisation. Stating how we agree to use the various comms mediums and tools such as GitHub Issues etc.
b.       This becomes the basis for the #GettingStarted guide referenced by Chris

Add any missing information from the website-hosted strategy and work plan to the wiki. Then delete these webpages.

Move the 5 pages of tasks to appropriate GitHub organisation or repository Project Boards

### The Mailing List


**** 

### Rationale

Mandatory. Describe why particular design decisions were made.

### Pros and Cons

_Not included_

### Alternatives

Mandatory. Ideas that were not ultimately selected

### Open Issues

1.  When to create/merge/delete GitHub repositories
2.  Potential overlap between the Wiki, and other documentation describing the software functionality, APIs, and/or implementation details.

### Test plan

Mandatory. How can one show the usefulness of the proposal in practice?

## Discussion

A comprehensive bullet list of link to where the BEP has been discussed by the community, such as the BONSAI mailing list, and Github pull requests and issues. For example, this template is discussed in:


## Previous Versions

None.

## Copyright

All BEPs must be licensed with [CC0](https://creativecommons.org/publicdomain/zero/1.0/):

  To the extent possible under law, Tom Millross has waived all copyright and related or neighboring
  rights to Bonsai Enhancement Proposal 0004. This work is published from: The Netherlands.

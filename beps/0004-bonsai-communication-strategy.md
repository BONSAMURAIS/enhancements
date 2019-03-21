# BEP-0004 BONSAI knowledge management and communication strategy

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

The goal of this effort is to organise the Bonsai mediums such that interested people can quickly navigate to the most up-to-date information which is relevant for them. This way they are more likely to properly understand the project without unnecessary struggle. Once they have this understanding, their path toward meaningful contributions will be clearly guided from a [getting-started guide](https://github.com/BONSAMURAIS/bonsai/wiki/Getting-started).

## Motivation

There are currently too many communication channels separate places for digitally documenting/storing our combined knowledge. It is  hard for newcomers to get started, and for active participants to know where each type of information should reside. The growth of new mediums should be halted, with any new alternatives discussed before they are created.

As of the writing of this proposal, there are the following:

* The bonsai.uno website
* The 'main' mailing list on groups.io and the hackathon sub-group
* BONSAMURAIS organization on Github, plus repositories
* A Slack workspace
* A Google Docs folder _(recently deprecated)_
* A LinkedIn company and closed group _(recently deprecated)_

Further mediums have also been suggested, such as:
* a Discourse forum
* an Open Science Framework (OSF) project
* a StackOverflow tag
* ...

## Proposal

This BEP proposes guidelines for knowledge management and communication. A specific use-case for each of three mediums is described: the Web-page, mailing list, and GitHub (with sub-sections). It is proposed that no other new mediums should be created without advanced discussion.

The scope of this proposal is limited to written, publicly accessible knowledge and communication mediums. Private communications including video/phone calls, personal emails, and messenging applications are beyond scope. Source code management, documentation and version control are also not covered.

All action points already discussed publicly and committed-to-acting-upon by Michele De Rosa [here](https://bonsai.groups.io/g/main/message/13_) are excluded. Discussions regarding LinkedIn (at a board meeting) and Google Docs ([here](https://bonsai.groups.io/g/main/topic/30174153?p=,,,20,0,0,0::recentpostdate,,,20,2,0,0&allview=1)) have already been completed (with the decision to deprecate their usage), and are hence also omitted from this proposal.

### The website bonsai.uno
The website should be used for information which does not require ongoing contribution and is mostly static. In the future it will be used by default for hosting web applications which are developed (unless an alternative solution is preferred, with rationale openly discussed).

Proposed action (in addition to [these](https://bonsai.groups.io/g/main/message/13_)): 
1.  The BONSAI web page source code to be made public as a Github repo under the BONSAMURAIS organization, enabling updates via pull requests.

### The Mailing List
To be used for high-level announcements and conversations. Particularly when the input of a broad range of potential contributors is sought. GitHub issues are more appopriate for many working-group specific topics, as they are integrated better with the task management and source-code version control functinoality.

### GitHub
GitHub offers a variety of integrated functionality which we propose to use in the de-facto standard way (as described by the GitHub help articles which are linked). This section first describes the top-level information architecture concepts: 'organisations' & 'repositories'. Then the suggested use of specific tools and functionality within these: 'community health files', 'wikis', 'issues', and 'project boards'.

#### Organisation (Bonsamurais)
There is only one existing Bonsai _organisation_ on GitHub. No others should be made without advanced discussion.

#### Repositories
_Guidance on when to create/merge/delete repositories is beyond the scope of this BEP_.

#### README files
As the first thing people see when navigating the GitHub website; each repository should have a README.md file which clearly describes the repo's purpose. We should follow the [GitHub recommendations](https://help.github.com/articles/about-readmes).

>   *  What the project does
>   *  Why the project is useful 
>   *  How users can get started with the project
>   *  Where users can get help with your project
>   *  Who maintains and contributes to the project

Whereas previously we were writing the "getting started" guide on a Wiki page - the readme is a more prominent and hence appropriate place, which will be seen by all potential contributors.

There should be limited duplication of information between the readmes and the 'community health files' (see below). Further examples and recommendations can be found/researched [here](https://github.com/matiassingers/awesome-readme). 

#### Other 'Community health files'
These include the licenses, contribution guidelines, and code of conduct. See this [help page](https://help.github.com/en/articles/creating-a-default-community-health-file-for-your-organization) and [this issue](https://github.com/BONSAMURAIS/bonsai/issues/17) for their implementation in the BONSAMURAIS organisation, which is a part of this proposal.


#### Wikis (**only 1**: within the 'Bonsai' repository)
Only the repository _[bonsai](https://github.com/BONSAMURAIS/bonsai)_ should have the [Wiki functionality](https://help.github.com/en/articles/about-wikis) enabled. 
All other repositories should link to content in this wiki, where appropriate.
The Wiki should be used:
* for storing persistent knowledge, which may be open to conribution, which is not already captured on the website or README files
* for end-user documentation
* for a growing list of FAQs

The Wiki should not be used for:
* task management, as the interface does not effectively support this use-case.
* source code documentation
* the getting started guide (instead, use the README.md of the BONSAI repo)

#### Issues
We should use [Github Issues](https://guides.github.com/features/issues/) for most of the written communication between contributors which is not apporpriate for the website or mailing list. Specifically functional and technical specifications are best discussed here. They are the most suitable place for writing, assigning and managing tasks and sub-tasks.

#### Project boards
[Project boards](https://help.github.com/en/articles/about-project-boards) can be used for organisation and prioritisation of Issues. 
It is possible for both _organisations_ and _repositories_ to have multiple project boards each. 

High-level organisation-wide project tracking should be handled on the [BONSAMURAIS boards](https://github.com/orgs/BONSAMURAIS/projects). Whereas projects relating to specific working groups should be managed within their respective repositories.

#### BEPS
_See BEPs 1 & 2_. These should be used for large-scale proposals and governance issues.

#### 'Notification' settings
This proposal suggests extending the usage of GitHub. A consequence of this is that contributors may need new habits in order to maintain their situational awareness. Using the GitHub [watch](https://help.github.com/en/articles/watching-and-unwatching-repositories) feature is one way this can be achieved: by watching the repos you'd like to receive notifications for. Then you must also sign into GitHub frequently or have appropriate email notification settings. _Better recommendations welcome!_



**** 

### Rationale

Broadly: to use well-integrated functionality wherever possible. GitHub is where our code is, and it makes sense to manage the project close to the code wherever possible. More detail explained above in sub-sections.

### Pros and Cons

_Not included_

### Alternatives

*  Extending/increasing usage of the mailing list
*  Managing tasks using the Wiki


### Open Issues

1.  When to create/merge/delete GitHub repositories
2.  Ideal mediums & locations for various [documentation types](https://en.wikipedia.org/wiki/Software_documentation) other than the GitHub issues for requirements. E.g. Architecture/design, source code, database, API, tests, end-user. (split between source-code, Sphinx, and the Wiki)
3.  Archiving strategy for code and knowledge generated in hackathon repository (due to the temporal nature of the hackathon, this will soon become a legacy artefact)


### Test plan

Communicate and manage the projects and knowledge following these guidelines, then survey people's perspective on whether this meets their requirements?

Also: iteratively improve if necessary as issues are found or further requirements are uncovered.


## Discussion
*  [This issue](https://github.com/BONSAMURAIS/bonsai/issues/10)
*  Bilateral video/phone conversations with Chris Mutel, Romain Sacchi, Michele De Rosa.

## Previous Versions

None.

## Copyright

All BEPs must be licensed with [CC0](https://creativecommons.org/publicdomain/zero/1.0/):

  To the extent possible under law, Tom Millross has waived all copyright and related or neighboring
  rights to Bonsai Enhancement Proposal 0004. This work is published from: The Netherlands.

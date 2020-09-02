# FRISK - Documentation

***To see the Portuguese 🇧🇷 version of this document click [here](./docs/ptBR_README.md).***

<hr />

### Introduction

Hi, this organization was made to facilitate the interaction between the members of the FRISK Project, a Undergraduate thesis made by [Gabriel Sacca](https://github.com/Gabrields1998) and [Vitor Camargo](https://github.com/vitorCamargo). This is the first thesis made by 2 people in the Federal Technological University of Paraná (UTFPR), so, for the next generation of studants, this documentation was created to make it easier to understand ways to structure their projects and make it possible to see the contributions made by students, how the writing was done, the text revisions, all accompanied by dates and logs that help to understand all the work done.

### Organization environment

For the project as a whole, development and writing, an organization was created on Github, obviously it is free and is in the name of one of the members, ideally the profile of the university/computing department would create this organization and add students and advisor, with proper roles. Creating the organization could also be the advisor's job, and as Github shares contributions, everyone involved would have the organization linked to their profiles, bringing more visibility to the project itself.

Within the organization, each repository can be separated according to the areas of development, one for the written part (documentation), and if you need more for development, it can also be created, for example, in this project, there is a front-end, back-end and a separate api that makes logs, each will have a specific repository.

It is important that, for several repositories, there is an issue manager, we recommend [ZenHub](https://www.zenhub.com/), which is used in this project.

### Issues and epics

Each of the repositories will have issues made especially for itself, however, as there are more than one repository, it is necessary to have a pattern so as not to be confused with the issues of other repositories. The standard used was `[REPO_TYPE] - NAME_ISSUE`, in our case, in the documentation repository, where the TCC is, the issues are created as `[TCC] - Introduction`, or, for the front-end repository, the issue would be `[FRONT-END] - Make main screen`.

Specifically for the written part of the work, an extra layer of organization for the work was created, which are the epics, they are the chapters of the work, in our case we have:
- `[TCC] - Introdução`
- `[TCC] - Referencial Teórico`

...

and issues are created for the work subsections, that is, the sub-chapters, such as:
- `[TCC] - Barreiras enfrentadas por novatos em contribuições de software livre` (which has a connection with the `Referencial Teórico` epic, so we know the progress of each chapter as a whole, of work as a general, and of each subchapter individually).

Github offers other tools that can help with organizing issues, such as labels, which help to understand status of issues, for example, we have 2 labels, `reviewed` and` reproved` that help to understand when a text, when being revised has been approved or will be redone. Another addition is the releases, which represent a sprint, a piece of time which must be finished with a set of issues/texts.

### Pipelines

We use the pipeline scheme, the logical order of the life cycle of an issue, we have: `New issues`, `To do`, `Doing` and `Testing` (There is also `Done`, but it comes as standard) . Every new issue is in `New issues`, at each new meeting we separate issues that will be made over time and we move to` To do`, adding the name of those who will write it, here, we adopt the issue concept for each topic of text at work, so the two cannot work directly on the same piece of text (subsection), but can work on the same chapter. As one of us starts writing about a topic, pass the issue to `Doing` and when finished, go to` Testing`, if approved, the issue placed with a label of `reviewed`, if disapproved, it goes back to` To do` with the label of `reproved` (which will only be removed when arriving at` Testing` again).

After an entire epic is reviewed and no issue is disapproved, the teacher views the work and its opinion, if everything is fine, we close the issues, if there are changes, we return the ones that should be corrected to `To do` and we add the that was spoken by the advisor in the comments.

It seems to be a long and boring process, but over time it becomes very quick to do, in addition to helping to understand the process of creating and evolving a text, so if you needed to go back to a previous version of the text, we would know by the date and we would be able to redeem more easily.

### Reviews

As we are in 2 students and the texts must be approved by both, but it is not feasible for one to write a very large chapter (causing opinion and context bias) and for both to write all parts together, we use a branch / pull request scheme / code review that is already applied to real projects in the Github community. So, to start writing a new topic, the student must create a branch from the master (or from another branch if there is a dependency), carry out their achievements, add images, etc. And when finished, submit a pull request with the changes to the master, from this point on, the other student will be able to view what has been done, start discussions or add suggestions to the work of the colleague, when everything is right, he will be able to approve the pull request. In this way, there is an agreement that each piece of the text was approved by both students, and even if a piece is more specific responsibility of one, both agreed on the finished text.

The branch default is `#ISSUE_NUMBER-EPIC_NAME-ISSUE_NAME`, it may seem confusing, but this was something suggestive, making it easy to remember what the branch will be talking about, but there may be other more compact forms of organization of the name.
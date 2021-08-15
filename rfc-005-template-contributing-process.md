# Template contributing proposed process

## Proposed by

Alyssa Rock - https://thegooddocs.slack.com/team/U012KCMPP0V

It's also worth mentioning that this proposal represents several months of work by many members of the community in both the base template working group and the community docs working group.

Special thanks to all who contributed to this process with their excellent feedback and suggestions:

- Aidan Doherty
- Cameron Shorter
- Carrie Crowe
- Deanna Thompson
- John Davenport
- Meg Albert
- Ryan Macklin
- Sachin Karol


## Proposal overview

This RFC outlines the proposed process for contributing templates to the Good Docs Project. This proposal explains:

- The workflow template contributors will follow as they begin writing a template until it is fully merged within the `templates` repository.
- The documents (deliverables) that are required for each template set and which are optional.
- Our project's template quality requirements. (Note that these quality guidelines will likely evolve over time.)
- The roles and resources our project needs to create in order to best support template contributors as they submit templates to our project.

Note that project management logistics (such as whether template projects are represented as epics or issues, how template contributors indicate the status of their template set, how templates are planned for releases, etc.) are out of scope for this proposal and will be worked out later.


## Motivation

Creating templates is core to the mission of the Good Docs Project.
This proposed template contributing process will ensure that our contributors have clear processes, guidelines, and resources as they contribute templates to our project.


## Proposal

In order to view this proposal in-depth, see these files that are included in this pull request (in this order):

- [Template contributing guide](template-contribuing-guide.md)
- [Template deliverables](template-deliverables.md)
- [Template quality checklist](template-quality-checklist.md)
- [Template roles and resources](template-roles-and-resources.md)

I'll provide a few key highlights here:

Template contributors will write templates as participants in template writing working groups that meet weekly and are led by an experienced template mentor. These template mentors will communicate regularly with the templates coordinator, who oversees the entire template process as a project manager.

Templates will be written in six different phases with certain checkpoints and milestones that each template must meet along the way:
- **Join the community** - A new contributor joins the community and find an initiative they want to work on.
- **Adopt a template** - If they are interested in contributing templates, they join a template writing working group led by a template mentor. They decide which template set to begin working on.
- **Research and draft** - They research best practices and look at examples of the type of document they are working on. When they are finished, they will create a rough draft.
- **Workshop the drafts with the community** - Revise and refine their template set with the community pull reviewers. At least three community reviews are required to move to the next phase.
- **Submit a pull request** - They open a pull request and it is reviewed for quality by the pull request reviewers. At least two pull request reviewer approvals are needed to be merged into the repository.
- **Improve the template with user feedback** - As users try the template in the wild, they may report usability issues or provide feedback for improvements to the template. Either the original template author or another templateer will evaluate feedback and incorporate it into future versions of the template. When that happens, the template will go through the previous phases again.

Each template set will include:
- **Raw template** - The basic template for the type of document you are creating. It provides a rough outline of the suggested content and a few embedded writing tips for how to fill in the different sections of the template.
- **Template guide** - Provides a deeper explanation of how to fill in the raw template. It provides a lightweight introduction to the purpose of this documentation and explains how to fill in each section of the document. Additional content may be included as needed.
- **Before you start (optional)** - This optional guide is designed to help template users understand some of the key research, brainstorming, or pre-writing steps that they might need to do before adding this type of document to a guide. If this documentation type has certain key decisions that need to be made with stakeholders or if it has a dependency on some other type of document or process, that should be mentioned in this guide.
- **Template example (optional)** - The Good Docs Project is in the process of designing a fake documentation project that can provide examples of our templates in action. Until this project is ready, template authors may optionally create an example of the template in action.


## Links and prior art

If you'd like to view the comment and revision history of these documents, you can see them in their Google Doc form:

- [Template contribuing guide](https://docs.google.com/document/d/19pLi0JMlib11g5Di076hjyUM5KRkPHPvZLQpCwmPYi8/edit?usp=sharing)
- [Template deliverables](https://docs.google.com/document/d/1uZPQ6jSj0TQoFSII_q6SbHgSySaGAZAevLvTuvXJeEU/edit?usp=sharing)
- [Template roles and resources](https://docs.google.com/document/d/1fXp0Q7mv-VFj9GxScoXG1ZahsaAnkI3drPxuVNf9JVQ/edit?usp=sharing)


## Open questions

We haven't really found a good title for the template deliverable I'm currently calling "Before you start." Cameron prefers "theory." Suggestions are appreciated!


## Decisions deferred

Project management logistics that are out of scope for now include:
- Whether template projects are represented as epics or issues
- How template contributors indicate the status of their template set
- How templates are planned for releases

Template formatting guidelines will also have to be deferred:
- Template style guidelines
- Markdown formatting guidelines
- Metadata guidelines
- Base template-related guidelines


## Consequences

Hopefully the consequence of this proposal will be that our community members have clear ways they can join a template working group and submit their first template to our project.


## Feedback

{Accepted suggestions will be incorporated into the proposal.
Additional feedback or rejected suggestions will be noted here.}


## Implementation checklist

If this proposal is accepted, the following tasks must be completed:

- [ ] Add these files to the `templates` repository and ensure they are linked from the website
- [ ] Nominate a member to fill the templates coordinator role
- [ ] Nominate members to fill the template mentor roles
- [ ] Nominate members to fill the pull request reviewer roles
- [ ] Accept volunteers to act as community reviewers
- [ ] Add template quality checklist as a pull request template to the `templates` repository
- [ ] Ensure that two pull requests from the approved list of reviewers are required to merge into the `templates` repository


## Votes

Votes as per our [decision process](https://thegooddocsproject.dev/decisions/):

Project steering committee (listed alphabetically by first name):

- Aaron Peters:
- Aidan Doherty:
- Alyssa Rock:
- Ankita Tripathi:
- Bryan Klein:
- Cameron Shorter:
- Carrie Crowe:
- Erin McKean:
- Morgan Craft:
- Ryan Macklin:
- Viraji Ogodapola:

Community members who voted (non-binding):

- {Your name}: {Your vote}

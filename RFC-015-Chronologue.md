# Chronologue processes and tools

## Proposed by

[Tina Luedtke](https://thegooddocs.slack.com/team/U02EQQDFLE8)

## Current status

- [x] Draft
- [ ] Under discussion
- [ ] Final comment and voting (until YYYY-MM-DD) {{Add date after selecting this status.}}
- [ ] Accepted
- [ ] Rejected
- [ ] Implemented
- [ ] Deferred
- [ ] Withdrawn


## Proposal overview

This proposal outlines the responsibilities, ambitions, needs, and ways of working within the Chronologue working group and how we interact with the Template working group. Specifically, the proposal discusses: 

-   [Function of the Chronologue project](#function)
-   [Role Matrix](#roles)
-   [Writing process](#process)
-   [Mock product: Technical and creative needs and a proposal for tooling](#tools)



## Motivation

This proposal aims to solidify our past decisions into a formal foundation from which the group can evolve and grow from.  
More specifically, the proposal highlights the role of the Chronologue working group within the Good Docs project, how we work, and what tools we use.

## Proposal

### Function of the Chronologue project <a id="function"> </a>

The Chronologue project is a working group within the Good Docs project. 
The primary task of the group is to create example documentation to increase the understanding of what good documentation can look like. 
The primary purpose is to educate people without a background in technical communication.
The group uses the Good Docs Project’s templates to create these examples, so the secondary purpose of the group is to act as a quality assurance for the Template working group.

To create credible examples, the group decided to build a fictional product - the Chronologue. The Chronologue is a time-travel telescope that records astronomical events of the future, and past. 

The Chronologue consists of:  

-   A time-travel telescope (fictional)
-   An API to transmit data between the telescope and the website
-   A website to view events recorded by the telescope


### Role Matrix <a id="roles"> </a>

| Role→ <br> Task↓| Working group lead | Developer    | Writer |
| :---      |    :----:   |   :----:  |  :----:  |
| Onboarding new members | X |  | |
| Assigning tasks within the group | X | | |
| Creating strategic / administrative documents like documentation plans, release notes, etc. | X |  | |
| Creating internal documentation | X |X| X|
| Writing Chronologue documentation | | | X|
| Web development||X||
| Website maintenance (Docs & Tool) |X|X||
| Review PRs |X |X | X|
| Merge PRs |X |X |X |
| Make improvements to the templates| | | X|

### Writing process <a id="process"> </a>

The Chronologue working group starts its writing process when the template is in [Phase 6 - Improve the template with user feedback](https://github.com/thegooddocsproject/templates/blob/dev/CONTRIBUTING.md#overview-of-the-template-writing-phases).

We decided to come in at this late stage because developing good templates is already quite time consuming and we don't want to add to the development cycle.

The following table describes what happens after a template has been released.

| Phase | Who does it? | What happens? |
| :---  |    :----:   |   :----  |
|1 - Plan | Working group lead| <li>Add the template to the documentation plan</li><li>Create an issue to track work <li>Assign content to a writer</li>|
|2 - Draft| Writer| <li>Create a new branch off of [`docs`](https://github.com/thegooddocsproject/chronologue/tree/docs)<li>Create Chronologue documentation using the template</li><li>Keep a [friction log](https://developerrelations.com/developer-experience/an-introduction-to-friction-logging) of template/guide for later improvements</li>|
|3 - Review | Writer|<li>Create PR against the `docs` branch </li><li>Assign WG lead or other writer as a reviewer</li><li>Improve content based on feedback</li>|
|4 - Commentary & Publication |Writer|<li>Add commentary to your content to highlight what makes it good</li><li>Merge the PR into the `docs` branch to publish the content</li>|
|5 (if applicable) - Template  | Writer| <li>In the `templates` repository, create a new branch off of [`dev`](https://github.com/thegooddocsproject/templates)</li> <li>Make changes to the template based on your friction log notes.</li><li>Create a PR and add the template author as a reviewer</li>|

### Mock product: Technical and creative needs and a proposal for tooling <a id="tools"> </a>

## Consequences

{Explain what impact this proposal will have on the community, both positive and negative.}


## Links and prior art

{This section is optional if you want to [link](https://example.com) to other resources.}


## Open questions

{This section is optional and is where you can list questions that won't be resolved by this RFC, including those raised in comments from community members.}


## Decisions deferred

{This section is option and is where you can list decisions that won't be resolved by this RFC, but which should be raised at a later time.}

-   Feedback channel for content (Reason: This should be unified across the sites we maintain?) 


## Feedback

{If you accept feedback from a community member, you will incorporate it into your RFC before it is accepted.
If you reject feedback, note that rejected feedback here before resolving the conversation.}


## Implementation checklist

If this proposal is accepted, the following tasks must be completed:

- [ ] Task number one
- [ ] Task number two
- [ ] Task number three, etc.


## Votes

Votes as per our [decision process](https://thegooddocsproject.dev/decisions/):

Project steering committee (listed alphabetically by first name):

- Aaron Peters:
- Alyssa Rock:
- Ankita Tripathi:
- Bryan Klein:
- Cameron Shorter:
- Carrie Crowe:
- Erin McKean:
- Deanna Thompson:
- Felicity Brand:
- Gayathri Krishnaswamy:
- Morgan Craft:
- Nelson Guya:
- Ryan Macklin:
- Tina Lüdtke:


Community members who voted (non-binding):

- {Your name}: {Your vote}

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
|5 (if applicable) - Template improvements | Writer| <li>In the `templates` repository, create a new branch off of [`dev`](https://github.com/thegooddocsproject/templates)</li> <li>Make changes to the template based on your friction log notes.</li><li>Create a PR and add the template author as a reviewer</li>|

### Mock product: Technical and creative needs and a proposal for tooling <a id="tools"> </a>

We want to follow good engineering practice, therefore this section separates our needs from the implementation.
That way, we can make sure that we choose appropriately for our current needs and can check in if the implementation still fits when needs change.

The Chronologue working group develops its mock tool on the [`main`](https://github.com/thegooddocsproject/chronologue) branch in the Chronologue repository. 

#### Needs:

* Framework/tool that allows for dynamic web page templating, since we want to pull in data from an API
* Needs to work with our hosting platform (Currently: Netlify OSS plan)
* Framework & knowledge support: Tool(s) need to be actively maintained and adopted by a large community. Larger projects often receive more support, and questions can be addressed by fellow community members.  
* Tool(s) need good documentation.
* Tech implementation should invite and onboard technical writers easily for maintenance later on. This can be mitigated by creating internal docs.

#### Possible technical implementation:

Since we have to build a website according to the [Chronologue mockup](https://www.figma.com/proto/lvaAChlbueycET2ws9ZquS/Chronologue?node-id=902%3A1745&scaling=min-zoom&page-id=902%3A1640&starting-point-node-id=902%3A1745), we lean towards the following implementation:

**Next.js** as our web development framework. It comes with a templating language and supports dynamic data fetching. Next.js is a mature project with extensive [documentation](https://nextjs.org/docs). It can be easily deployed through Netlify.

We are aware that deviating from our standard tech stack comes with risk. 
Ian, Chronologue's web developer, is open to experiment with data fetching, templating and page routing with HUGO. 
However, even if HUGO supports all our needs, it might not be worthwhile to switch, since development started already. 
The web development team is small (1-2 people) and they would need to refactor the whole code base, delaying the deployment date. 
Opposed to the Chronologue documentation, we don't anticipate that the mock tool needs much attention after it has been published. 


## Consequences

### Positive impact

The proposal contributes to a better understanding of the Chronologue project’s responsibilities, ambitions, and ways of working. 
Furthermore, it establishes a firm foundation on which the working group can rely on when making future decisions. 
With this RFC, we aim to ensure a smoother process to create usable, understandable examples for people that want to use the Good Docs Project’s templates. 

### Possible negative impact

The mock tool website poses a possible risk to the maintainablity of the fake tool. Since we want to divert from standard tooling (staticly generated site using HUGO), it can become a bottleneck if knowledgable members of the working group become unavailable. 
If we lose critical knowledge, we become less agile when it comes to resolving bugs or further development.  

### Mitigation strategy
To mitigate the risk of losing knowledgable members and becoming immobile, we want to supply comprehensive internal documentation about: 

* The framework we are working with and deviations from standard implementation (if applicable) 
* How the repository is organized
* How we approached the CSS and how its related to our source code
* How to maintain vital parts of the website, including security updates of the framework and dependencies
* A reference document with links to more in-depth resources.

## Links and prior art

[Chronologue Figma Mockup]([https://example.com](https://www.figma.com/proto/lvaAChlbueycET2ws9ZquS/Chronologue?node-id=902%3A1745&scaling=min-zoom&page-id=902%3A1640&starting-point-node-id=902%3A1745) created by Ulises de la Luz and Serena Jolley.


## Open questions

{This section is optional and is where you can list questions that won't be resolved by this RFC, including those raised in comments from community members.}


## Decisions deferred

While the RFC lays out what the group's purpose is and how it operates, two questions still remain to be answered as of this writing. Both of them touch on topics affect other working groups as well; therefore, these decisions should be made in other RFCs.

-   **Onboarding new members**: A bottleneck in onboarding is that the writers and developers need to establish a lot of context before they can make quality contributions. It takes a lot of time to get members into a state where they can make contributions. In the past, the working group lead onboarded members personally - mostly because of the group's velocity. Since this RFC establishes a basic understanding of the group, we could develop more text-based onboarding materials, including internal documentation. 

-   **Feedback channels**: Once we publish templates and example content, and our audience interacts with them, they might want to give feedback. Instead of being angrily tweeted at, we might want to establish dedicated feedback channels. A possible solution could be an embedded form at the bottom of a page so that we get. This would allow us to get feedback specific to our content or template. However, to have a consistent UX, we should discuss how to create consistent feedback channels across our sites. 

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

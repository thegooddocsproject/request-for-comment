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

- template-contributing-guide.md
- template-deliverables.md
- template-quality-checklist.md
- template-roles-and-resources.md

I'll provide a few key highlights here:

Template contributors will write templates as participants in template writing working groups that meet weekly and are led by an experienced template mentor.
These template mentors will communicate regularly with the templates coordinator, who oversees the entire template process as a project manager.
Additionally, a large, inclusive group of volunteer community reviewers will review templates that are in the community feedback phase.
A small group of experienced pull request reviewers will review and check the templates for quality before merging them into the `templates` repository.

Templates will be written in six different phases with certain checkpoints and milestones that each template must meet along the way:

1. **Join the community** - A new contributor joins the community and find an initiative they want to work on.

2. **Adopt a template** - If they are interested in contributing templates, they join a template writing working group led by a template mentor. They decide which template set to begin working on.

3. **Research and draft** - They research best practices and look at examples of the type of document they are working on. When they are finished, they will create a rough draft.

4. **Get feedback on drafts from the community** - Revise and refine their template set with the community reviewers. Community reviewers includes anyone who is a member of the Good Docs Project, including members of template writing working groups. At least three community reviews are required to move to the next phase.

5. **Submit a pull request** - They open a pull request and it is reviewed for quality by the pull request reviewers. At least two pull request reviewer approvals are needed to be merged into the repository.

6. **Improve the template with user feedback** - As users try the template in the wild, they may report usability issues or provide feedback for improvements to the template. Either the original template author or another templateer will evaluate feedback and incorporate it into future versions of the template. When that happens, the template will go through the previous phases again.

Each template set will include:
- **Template file** - The template for the type of document you are creating. It provides a rough outline of the suggested content and a few embedded writing tips for how to fill in the different sections of the template.
- **Template guide** - Provides a deeper explanation of how to fill in the template. It provides a lightweight introduction to the purpose of this documentation and explains how to fill in each section of the document. Additional content may be included as needed.
- **Deep dive (optional)** - This optional guide is designed to help template users understand some of the key research, brainstorming, or pre-writing steps that they might need to do before adding this type of document to a guide. If this documentation type has certain key decisions that need to be made with stakeholders or if it has a dependency on some other type of document or process, that should be mentioned in this guide.
- **Template example (optional)** - The Good Docs Project is in the process of designing a fake documentation project that can provide examples of our templates in action. Until this project is ready, template authors may optionally create an example of the template in action.


## Links and prior art

If you'd like to view the comment and revision history of these documents, you can see them in their Google Doc form:

- [Template contribuing guide](https://docs.google.com/document/d/19pLi0JMlib11g5Di076hjyUM5KRkPHPvZLQpCwmPYi8/edit?usp=sharing)
- [Template deliverables](https://docs.google.com/document/d/1uZPQ6jSj0TQoFSII_q6SbHgSySaGAZAevLvTuvXJeEU/edit?usp=sharing)
- [Template roles and resources](https://docs.google.com/document/d/1fXp0Q7mv-VFj9GxScoXG1ZahsaAnkI3drPxuVNf9JVQ/edit?usp=sharing)


## Open questions

We haven't really found a good title for the template deliverable I'm currently calling "Before you start." Cameron prefers "theory." Suggestions are appreciated! Other ideas that were floated in the community:

- Prewriting guide
- Brainstorming guide
- Template background
- Template README

I'm noting here some of the conversation that occurred around this question:

- Erin: +1 for 'before you start': very clear and helpful!
- Gayahtri: I like Before You Start as well...
- Cameron: thought (non-blocking): My reservations with "before you start" is that while this theory type doc is likely to be read before starting on a doc, I anticipate it will often be read as part of a future doc iteration, like a phase 2 improvement. Another word I've recently seen in the wild is a "primer". A primer is a conceptual document which provides the background theory related to a topic. While a primer need not be read "before you start" is does imply you should read first (like a primer coat of paint, being the first coat of paint you use). How would you feel about "primer"?
- Alyssa: I do like primer. That could possibly work well because it doesn't sound as heavy as "theory," doesn't pre-suppose when you will read the doc, and doesn't make you instantly forecast what the content is going to be. Other reactions?
- Morgan: I like primer as well.
- Aidan: I prefer "About this Template" or just "About". Filename could be -about.md. I find Before you Start problematic because in many cases content like references supporting the decisions made to construct the template are simply not of interest to end users, and so it is incorrect to say that they need to review them before they use the template. Some users will want this, and perhaps even more common will be new templateers interested in deciding for themselves if they agree with the approach taken when creating the template originally. Essential facts that the user should know before filling out the template should be in -guide, not in some other file. Primer also seems incorrect here --- it refers to an introductory educational book about a subject. The scope of what's being described is too small for primer to make sense. My understanding also is that knowledge essential to read before using the template should go in -guide. There seems to be quite a bit of overlap here about what the -guide is vs. -theory/before-you-start. I would rate this a blocking concern.
- Viraji: Out of the already proposed names, I vote for “Template background”. But I would also like to suggest “Backdrop” or “Groundwork” implying just that. Because this is likely to contain all the information that went into setting the stage for the actual template.
- John: I don't have a strong opinion here, but "Getting Started" is a common term used for this or something like it, and people will know what it means.
- Alyssa: Remember that the description for this content is "This optional guide is designed to help template users understand some of the key research, brainstorming, or pre-writing steps that they might need to do before adding this type of document to a guide. If this documentation type has certain key decisions that need to be made with stakeholders or if it has a dependency on some other type of document or process, that should be mentioned in this guide." For that reason, I don't feel like "about" accurately describes what this document does. For some extra context, the purpose of this additional optional document was discussed heavily in the Community Docs working group on August 8 and this was the decision that the 5 templateers in attendance gave. (See Community Docs notes for more context.) Here's the key takeaways:
  - Re: the base template "theory" document: The general recommendation was to include most of this material in a simpler, more lightweight form in the template guide document. The template guide document could open with a section about “Why do I need this type of document”, then it could give a guide for filling in all the sections of the document, then it could close with a list of links or references for deeper learning and research (including any Good Docs Project blog entries or white papers).
  -  We also had a brief conversation about content that seems to be missing: what about a guide that helps you do “pre-writing” and brainstorming or work through some of the research you need to do to prepare to write the template? Perhaps we could create a simple guide that asks you questions and gets you to think through what needs to be considered before you begin writing. This content could possibly go into the template guide (but that guide is starting to have a lot of content, isn’t it?) or it could be a separate document.

  That second comment forms the basis for why it was originally called "before you start." It was meant to include pre-writing activities or questions to help you do the necessary groundwork you needed to do before you even sat down to write. For that reason, I am still somewhat partial to "Getting Started" or "Before You Start" but I am also open to "Primer."
- Alyssa: Thanks to everyone who commented on the naming and content of the "before you start" document. We discussed this at length at last week's general meeting and the group consensus there was to call this the "deep dive" document. It basically contains miscellaneous information or guidance that is too comprehensive for the "guide" document. Based on whatever the each unique template needs, this document could include research, deep theories, pre-writing information, and/or any other material that users need to know when implementing this topic. Template writers are encouraged to point/link readers to that document in their guide to encourage users to read it in more depth.


## Decisions deferred

Project management logistics that are out of scope for now include:
- Whether template projects are represented as epics or issues
- How template contributors indicate the status of their template set
- How templates are planned for releases
- Whether template changes are tracked and communicated at the release level or the template level

Template formatting guidelines will also have to be deferred:
- Template style guidelines
- Markdown formatting guidelines
- Metadata guidelines
- Base template-related guidelines


## Consequences

Hopefully the consequence of this proposal will be that our community members have clear ways they can join a template working group and submit their first template to our project.


## Feedback

### Definition of deliverables
Cameron notes that you need to be careful about replicating the same definition of a deliverable in multiple documents: The explanation text from here is a copy of "Template Deliverables". This is a situation where you are creating multiple-points-of-truth for the same concept, which is a dangerous thing when scaled out to a large management of requirements level, as the points-of-truth will inevitably get out of sync. Better is to just list the title, such as "raw template" and hyperlink to the point of truth.
Don't worry about fixing here. As this is a short term proposal, it is not going to be a problem. Just something to consider for future.

### Description of template guide
Cameron also notes that the description of the template guide could be refined: This text is based on our earlier thinking re split between "guide" and "before you start". From more recent discussions, I think we having been coming to the opinion that we should push a bit more content from guide => template, and from "before you start" => guide.
Current wording is good enough for the moment, and we may refine after testing this with some real doctypes.

### Nominating individuals
Cameron had concerns about nominating individuals to fill specific roles: I'm feeling a bit nervous about pre-filling roles and titles. I think that within a healthy volunteer community, people who are going to do the work (and do it well) typically don't step up until there is work needing to be done and they have the bandwidth and motivation at that point in time. Yes, we definitely need a template coordinator now - this is an active role needing filling. But I suggest we don't assign people to roles associated with development of future templates, and don't expect that just because someone mentored a template that they were interested in, that they will also mentor other templates too. Instead, I think we should acknowledge that people will move in and out of these roles on an as needed basis.
Maybe on our template development landing page, we should include the roles of people involved in the template (which will also serve as a nice record and acknowledgement for their work).

Alyssa's response: That's fair, Cameron. But I really can't see how we would operate without having clearly designated templates coordinator or template mentors in this process. The same goes for pull request reviewers because those people will be given specific GitHub permissions that we won't freely distribute to everyone. I can see the case for not defining community reviewers though. It can simply be anyone from the community.

### Requring template examples
John notes: I personally think this should be required. It's literally my best resource when I'm looking at templates, because of the way my brain works. It should be a trivial ask.

Alyssa replies: Unfortunately, it has to be optional since our example project is not available yet.

### Template project management
Defining template project management is outside of the scope of this RFC, but I'll note comments that are still unresolved that were raised relative to project management:

- Aidan notes: It would be good to mention that you can find all the template writing issues by sorting on the "templates" label.
- Aaron notes: As it stands right now I'd expect templates to be represented by epics, either release-specific or otherwise. We may need to adjust this wording accordingly.
- Aidan notes: We might want to add a requirement here to create an issue to handle feedback and do the next version of the template, after it is finalized. This can then be assigned directly to the creator, or left unassigned (surfacing clearly that there is a gap in coverage, to facilitate governance of the content). But perhaps the template coordinator or mentors could do that.

### Number of community reviewers
Aaron notes: I'm a little worried about the level of coordination that might be required here, especially when considering iterations on templates post-v1, where each minor change requested might be represented by an issue, each of which would need the required three reviews.

Aidan adds: Maybe two reviewers needed for a new template, and one reviewer needed for an update to an existing template?

Alyssa replied: Keep in mind that we already have a requirement to author templates as part of a template-focused working group. So if you could even just get three community reviewers from your group, that satisfies the requirement. Our two template-focused working group currently both have well above three members. And then you always have the larger community to draw upon, of which we have many more than three.

Alyssa's second reply: In last week's general meeting, we decided that, for now, we'll keep the requirement to have at least three community reviews are required to move to the next phase. We'll adjust this requirement if we discover it is too difficult.

### Indicating our intended audience
Cameron notes: I think we should introduce a point or section that explains the key audience types that these documents are addressing:

1. The document author, who is the user of the template (as described here).
2. The document reader, who is the audience of the document author.

If we skip explaining these audiences, I feel our readers are likely to get confused. (Actually, they are probably going to get confused no matter what, but we can start to help them.)

Alyssa replied: I agree with you, but I wonder if this should be a separate project-wide document (e.g. our personas). I think the Content Strategy working group should create this content and that they should be responsible for putting this on our website. Then we can link to it here.

### Template file instructions
Cameron writes: I suggest breaking these bullet points into two lists:

1. Structure (using the titles you have)
2. Style (talking about how to use curly brackets, how deep to make headings, ...}

Alyssa responds: I'm not sure how to take action on this comment. Can we defer it for after the RFC, perhaps as a pull request against this document in the templates repo?

### Template formatting and questions of style

Cameron notes: I've found myself using curly brackets in two ways in the base template, and I think we should call them out separately:

1. As explanatory writing tips to the doc author. I suggest these be written with the keyword "Tip" (or similar): {Tip: Some writing tip here.}
2. As text or variables to be replaced within a sentence, such as:
This document {explains/covers/shows what/how to do something}. It is designed to help {persona or personas} to achieve {some goal}.

Cameron adds:

> :triangular_flag_on_post: I see that Alyssa has discovered how to use emojis in github text, along with a tab insert. This is pretty cool. (See this sentence for example).

I suggest that we reconsider how we do our call out tips, maybe use a combination of curly brackets and emojis.

Alyssa responds: I think we need to create a template style guide and put stuff like this in that guide. I've had that on my to-do list for awhile.

### Who we are designing templates for

Cameron writes in the template deliverables document under the first question in the FAQ for the template guide: This answer is acceptable for this first round, and I like the suggestion of making it a judgement call. I'd suggest that we actually articulate a preferred project size to help orient the template author. I've had a crack at this in Using the base template set. Quote:

**Target project**
For the raw template and guide imagine you are writing for:

- An emerging project, getting ready to publish their first 1.0 stable release;
- With 1 to 5 developers;
- Which doesn’t have a dedicated technical writer;
- Which is considering an audience of tens to hundreds of users.


### Checklists
Cameron notes: At the moment, we have a separate checklist file. I'd suggest we either include the checklist in this guide, or we have it as an external doc, but not both. My preference is to have the checklist separate, and I believe the checklist can stand alone as its own document. (A reviewer can copy the checklist and tick off the boxes separately to needing to read the guide.)
Side note: An example of a checklist for another project I've worked on: https://wiki.osgeo.org/wiki/OSGeoLive_AddProject#Quickstart_Review_Checklist

Alyssa writes: I'm not sure that I understand this comment well enough to take action on it.


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

# Glossaries repository and website

## Proposed by

Cameron Shorter

## Current status

- [x] Draft
- [x] Under discussion (until 2021-10-06)
- [ ] Final comment and voting (until 2021-10-13)
- [ ] Accepted
- [ ] Rejected
- [ ] Implemented
- [ ] Deferred
- [ ] Withdrawn

## Proposal overview

The Good Docs Project's [glossary working group](https://thegooddocsproject.dev/working-group/) wish to establish a glossary specific landing page and associated repository.


## Motivation

Within the glossary working group:
* We want to present ourselves as a stand-alone project, under the umbrella of The Good Docs Project.
* We want a website describing all details associated with glossaries, such as a landing page, howtos, current project status, how to contact us, etc.

## Proposal

We propose to:
* Establish a glossary web site at https://thegooddocsproject.dev/glossary.
* Store the website source files in The Good Docs Project's existing unpopulated github repository, https://github.com/thegooddocsproject/glossary.
* The glossary website will be published through The Good Doc Project's existing hugo infrastructure as a hugo module.
* The glossary is expected to adopt a separate theme to The Good Docs Project, with different headings, such that the glossary project can be viewed with a unique focus on glossaries. This is expected to have a link back to The Good Docs Project.
* Apply a license of CC-By 4.0 the glossary website repository.

## Consequences

* This rfc extends the separately-themed concept to sub-projects, a precedent which other sub-projects may follow.

## Decisions deferred

* What page structure and content will be on the website?
* Where will we publish the public schema for the defacto standard glossary we are developing, and associated git repository? This URL will be referenced by other schemas. We will probably use [https://w3id.org](https://w3id.org) which is used by other schemas for this purpose.
* Whether we will establish a subdomain: https://glossaries.thegooddocsproject.dev for the website. This might initially be a redirect or might be the actual homepage.


## Feedback
* bwklein:
   * I have made a video showing how the 'Blog' section (content and design) works with different layouts for that section of the site. https://youtu.be/7qJtPBXg_fc We could come up with any form of source formatting for the 'content' in the glossaries section and a different look/feel too. It's nice to be able to leverage the same tech stack for the site and have each section present the information any way you want it.  
  * One other thing that we could do, if you want to keep the glossary 'content' in a different project from the website, is to use Hugo's 'Module' system to take a file path from the Glossary project and insert that into the website 'content' folder. This is a way to 'include' files from one project into the filesystem of another and build it all into the same site. It's a pretty cool feature of Hugo.
* barbaricyawps questioned whether the glossary project fits within the mission statement of The Good Docs Project, which led to the bigger question "What is the mission of the Good Docs Project and how broad to we want to be?" Do we want to be an umbrella foundation for like-minded doc initiatives, like the Apache Foundation, or the Open Source Geospatial Foundation? Or do we want to be a targetted project, just focused on templates? Or maybe something in between? This is a conversation worth having but we decided that this RFC need not be held back by the broader mission decision. (Outcomes of this RFC can be relatively easily reversed if needed.)
* More related comments at https://github.com/thegooddocsproject/request-for-comment/pull/13

## Implementation checklist

If this proposal is accepted, the following tasks must be completed:

- [ ] Establish the subdomain glossaries.thegooddocsproject.dev
- [ ] Add the CC-By 4.0 license to [https://github.com/thegooddocsproject/glossaries](https://github.com/thegooddocsproject/glossaries).
- [ ] Set up website tooling (probably Hugo).
- [ ] Populate the website with initial content.


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

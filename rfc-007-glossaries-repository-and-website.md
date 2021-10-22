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
* Adopt the same license for the glossary website as it used by The Good Docs Project's website repository.

## Consequences

* This rfc extends the separately-themed concept to sub-projects, a precedent which other sub-projects may follow.

## Decisions deferred

* For the long term, we are yet to decide whether the glossary project should be spawned into an independent project, or should be considered a sub-project of The Good Docs Project.
* What page structure and content will be on the website?
* Where will we publish the public schema for the defacto standard glossary we are developing, and associated git repository? This URL will be referenced by other schemas. We will probably use [https://w3id.org](https://w3id.org) which is used by other schemas for this purpose.
* Whether we will establish a subdomain: https://glossaries.thegooddocsproject.dev for the website. This might initially be a redirect or might be the actual homepage.


## Feedback

### Blog setup, mechanics, and logistics
Brian writes: Sounds good to have something like this. Why a subdomain and not a subsection of the current website? Or a subdomain that redirects to a subfolder? Do you just want the subdomain URL, or a different tech stack for the website? We can easily make a new section of the website with a totally different look/feel for the content. Similar to what we are doing for the blog.

Cameron responds: I'd be interested to hear you expand on how the blog settup works, and whether the format could be set up to be very glossary specific.

Brian writes: I have made a video showing how the 'Blog' section (content and design) works with different layouts for that section of the site. https://youtu.be/7qJtPBXg_fc We could come up with any form of source formatting for the 'content' in the glossaries section and a different look/feel too. It's nice to be able to leverage the same tech stack for the site and have each section present the information any way you want it.

One other thing that we could do, if you want to keep the glossary 'content' in a different project from the website, is to use Hugo's 'Module' system to take a file path from the Glossary project and insert that into the website 'content' folder. This is a way to 'include' files from one project into the filesystem of another and build it all into the same site. It's a pretty cool feature of Hugo.

Ryan states: From a mechanics standpoint, we could:
- start with a folder, like the blog has, with what Bryan's saying
- if the need arises, we could turn it into a subdomain, with redirects in place to move it from the folder-based URL
- and have this possibility on the books for all folder-separate projects (like the blog)

Viraji states: I understand the reasoning behind why glossaries should need its own separate website/domain, so +1 on that. However, with regards to the technical details, I'm interested in what Bryan proposes - with glossaries as more of a subdomain of The Good Docs Project, different look and feel and functionality, yet falling under the main TGDP domain.

Brian writes: I'm fully in support of a dedicated glossary section of the good docs project website and will be glad to help build out a unique content model and layouts/design for it. I'm personally not interested in setting up another complete website stack for a different site at a new subdomain. But of course, other people are welcome to do so without me, I know I'm not the only one in the group who can make things show up on the webz.

Erin states: I would like to +1 the "start with a page/folder" suggestion ... way less friction to start and it's relatively simple to redirect later if a subdomain makes more sense.

### Subdomains and glossary project
Aidan writes: I’m somewhat concerned about the precedent of having a subdomain for individual templates/content types. I would tend to think a sub-directory makes more sense for this. But open to hearing arguments for why I’m wrong.

Cameron responded: An argument for why glossaries might be considered separate (but related) to The Good Docs Project is:
- Rather than being aligned with docs, Glossaries are probably more closely aligned with Knowledge Organization Systems (KOS), and standards associated with KOS, such as the Simple Knowledge Organization System (SKOS), Dublin Core, schema.org, and specific ISO standards.
- I'm suggesting that the glossary web pages should be targetted glossary builders, and the glossary related pages, without pushing people off to all the rest of the good docs pages.

Erin writes: I'm unclear on the need for a standalone identity if the glossary project is still part of TGDP? If it needs a separate identity perhaps it should be a completely separate project? I think it might be confusing to have a TGDP domain name but a completely different look.

Alyssa states: My comments are largely along the same questions as Erin's. I'm unclear on the need for a standalone identity if the glossary project is still part of TGDP? If it needs a separate identity perhaps it should be a completely separate project? I think it might be confusing to have a TGDP domain name but a completely different look.

I apologize if my comments are out of the scope for this RFC, and I worry that the next comments I make are going to sound incendiary. That is not my intent. That being said, I'm just going to frankly state that I've never fully understood why the glossaries project was part of The Good Docs Project to begin with. This RFC lays this question a little bare for me.

For example, Cameron said earlier: "Rather than being aligned with docs, Glossaries are probably more closely aligned with Knowledge Organization Systems (KOS), and standards associated with KOS, such as the Simple Knowledge Organization System (SKOS), Dublin Core, schema.org, and specific ISO standards."

If glossaries are not aligned with docs, how is this not a separate project entirely? Yes, there is some tiny overlap in terms of personnel who work on both glossaries and Good Docs Project. (Cameron and Ankita, maybe Nelson?) But other than that somewhat coincidental fact, the projects have almost entirely different community members, workflows, and purposes. To be fair, I can see how there might also possibly be some loose overlap in terms of end users in the sense that end users who are interested in doc tools and resources might also be interested in glossary tools and resources. But that's about the only overlap I can see.

At the end of the day, I don't see how the glossaries project supports the Good Docs Project mission. To me, it sounds like these are indeed two different open source projects and should be treated as such. So, I think we need to maybe start by answering that question. Because if the glossaries project doesn't really support the GDP mission or purpose, then I feel very hesitant to devote our own project's time, energy, and resources toward it.

If these are indeed two different projects (as I suspect they are), maybe it's also time for glossaries to create its own GitHub org, its own web domain, its own Slack, and have its own leadership structure. Maybe we should begin thinking of the relationship between the GDP and glossaries the way we think about our relationship with Write the Docs (WTD): there's a lot of community crossover and shared interest in common goals, but they're two different groups with different goals and aims, and different leadership structures. The relationship between GDP and WTD is mutually supportive and friendly and recruitment across communities is fully tolerated, but no one would ever think they were the same org, because they're not. And their resources are deployed entirely differently.

For that reason, I am okay with people working on both the GDP and glossaries. There's no rule stating you can only contribute to one open source project at a time. I'm okay with a partnership of sorts with the glossaries project. I'm also sort of okay with Cameron telling the GDP members about the glossaries project and inviting members to work on that project if they seem to have a genuine interest in it. But maybe we should re-examine whether we are in fact two different projects and whether we have more of a partnership relationship rather than an umbrella relationship.

I promise I'm not trying to be combative or territorial or that I want to stop the momentum for the glossaries project. But this question has been nagging me for many months and now this gives me a reason to articulate these concerns and start a dialogue about this topic. I hope you'll appreciate that I only want to have a discussion and that I'm 100% open to having my mind changed. Help me to see how the glossaries project supports the GDP mission.

Cameron responds: 

I agree that establishing a separate glossary project is a valid and reasonable suggestion. It is something we have discussed within our glossary project. We've also considered becoming part of the inter-related open source software projects paneron or glossarist. Or possibly becoming part of a standards organization such as ISO TC211 or the OGC.

Let's start by defining what artifacts we are creating as a project:

1. We are creating a standard for glossaries. This will be relatively light weight, but there is a case for creating a new project for it. We wouldn't want to sit under ISO because ISO puts all standards behind a paywall and we want an open standard. The OGC is spatially focused and not a logical fit. And we don't have relationships with other standards bodies.
2. We will create processes, articulated as guides published on a website. These are likely to align with the "deep dive theory" document we are developing for The Good Docs Project. Although they might go further than other templates.
3. We will create a glossary template, which would follow The Good Docs Project format.
4. We expect there will be software tooling created with implements our processes, but these are anticipated to be created in separate (sometimes competing) projects. Hence it is a good idea to keep the standard separate from the software.

So why might we want a glossaries project associated with The Good Docs Project?

1. Most of what we are generating is process and a guide for a documentation concept (glossaries). At the very least, the glossary template aligns directly with The Good Docs Project.
2. Assuming both projects are high value, there is potential for increased brand value for both glossaries and The Good Docs Project by associating with each other.
3. A question: Do we want to limit The Good Docs Project to just focus on templates, or do we want to be an umbrella foundation (like the Apache Foundation or the Open Source Geospatial Foundation), where we establish a quality brand and processes, which are adopted by multiple documentation related initiatives? We initially started with a long term goal of a foundation type model, and I think have been growing in that direction.
4. Establishing the infrastructure behind an open source project is time consuming, and it would be helpful for the glossaries project to piggy back on the prior work and processes already in place for The Good Docs Project, with relatively small burden to The Good Docs Project.
5. The glossary work is still in a formative stage at the moment, and just needs a place to put our docs which potential collaborators can be pointed to. Sitting in under The Good Docs Project is a reversible decision, and it will be possible to spawn off a new project in future if it becomes a logical thing to do.

Morgan responds: Entirely up to you on whether that is the path, but coming from a doc-ops focused background I value the idea of operationalized knowledge and to me glossaries serve as critical piece of the IA (Information-Architecture) for docs as they give rise to the structure and relatedness of content. As we build better tooling for our templates the ability to connect docs and glossaries as part of a doc-set has more impact.


## Implementation checklist

If this proposal is accepted, the following tasks must be completed:

- [ ] Establish the subdomain glossaries.thegooddocsproject.dev
- [ ] Update the license of [https://github.com/thegooddocsproject/glossaries](https://github.com/thegooddocsproject/glossaries) to align with The Good Docs website license - based on Creative Commons by Attribution.
- [ ] Set up website tooling (probably Hugo).
- [ ] Populate the website with initial content.


## Votes

Votes as per our [decision process](https://thegooddocsproject.dev/decisions/):

Project steering committee (listed alphabetically by first name):

- Aaron Peters:
- Aidan Doherty:
- Alyssa Rock:
- Ankita Tripathi:
- Bryan Klein: +1
- Cameron Shorter:
- Carrie Crowe:
- Erin McKean:
- Morgan Craft:
- Ryan Macklin:
- Viraji Ogodapola:

Community members who voted (non-binding):

- {Your name}: {Your vote}


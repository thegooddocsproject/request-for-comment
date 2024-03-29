# RFC002 - Blog content publishing model

## Proposed By

Ryan Macklin ([@macklin](https://thegooddocs.slack.com/team/U01DYRWG43X)) , Carrie Crowe ([@Carrie Crowe](https://thegooddocs.slack.com/team/U01QS8YAHHN))

## Proposal State

- [x] Draft (submitted to GitHub on May 26, 2021)
- [x] Under discussion
- [x] Waiting on dependencies (RFC-004)
- [x] Final comment and voting ({{date}})
- [x] Accepted
- [ ] Rejected
- [ ] Implemented
- [ ] Deferred
- [ ] Withdrawn

## Proposal Overview

Producing and hosting blog posts content, including publication ownership and models.

### Motivation

Part of promoting good documentation is helping those uncertain about (or overwhelmed by) what constitutes good docs and best practices. We seek to create a space where the community can contribute to the body of knowledge, as it relates to the mission of the Good Docs Project.

We also want to foster community contributors, to elevate voices that aren't elevated and to empower individuals to be thought leaders in their careers.

### Proposal depencencies

The proposal requires the following to be resolved before it be fully implemented:

- Content strategy working group decisions that impact website content
- Resolution of website license conversations (RFC004)

## Proposal Details

Regarding specifics on dates and number of participants, this proposal represents our blue sky ideal. It's intended to be flexible with reality, but for simplicity's sake we won't keep mentioning that as a caveat throughout this document.

### Scope of proposal

This proposal focuses on "community-driven media," namely **blog posts** (and possible later videos or podcasts) about individual topics, created by individual community members and based on those individual viewpoints. All these media elements will be curated by the editorial collective, steered by the core publishers (and input from the Project Steering Committee).

The audiences for this media are:
* Developers and other "non-technical writers" looking to empower themselves, either in using our templates or in other applicable writing advice
* Technical writers in that same position
There is no expectation that either audience will also be GDP contributors or community members. Material will always shoot for outside of the contributor sphere.

#### Out of scope

This proposal doesn't cover **white papers**, though it does address some nuance between white papers and blog posts for clarity.

This proposal also doesn't cover the potential for other media like **videos or podcasts**, but that could be a future expansion.

This proposal also doesn't cover social media, but is certainly tethered to that element of community engagement.

#### Aside: defining white papers vs blog posts

In this model, **blog posts** are community contributions to general knowledge about technical communication, an informal stance of Good Docs Project template support, or other points of interest for those interested in GDP's mission and broader content.

They're periodical content, to keep engagement up. They're individually credited, and live on a dedicated blog subfolder on GDP's website.

To contrast, **white papers** would cover topics core to Good Docs Project templates, in philosophy and execution. They would be created by community consensus and represent the community as a unified element. They would live on the core GDP website, rather than in the publication models outlined below.

White papers are created as needs arise, rather than an ongoing periodical model to keep external engagement up.

The blog team will be very happy to be involved with white papers, including co-running it to lend editorial expertise, but doesn't want to muddy this proposal by including a different sort of publication.

#### Out of scope for now: templates for this content

Templates are great! That's why GDP exists. But rather than starting with blog post templates, we want to give freedom for various forms of conversational writing.

That said, some months in we do want to examine our content for templating, as that empowers onboarding contributing.

### Content types

All media is community-contributed pieces on documentation philosophy, best practices, and related opinion or research pieces. They are individually created and driven, representing a viewpoint within the community that the community respects enough to be associated with it, but with bylines that attach the viewpoint to the original author or authors.

(This means the authors and the community co-own any potential fallout from poorly received posts.)

Blog posts are 500- to 1000-word pieces about a subject, whether that's a single topic, a top N post, a collection of interesting links with commentary, and so on. Some posts will be solidary, and others will be part of a series.

#### Where content would live

Blog posts would live on (our website)[http://thegooddocsproject.dev], as a folder. Bryan Klein has already donated time and energy into a Hugo build for our blog, with a lot of modularity and customizability. (This is a pivot from originally suggestion Medium.com, which we're moving away from because of the paywall factor.)

Regarding external housing (should it become relevant): It's the responsibility of the publishers to make the Terms of Service of those services known to the Project Steering Committee. That includes any changes we're aware of.

### Organization & personnel

First, the blog ideally operates on a "fail early, learn, keep on keeping on." Keep that in mind.

Publication standards are important to all organizations, especially to those promoting publication standards themselves. To that end, there's a hierarchical model borrowed from Ryan's periodical background.

* There's a central **publisher** role, held by two people. They have publication rights on the external accounts (such as YouTube). They maintain the publication queue and quality, and have as part of their role to also recruit contributors.
	* First publishers would be: Ryan Macklin & Carrie Crowe.
	* The GDP chair is also in this role, with respect to account access.
* There are **editors**, who edit pieces to align with our community standards and style. We'll want two editors—and only two editors—involved in any one piece, to keep editors from burning out and to keep the signal/noise ratio down.
	* Publishers are also editors, and it should go without saying that an author is never their own editor.
* Anyone in the blog group can be a **reviewer** when reviews are solicited. Pieces should have reviews solicited.
* Anyone in the blog group can submit a proposal for a piece they want to create. Such pieces would be one-off blog posts, and when green lit will go through the process of drafting, reviews, edits, and finally entering the publication queue.
	* A few authors may do a series, but that will be limited—partly because our publication queue can't maintain several series, and partly because we want to see what contributors provide to the group before promising to support a series.
* Anyone in the blog group can add to a topic wishlist.

#### Publisher role rotation

We want to encourage publisher rotation. This could mean one publisher steps down every six months or year, allowing an interested editor to fill that role. This means part of being an editor is getting the specific experience needed to take on the role of publisher. (The first handoff may be bumpy, so we'll play this by ear.)

The depends on both checking the bandwidth of our publishers and potenitally willing editors. We'll start this clock once the blog is launched. We'll keep this flexible for now, and change if a need for a stricter timetable arises.

### Publication rights & ownership

The creators of each piece will retain ownership of their pieces, and the Good Docs Project asks permission to publish that version of their piece in perpetuity. From a licensing perspective, that's covered as the results of RFC-004.

Important elements to have on record regarding this topic:

1. We want to allow contributors a space to incubate their ideas, which means in some cases a space to develop IP they want to work with later—such as in a talk or book down the road. And we want our contributors to feel good about having added to GDP's body of knowledge, rather than regret "giving up a good idea."
2. There is an unfortunate history of privileged classes taking work created by marginalized people, and profiting off of that work without recognition of or compensation to those people. Because of the individual nature of each post, we should strive to not be a part of that history.
3. Such media doesn't need to be replicated and altered in the way code bases are. Code bases and similar need legal declarations to protect those using them. The replication and alteration process is a personally interpreted one, and it doesn't necessitate the same sort of legal declaration (either liability license or replication permission).
4. We want to be good facilitators and custodians of community knowledge, and encourage our participants to see themselves as empowered to donate their insights to the global community of technical writers and those interested in the craft.

### Publication cadence

We want to soft-launch our blog content two months after this RFC is accepted. Initially, blog posts would come out once a every two weeks. Within a few weeks or months, we'd like to move to an every-week cadence. We'll play that by ear, and adjust as we need to.

Ideally, we want to build up to a six-item queue of content for blog posts.

## Open questions/thoughts (non-blocking)

* Over time, we'd like to see how to get an organization-wide Drive, as being able to develop content in a system designed for written material would be of great benefit. Submitting to GitHub is planned as a later stage in the process, because of the limits of git's editor and commenting capabilities for non-code content. (This is touched on in RFC003.)

## Ambition vs. reality

We recognize that the dates we provide are ambitious, tempered with some respect for contributor bandwidth. They've already slid during this RFC process, so we want to recognize the dates and numeric specifics are goals, not requirements or a litmus test for a successful subproject.

## Reference Links

* [#blog Slack channel](https://thegooddocs.slack.com/archives/C01SDNR5X1C)
* [Blog working group draft responsibility model, brainstormed late April 2021](https://jamboard.google.com/d/1iyfr4A9GcdRbvnkrokfg6YGXTBhIgmeA55UTBvtN_-o/viewer)
* [Blog working group's temporary Google Drive folder](https://drive.google.com/drive/folders/1UCIwyvmOa4Gh5nBmXu1GckrI7mfeT2AW?usp=sharing]) (owned by Ryan's personal account)
* [Blog working group's meeting notes](https://docs.google.com/document/d/18T2dku9WMRLJTq1rcnFwuUeA1i-thVLOtVqhX2SOxIY/edit?usp=sharing) (last meeting in late April; meeting cadence is TBD)
* [Content style guide](https://docs.google.com/document/d/1St73OBFhbQT4hNKp-cayTjDfjOltZSMP7X2Z4QBzgQo/edit) (in notes form, not yet following a template)
* [GDP meeting notes](https://docs.google.com/document/d/13xr5PLMMqm6Rz_yXzxl5WMOwY9H6liB1abU_i0-ws60/edit#) (where various blog discussions happen at a larger-org level)

## Initial Implementation Checklist

If this proposal is accepted, we'll do the following to spin this up.

- [X] Initialize the blog site
- [ ] Complete initial version the blog core project document (intended as a living source of truth, unlike this static RFC)
- [ ] Complete initial version the blog sub-style guide (a living document meant to grow and evolve over time)
- [ ] Begin drafting one or two initial editors outside of the publishers
- [ ] Provide an initial solicitation process for blog posts
- [ ] Provide an editorial pipeline process for blog posts, so reviewers and editors have a reference

We expect these to take roughly two months to achieve this setup, most likely concurring with the beginning of publishing.

Naturally, these count for those steps we're aware of at the onset. We'll likely uncover more as we progress, though adding them to this doc post-acceptance is out of scope.

### Intended Next Steps

These points are out of scope for tracking in this document, but worth pointing out as effort to take in the two to three months post-acceptance.

- Populate the blog queue with at least four articles before beginning biweekly publication, written by the publishers to set the initial tone
- Sync with social media initiatives and other community outreach (such as any newsletter plans)
- Set a regular cadence for working group meetings
- Outreach for guest writers, such as Write the Docs speakers who might want to write about a topic

## Feedback & Change Log

Cameron Shorter on 5/16 via slack (already implemented per discussion):

1. Nice work. This will be really valuable
2. We should agree on spelling of "The Good Docs Project". I'd err toward a url of thegooddocsproject rather than the-good-docs-project to align with [thegooddocsproject.dev](https://thegooddocsproject.dev)
3. With regards to hand over of roles, I suggest doing that in March instead of July (to align with our election schedule) [thegooddocsproject.dev/roles/#selection-of-roles](https://thegooddocsproject.dev/roles/#selection-of-roles])
4. I'd suggest soften publishing criteria to increase the bus factor and allow for an elastic volunteer workforce. That is, say "we will typically publish bi-monthly", which gives you the flexibility to take a break over Christmas. Likewise, "We typically aim for two editors". (Still keep the quality criteria which I think is very important to long term success.)

Other changes made between sharing initial draft in Google Drive (5/12/2021) and the GitHub repo (5/26/2021):

- Implemented Cameron's feedback.
- Added details to implementation checklist, plus non-binding future checklist for clarity.
- Adjusted video launch timeline by a few months, to give the blog content workflow time to solidify and get established in the wider community.
- Added reference to external housings' terms of service.
- Added open questions section for anything non-blocking but potentially worth addressing. These don't need to be discussed within this RFC process.

Revised on 6/30 to incorporate:

- Moving away from Medium.com to a locally hosted Hugo blog
- Shifting the license dependency to the general site's licenses page
- Decreasing the ambitious cadence of blog posts
- Not committing to a start date on videos, to test the blog process first
- Other minor tweaks

Revised 7/14:
- Retired "Procope" as a term.
- Removed video elements. We aren't ready for that, and a new RFC should happen when we are that reflects what we've learned and where we want to go at that point.
- Minor updates relating to newer RFCs and other converstions since last update.

## Voting

Votes as per our [decision process](https://thegooddocsproject.dev/decisions/):

Project steering committee (listed alphabetically by first name):

* Aaron Peters: +1
* Aidan Doherty: +0 (abstain)
* Alyssa Rock: +1
* Ankita Tripathi: Didn't vote
* Bryan Klein: +1
* Carrie Crowe: +1
* Cameron Shorter: +1
* Erin McKean: +1
* Morgan Craft: Didn't vote
* Ryan Macklin: +1
* Viraji Ogodapola: Didn't vote

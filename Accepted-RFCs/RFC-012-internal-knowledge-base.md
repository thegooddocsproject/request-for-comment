# RFC-012: Internal Knowledge Base
## Proposed by

Ryan Macklin ([@macklin](https://thegooddocs.slack.com/team/U01DYRWG43X))

Initially submitted on 24 Aug 2022

## Current status

- [x] Draft
- [x] Under discussion
- [ ] Final comment and voting (until YYYY-MM-DD) {{Add date after selecting this status.}}
- [ ] Accepted
- [ ] Rejected
- [ ] Implemented
- [ ] Deferred
- [ ] Withdrawn

## Proposal overview

We need a central knowledge repository for contributors that:
* Isn't fragmented across different platforms or accounts
* Is easy for new contributors to access
* Has a sense of hierarchy
* Allows contributors to dump critical or needed info in a place that keeps them from being a bus number
* Has some sense of discipline/oversight to keep it from becoming disorganized or discordant

## Motivation

We don't have a good way to share information to use contributors, or a common places where information can live and grow. This was mentioned by multiple people during our recent retrospectives.

## Proposal

We could use a GitLab wiki or repo as a place where contributors can post material or comment on said material with questions, corrections, etc.

We'd have some guideline on structure, intent, etc. Each core initiative would have a space for their information, along with general information, community resources, etc.

Ideally, our docs would make use of our templates—in fact, they would make for great use/test cases. However, we would allow for a "quickly written" status, in cases where information needs to be dumped from someone's mind, but the time/effort cost in polishing isn't currently possible.

We'd have a mechanism for checking the freshness of content, though we can defer the details of that until later.

### GitLab wiki: a.k.a. Do we already have this?
There's a wiki in GitLab, and [Aaron has release weight information there](https://gitlab.com/tgdp/governance/-/wikis/Guide-to-assigning-weight-scores-to-issues-and-epics-%28release-planning%29). Should we just go with that? Does that make sense for us as a group of groups?

Is the wiki going to be oversaturated with other purposes? Would it be difficult to use search functionality when looking for KB articles, due to non-KB stuff in the wiki also populating the search results?

## Consequences

We'd have a central place for information.

Said information though could become out of date without a contributor realizing it, due to the nature of knowledge bases and the bandwidth of contributors.

We also need to decide on the access control. Having new contributors being able to edit can be great for finding holes in the content, but could also be an issue if contributors put misunderstandings into our KB without others noticing right away.

This space would also be great for small procedural elements that should be documented, but don't need a full RFC for said documentation (such as the recent "break/restart" process the co-chairs initiated). That way such info isn't lost to the ether due to a lack of documentation procedure for such things.


## Links and prior art

{This section is optional if you want to [link](https://example.com) to other resources.}


## Open questions

{This section is optional and is where you can list questions that won't be resolved by this RFC, including those raised in comments from community members.}


## Decisions deferred

* Freshness mechanisms
* Access control (a.k.a. who can edit/update)


## Feedback

{If you accept feedback from a community member, you will incorporate it into your RFC before it is accepted.
If you reject feedback, note that rejected feedback here before resolving the conversation.}


## Implementation checklist

If this proposal is accepted, the following tasks must be completed:

- [ ] Set the site/wiki/whatever up
- [ ] Draft the core info on how to use & contribute, so we're all on the same page about it
- [ ] Create the initial structure/document tree
- [ ] Ask group leads to dump critical or infrastructure knowledge from their brains or disparate notes into the KB


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
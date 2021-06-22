# RFC001 - ZenHub for TGDP Product Management

## Proposed By

Aaron Peters


## State

- [ ] Draft
- [x] Under discussion
- [ ] Final comment and voting
- [ ] Accepted
- [ ] Rejected
- [ ] Implemented
- [ ] Deferred
- [ ] Withdrawn


## Proposal Overview

As The Good Docs project matures, we should strive to make regular releases to the community. Implementing a product management solution will provide transparency, and allow us to plan releases that regularly provide value while balancing the available bandwidth of project volunteers.


## Motivation

As The Good Docs Project grows, both in scope and in membership, a more formal “source-of-truth” for the org’s ongoing development will help ensure continued progress. This is particularly true given recent discussions of conducting meetings for individual Working Groups, during which decisions will be made and tasks taken up that would otherwise be difficult to coordinate using the default GitHub mechanisms.

To this end, this proposal includes the supplement of the current work management system (GitHub) with enhanced project/product management capabilities.


## Proposal

In an effort to coordinate work across multiple working groups, this proposes the addition of [https://www.zenhub.com/](ZenHub) to the existing GitHub account for TGDP. This will bring multiple benefits including:

* The ability to add multiple repositories to the Workspace.
* The ability to define multiple projects for the Workspace.
* The ability to group related tasks (Issues) into Epics.
* The ability to add Epics into Milestones.
* A project-level, consolidated Roadmap view that provides visibility across the activities of individuals and Working Groups.

ZenHub was chosen for this proposal for the following reasons:

* It provides the core capabilities of accommodating multiple workstreams, triage/backlog management, and release planning.
* It provides free accounts for open source projects and orgs.
* It appears to be largely backwards-compatible (see the below section for more detail).

ZenHub is an app that, once granted access to GitHub assets, allows them to be assigned specific tags. These tags are then given special representation in the UI: for example, Issues with the **Epic** tag are items that show on the Roadmap, where Issues without this tag are not. Furthermore, issues without the tag can then be assigned to Issues that have it.

In this respect, ZenHub uses established GitHub mechanisms to implement its features. And so in the event the org needs to switch to another alternative (or otherwise stop using ZenHub), it appears basic GitHub data (such as base-level issues) will remain intact. //Note: it does appear in this circumstance that some re-work, such as grouping the base-level Issues into Epics, would need to be re-done).


## Implementation Checklist

- [ ] Confirm decision on platform proposal (ZenHub)
- [ ] Define organizational structure (workspaces by Working Group? by deliverable? Epics?)
- [ ] Scrub existing issues: validate, categorize, prioritize.
- [ ] Create next release (discuss release scheduling).
- [ ] Working Groups to define what will be included in the next release.


## Voting

Project steering committee (listed alphabetically by first name):

* Aaron Peters:
* Aidan Doherty: +1
* Alyssa Rock:
* Ankita Tripathi:
* Bryan Klein:
* Cameron Shorter:
* Clarence Cromwell:
* Erin McKean:
* Morgan Craft:
* Viraji Ogodapola:

Community members who voted (non-binding):

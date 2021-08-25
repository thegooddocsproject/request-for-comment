# RFC006 - Release Planning & Management Process

## Proposed by

Aaron Peters (@acpkendo)

## Current status

- [x] Draft
- [x] Under discussion (until 2021-09-15)
- [ ] Final comment and voting (until YYYY-MM-DD) {{Add date after selecting this status.}}
- [ ] Accepted
- [ ] Rejected
- [ ] Implemented
- [ ] Deferred
- [ ] Withdrawn


## Proposal overview

This proposal outlines a process to plan for and manage releases for The Good Docs Project. Specifically, it will detail:

- The process through which the project defines and agrees on a Release;
- The versioning scheme the project will use to track and communicate progress across Releases, and;
- The tooling the project will use to manage progress towards Releases.


## Motivation

The Good Docs Project has grown to contain multiple sub-initiatives ranging from the templates (arguably the core of the project's activities at time of writing), to tooling aimed at technical writers, to useful content in the form of example documentation and blog posts.

Given the project's increasing membership across multiple time zones, implementing a standard process through which the Project Steering Committee can define and manage releases will align expectations and better enable monitoring of progress.


## Proposal

The release planning process will be a collaborative process between members, their Working Groups, and the Project Steering Committee, and the Release Manager as follows:

1. The PSC will decide on a target date for an upcoming release. This can be driven by the desire to release together with a particular event (e.g. at a Write The Docs conference), or based on a regular schedule (such as quarterly). The overall project release will be tracked in a TBD location: ZenHub if it supports recursive Epics, or e.g. a wiki if not.
1. Based on a target release date, Working Groups will convene and decide (based on capacity) the items to which they can commit. They will be able to plan the precise issues they will complete as part of a release using their workspace in the ZenHub application.
1. The PSC will evaluate each Working Group's release plan and provide feedback. As the plan will be based on a realistic bandwidth estimate, the PSC should focus on identifying items to be added/removed based on strategic priorities. The PSC and Working Groups will negotiate and come to a consensus on what from each sub-project will be included in the release.
1. The Release Manager will track progress towards the release's goals as reported in ZenHub, and will be responsible for identifying slippage and risk. The Release Manager will provide regular updates to the project's members as part of the regular meetings, although overall progress will be available anytime from ZenHub for members with access.
1. If the release appears at risk for slippage, the Release Manager will coordinate with the Working Groups to see if progress can be brought back to the baseline, or if items will need to be removed from the release. The Release Manager will inform the PSC if the latter occurs, to determine if this is feasible, and if not how it should be handled.
1. Working Groups will provide an update/demo of the results of their work in preparation for the release. Once the PSC and other stakeholders are satisfied that it meeds the commitment, members of the project can perform the necessary reviews/approvals, merge pull requests, and package the Working Groups' deliverables.


## Links

- [Meeting notes from discussion on versioning](https://docs.google.com/document/d/1Oc3hNhJRrXsr-abEmUKAdamC5aKJydtldvpcSK_Hv_E/edit)

## Feedback
{{Reviewer name}}:
- {{I suggest that ...}}
    - {{Community member name}}: {{Additional comment on same topic.}}
    - {{Proposer name}}: {{Addressed by ... / Ignored because ... / ...}}


## Implementation checklist

If this proposal is accepted, the following tasks must be completed:

- [ ] Confirm/decide on the mechanism to manage project-level releases.
- [ ] Configure ZenHub with necessary workspaces and link projects.
- [ ] PSC to identify the first target release date.
- [ ] Working Groups to make initial commitments towards first release.


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

- {{Your name}}: {{Your vote}}

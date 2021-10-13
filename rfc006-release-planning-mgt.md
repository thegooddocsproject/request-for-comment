# RFC006 - Release Planning & Management Process

## Proposed by

Aaron Peters (@acpkendo)

## Current status

- [x] Draft
- [x] Under discussion (until 2021-09-29)
- [ ] Final comment and voting (until YYYY-MM-DD)
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


## Motivation for Releases & a Release Planning Strategy

Many volunteer open source projects will release new versions of their output (software) whenever it's deemed to be in a user-ready state that includes new value. But The Good Docs Project has identified a few prevailing reasons for creating formal Releases of our outputs, as follows:

- For technical writers, creating formal releases makes it easy to ensure they're always working from the latest stable/approved versions of templates.
- For integrators (i.e. those who might create solutions based on our work), well-versioned releases make it easy to ensure (backward-)compatibility and plan future development of their downstream products.
- For project members, it aligns expectations on when to target tasks for completion, and way to ensure only updates of the appropriate value and quality are distributed to users.

The Good Docs Project has grown to contain multiple sub-initiatives ranging from the templates (arguably the core of the project's activities at time of writing), to tooling aimed at technical writers, to useful content in the form of example documentation and blog posts. Given the project's increasing membership across multiple time zones, implementing a standard process through which the Project Steering Committee and Working Groups can define and manage releases will align expectations and better enable monitoring of progress.


## Definition of a Release of The Good Docs Project

As an organization with multiple sub-projects (some of which arguably have their own sub-projects) working with different cadences and outputs, we'll define for the purposes of the process this RFC describes what constitutes a "release" from The Good Docs Project. It's been noted that The Good Docs Project will produce two types of outputs:

- "Product Outputs," or assets such as templates that will actually be used by our core audience in their own documentation efforts, and;
- "Non-Product Outputs," which includes thought leadership, whitepapers, and other content that may inform documentation efforts but will not be used directly.

A release constitutes:
* A list of Product Outputs and their features which are to be included in the release.
* A definition of quality to be applied to the release, such as "stable", "beta", "bleeding edge", as defined by our internal processes. All proposed features will be expected to meet this criteria, otherwise it won't be included.
* A statement of planned support that will be applied to the release (which might be "no support", or "security and typo patches").
* A release date, which will typically align with a key event, such as a conference.
* A working schedule with key milestones. A sub-project will be expected to meet the milestones or risk having proposed updates being excluded from the release.
 

At the time of writing, the following outputs are considered Product Outputs of TGDP:

- The Templates collection
- The Doc Tools initiatives
- The Chronologue project, by virtue of its inclusion as examples to both the above

Note however that while a given Release from The Good Docs Project may not include any *updated* material as part of a Product Output, its current version will still be included as part of any release packages that are creation. For example, the Doc Tools Working Group may release a new version of that software as part of a Release implementing a new feature. But the Chronologue WG's content included with that software need not be updated at all, unless the new feature specifically requires it (e.g. it makes use of a new metadata field).


## Roles and Responsibilities

The main participants in the Release Planning Process are as follows:

- Project Steering Committee: The PSC will collectively provide input into goals for releases, and review/approve proposed release plans.
- Release Manager: This role will be responsible for driving the planning process for future Releases, and for maintaining an easy-to-understand status on any in-process Release(s). This individual will interact regularly with Working Group leaders to understand current progress, and update the PSC if it's trending away from targets.
- Working Group Coordinator: Each Working Group should designate a coordinator, who will work with the Release Manager in reviewing the goals of the Release and determining if they are feasible given available time and volunteer bandwidth. The will also provide updates on the WG's progress during the course of a Release. While Coordinators will be responsible for gathering the progress of their WG's members, the Release Manager will establish communication channels that will make this efficient.


## Proposal

The release planning process will be a collaborative process between members, their Working Groups, and the Project Steering Committee, and the Release Manager as follows:

1. The PSC will decide on a target date for an upcoming release. This can be driven by the desire to release together with a particular event (e.g. at a Write The Docs conference), or based on a regular schedule (such as quarterly). The overall goals of the project release will be tracked in a TBD location: ZenHub if it supports recursive Epics, or e.g. a wiki if not.
1. Based on a target release date, Working Groups will convene and decide (based on capacity) the items to which they can commit. They will be able to plan the precise issues they will complete as part of a release using their workspace in the ZenHub application.
1. The PSC will evaluate each Working Group's release plan and provide feedback. As the plan will be based on a realistic bandwidth estimate, the PSC should focus on identifying items to be added/removed based on strategic priorities. The PSC and Working Groups will negotiate and come to a consensus on what from each sub-project will be included in the release.
1. The Release Manager will track progress towards the release's goals as reported in ZenHub through regular iterations (sprints), and will be responsible for identifying slippage and risk. The Release Manager will provide regular updates to the project's members as part of the regular meetings, although overall progress will be available anytime from ZenHub for members with access.
1. If the release appears at risk for slippage, the Release Manager will coordinate with the Working Groups to see if progress can be brought back to the baseline, or if items will need to be removed from the release. The Release Manager will inform the PSC if the latter occurs, to determine if this is feasible, and if not how it should be handled.
1. Working Groups will provide an update/demo of the results of their work in preparation for the release. Once the PSC and other stakeholders are satisfied that it meets the commitment, members of the project can perform the necessary reviews/approvals, merge pull requests, and package the Working Groups' deliverables.


## Toolset

In as described above, this process will leverage three major tools to plan and manage releases.

- Wiki: The high-level goals and commitments of a Release should be documented on a publicly-available wiki, to align expectations and provide transparency. The Release Manager will collect proposals from the Working Groups, and facilitate the discussions between Working Groups and the PSC to reach a consensus on the Release's contents.
- GitHub: Work towards the goals of the Release will be represented by Issues in GitHub. GitHub will also be used to distribute the end products, either directly from source repositories, or as packages (e.g. .ZIP files) for end users to download from the **Releases** page of the appropriate repository.
- ZenHub: ZenHub will provide organization and visibility through its ability to group individual work items (e.g. Issues) into higher-level Epics, and show progress toward their completion.


## In Scope

All Working Groups and sub-projects of The Good Docs Project are eligible for inclusion in a Release. That said, the precise contents of any Release should be reached through consensus between the PSC, who should seek to maximize the value delivered, and the Working Groups, who should ensure commitments are feasible.


## Dependencies

This RFC should be considered together with RFC-008, which describes in detail the versioning and numering scheme to be used for the project's Releases.


## Decisions deferred

The following items are out of scope for this proposal, as they're either not integral to a Release Planning & Management plan, or are addressed by other (potentially upcoming) RFCs:

- Promotion/Marketing: This is a more holistic topic of who should drive promotion and marketing for the project. While Releases should certainly be part of this, the individual who takes on this role should drive the strategy behind communicating new and upcoming Releases to the community.


## Links and prior art

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

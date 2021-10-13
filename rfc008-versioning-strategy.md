# RFC008 - Release Versioning Strategy

## Proposed by

Aaron Peters

## Current status

- [x] Draft
- [ ] Under discussion (until YYYY-MM-DD)
- [ ] Final comment and voting (until YYYY-MM-DD)
- [ ] Accepted
- [ ] Rejected
- [ ] Implemented
- [ ] Deferred
- [ ] Withdrawn


## Proposal overview

As The Good Docs Project moves towards a formal release structure, this RFC proposes a standard versioning scheme to apply at least to the project's Product Outputs, as defined by outputs directly employed by users in their own documentation efforts. For example, this includes the collection of templates (which users copy as a starting point for their own documents), but not whitepapers (which serve to inform their audience, but are not used verbatim).

TGDP will use the Semantic Versioning convention for the versioning of individual Product Outputs (at the time of writing, this includes the template collection and the DocTools website package).

> :triangular_flag_on_post: For the purposes of this RFC, "features" and "functionality" can refer to new **content**, such as additional sections or boilerplate text, added to doc templates.


## Motivation

Using the well-established SemVer framework will provide the following benefits:

- It will demonstrate the project's progress to users and prospective users through publicly visible notifications.
- It will set expectations to current users regarding the extent of change(s) contained in a newly-release version of a Product Output, as compared to the version the user currently has, including potentially breaking backward-compatibility. 
- It provides contributors to the project a 
- It provides downstream integrators of TGDP's Product Outputs an easy way to identify if their own work products will need to be updated to support new features, or if there is a risk of compatibilty issues.


## Proposal

In the course of preparing for a Release from the project:

1. The PSC and Working Groups will decide on what functionality/features to target for it.
1. Working Groups will work towards these goals during regular working sessions.
1. Once the updates to a Product Output are **functionally complete**, meaning the initial implementation of new functionality has been completed, the Product Output can be tagged with a semantic target version number depending on changes introduced.
1. The first such tag within a Release cycle should also carry the "-alpha" suffix.
1. Further work during the release will focus on stabilizing the existing functionality and making it ready for general/production use.
1. Once the Product Output is deemed ready, it will be tagged with the same semantic version number and the "-beta" suffix.
1. At this point it should be released to a community of beta testers to actually use the Product Output. Feedback from this use should be actively solicited and captured.
1. Provided there are no "blocker"-level issues issues remaining with the Product Output as the Release's target date approaches, the Release Manager will coordinate the completion of any final updates before signaling for them to be tagged with the same semantic version number, minus any suffix (indicating a final release).
1. Once tagged, building and packaging the Product Outputs can commence.

{
This section may continue depending on the answer to the minor version support question below, as in this case we'll be releasing fix versions of the prior release in parallel with the development of the next release.
}


## Consequences




## Dependencies

This RFC should be considered together with RFC-006, which describes the high-level planning process to be used for the project's Releases.


## Links and prior art

- [Meeting notes from discussion on versioning](https://docs.google.com/document/d/1Oc3hNhJRrXsr-abEmUKAdamC5aKJydtldvpcSK_Hv_E/edit)


## Open questions

- Should we limit Product Outputs to one per Working Group? For example, the Community Docs Working Group would produce the "Template Collection," as opposed to considering each template as a separate Product Output?
  - In the context of this RFC, this means the collection as a whole would be versioned together.
  - A result of this would be that, as defined by the SemVer standard, **any** update to a template that adds materially to it (i.e. not fixing typos or other "bugs") would mean an increase in the minor version of the collection as a whole.
- How long will the project aim to support legacy major versions? Minor versions?


## Decisions deferred

The following items are out of scope for this proposal, as they're either not integral to a Release Planning & Management plan, or are addressed by other (potentially upcoming) RFCs:

- Promotion/Marketing: This is a more holistic topic of who should drive promotion and marketing for the project. While Releases should certainly be part of this, the individual who takes on this role should drive the strategy behind communicating new and upcoming Releases to the community.


## Feedback

{If you accept feedback from a community member, you will incorporate it into your RFC before it is accepted.
If you reject feedback, note that rejected feedback here before resolving the conversation.}


## Implementation checklist

If this proposal is accepted, the following tasks must be completed:

- [ ] Approve RFC006
- [ ] Decide on the appropriate version for existing Product Outputs
- [ ] Conduct Planning for the initial project Release as described in RFC006


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

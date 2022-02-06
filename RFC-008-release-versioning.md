# RFC008 - Release Versioning Strategy

## Proposed by

Aaron Peters


## Current status

See the status indicated on the pull request description.


## Proposal overview

As The Good Docs Project moves towards a formal release structure, this RFC proposes a standard versioning scheme to apply at least to the project's Product Outputs, as defined by outputs directly employed by users in their own documentation efforts. For example, this includes the collection of templates (which users copy as a starting point for their own documents), but not whitepapers (which serve to inform their audience, but are not used verbatim).

TGDP will use the Semantic Versioning convention for the versioning of individual Product Outputs (as at November 2021, this includes the template collection and the DocTools website package).

> :triangular_flag_on_post: For the purposes of this RFC, "features" and "functionality" can refer to new **content**, such as additional sections or boilerplate text, added to doc templates.


## Motivation

Using the well-established [Semantic Versioning](https://semver.org/) framework will provide the following benefits:

- It will demonstrate the project's progress to users and prospective users through publicly visible notifications.
- It will set expectations to current users regarding the extent of change(s) contained in a newly-release version of a Product Output, as compared to the version the user currently has, including potentially breaking backward-compatibility.
- It provides contributors to the project a common point of reference when collaborating, making the team more efficient.
- It provides downstream integrators of TGDP's Product Outputs an easy way to identify if their own work products will need to be updated to support new features, or if there is a risk of compatibility issues.


## Proposal

In the course of preparing for a Release from the project:

1. The PSC and Working Groups will decide on what functionality/features to target for it.
1. Working Groups will work towards these goals during regular working sessions.
1. Once the updates to a Product Output are **functionally complete**, meaning the initial implementation of new functionality has been completed, the Product Output can be tagged with a semantic target version number depending on changes introduced.
1. The first such tag within a Release cycle should also carry the "-alpha" suffix.
1. Further work during the release will focus on stabilizing the existing functionality and making it ready for general/production use.
1. Once the Product Output is deemed ready, it will be tagged with the same semantic version number and the "-beta" suffix.
1. At this point it should be released to a community of beta testers to actually use the Product Output. Feedback from this use should be actively solicited and captured.
1. Provided there are no "blocker"-level issues issues remaining with the Product Output as the Release's target date approaches, the Release Manager will coordinate the completion of any final updates before signaling for them to be tagged with the same semantic version number, minus any suffix (indicating a gamma/final release).
1. Once tagged, building and packaging the Product Outputs can commence.
2. Following the gamma release of an Output, "patch" releases may be released in parallel to updated versions, as described in the section Semantic versioning addendum for documents below.

## Semantic versioning addendum for documents

This document describes how MAJOR.MINOR.PATCH [*semantic versioning*](https://semver.org/) should be applied to documentation.


### Introduction

The [*semantic versioning specification*](https://semver.org/) (SemVer) is widely applied to describe software release versions, however these SemVer rules don't align well with the characteristics of documentation. This addendum suggests rules which can be applied when versioning documents.


### SemVerDoc rules

The following table adds documentation-specific interpretations of the [*semantic versioning*](https://semver.org/#semantic-versioning-specification-semver) rules. When applied to documentation, the SemVerDoc rules should take precedence over the equivalent software centric rules.


The remaining SemVer rules remain the same as their software equivalent.

<table>
<tbody>
<tr class="odd">
<td><strong><em>SemVer 2.0.0 specification extract</em></strong></td>
<td><strong>SemVerDoc addendum</strong></td>
</tr>
<tr class="even">
<td><a href="h%20ttps://semver.org/#spec-item-4"><em>4.</em></a><em> Major version zero (0.y.z) is for initial development. Anything MAY change at any time. The public API SHOULD NOT be considered stable.</em></td>
<td><p>4.1 For documents, major version zero (0.y.z) MAY be used for any of the following:</p>
<ol type="a">
<li><p>A document with incomplete content.</p></li>
<li><p>A document which hasn’t been fully reviewed.</p></li>
<li><p>A document which hasn’t reached applicable quality guidelines.</p></li>
</ol></td>
</tr>
<tr class="odd">
<td><a href="h%20ttps://semver.org/#spec-item-5"><em>5.</em></a><em> Version 1.0.0 defines the public API. The way in which the version number is incremented after this release is dependent on this public API and how it changes.</em></td>
<td><p>5.1 For documents, version 1.0 SHOULD designate the first officially complete version of the document.</p>
<p>This MAY be the first published or publicly released version.</p></td>
</tr>
<tr class="even">
<td><a href="h%20ttps://semver.org/#spec-item-6"><em>6.</em></a><em> Patch version Z (x.y.Z | x &gt; 0) MUST be incremented if only backwards compatible bug fixes are introduced. A bug fix is defined as an internal change that fixes incorrect behavior.</em></td>
<td><p>6.1 For documents, patch version Z (x.y.Z | x&gt; 0) SHOULD be incremented if updates are introduced which have minimal impact on the meaning of the text.</p>
<p>Examples include:</p>
<ol type="a">
<li><p>Correction of ambiguous text.</p></li>
<li><p>Spelling, grammar or formatting changes.</p></li>
<li><p>Sentence restructuring.</p></li>
<li><p>Additional clarification notes or cross references.</p></li>
<li><p>Addition of document metadata, such as <em>document_license:</em> or <em>document_author:</em>.</p></li>
</ol></td>
</tr>
<tr class="odd">
<td><a href="h%20ttps://semver.org/#spec-item-7"><em>7.</em></a><em> Minor version Y (x.Y.z | x &gt; 0) MUST be incremented if new, backwards compatible functionality is introduced to the public API. It MUST be incremented if any public API functionality is marked as deprecated. It MAY be incremented if substantial new functionality or improvements are introduced within the private code. It MAY include patch level changes. Patch version MUST be reset to 0 when minor version is incremented.</em></td>
<td><p>7.1 For documents, minor version Y (x.Y.z | x &gt; 0 ) SHOULD be incremented if a backwardly compatible update has been made to the documentation, which means that downstream dependent documents or products are not likely to require updating.</p>
<p>Examples include:</p>
<ol type="a">
<li><p>A new concept or feature is added.</p></li>
<li><p>A new section is added.</p></li>
<li><p>Documentation is updated to reflect a Minor update to an application.</p></li>
<li><p>Removal of document metadata, such as <em>document_license</em> or <em>document_author</em>.</p></li>
</ol></td>
</tr>
<tr class="even">
<td><a href="h%20ttps://semver.org/#spec-item-8"><em>8.</em></a><em> Major version X (X.y.z | X &gt; 0) MUST be incremented if any backwards incompatible changes are introduced to the public API. It MAY also include minor and patch level changes. Patch and minor versions MUST be reset to 0 when major version is incremented.</em></td>
<td><p>8.1 For documents, major version X (X.y.z | X &gt; 0) SHOULD be incremented if significant backwards incompatible changes are introduced to the document, which means that downstream dependent documents or products are likely to require updating.</p>
<p>8.1.1 The document update MAY also include minor and patch level changes.</p>
<p>8.1.2 Patch and minor versions MUST be reset to 0 when the major version is incremented.</p>
<p>Examples include:</p>
<ol type="a">
<li><p>Changed advice provided by a key concept within the document.</p></li>
<li><p>A restructure of a template document.</p></li>
<li><p>Documentation is updated to reflect a Major update to an application.</p></li>
<li><p>Changed metadata for the <em>document_license</em> to a more restrictive license.</p></li>
</ol></td>
</tr>
<tr class="odd">
<td></td>
<td><p>14. The semantic version SHOULD only be updated when the software or document is baselined or published.</p>
<p>The semantic version doesn’t need to be updated on every author commit during development.</p></td>
</tr>
</tbody>
</table>


### Applicability

Different documentation scenarios may apply the SemVerDoc rules differently.


### When to update the semantic version

The semantic version SHOULD only be updated when the software or document is baselined and shared. It doesn't need to be updated on every author commit during development.


### Auto-generated documentation from code

Some documentation is automatically generated from code comments, using tools such as javadoc. In such cases, documentation version numbers should match the code version numbers.


### Stand alone documents

Documents which logically should be tracked independently should follow the SemVerDoc standard, as stated.


### Documentation set

Often a set of documents are delivered as part of a milestone or release. In these cases, each document should maintain its own version
number, and then a separate version is assigned to all documents in aggregate.

This should be handled in a similar manner to a linux distribution. Linux distributions typically apply a time based milestone release, and each linux release includes multiple, independently versioned, software packages.


### Website

If a website, or a section of the website is versioned, then it should follow the same conventions as a documentation set.


### Further reading

-   [Semantic Versioning 2.0.0](https://semver.org/) specification for software.
    -   [Proposed doc addendum github bug](https://github.com/semver/semver/issues/792)
-   [Semantic Versioning for Documents and Meaningful Manual Version Control](https://semverdoc.org/) from Nils Tekampe.
-   [Semantic versioning for docs proposal](http://neelsmith.github.io/2015/12/15/semver/) from Neel Smith.
-   [Semantic Versioning and Structure for IETF Specifications](https://datatracker.ietf.org/doc/html/draft-claise-semver-02).
-   This addendum is intended to complement [The Good Docs Project's](https://thegooddocsproject.dev) [RFC 008 Release Versioning proposal](https://github.com/thegooddocsproject/request-for-comment/pull/17).
-   [Semantic Versioning and Structure for IETF Specifications, draft-claise-semver-02](https://datatracker.ietf.org/doc/html/draft-claise-semver-02).
-   [Open Geospatial Consortium's Policy Directive 18](https://portal.ogc.org/public_ogc/directives/directives.php) defines use of Major.Minor.Bug-fix versioning for spatial specifications and related documents.


## Consequences

This decision will dictate how Releases are communicated to both internal and external parties. Using the Semantic Versioning convention will be familiar to many of the project's most important audiences, namely open source projects (many of which use the same or similar numbering schemes) and technical writers of various levels of experience.


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

# Good Docs Project request for comment (RFC) proposal process

This repository hosts a record of project proposals that require a request for comment (RFC) from the community.
Any active member of the Good Docs Project can submit an RFC proposal for consideration to the community.

A RFC proposal is a proposal to change some aspect or element of The Good Docs Project, such as major changes to:

- Our community's governance or project management processes.
- The project's architecture, such as branching or release strategies.
- Legal or financial designations for the project, such as license changes.
- High-level technical features or toolchain changes.

In general, an RFC proposal is required when a change is substantial and impacts more than one system or other team members.
If you're not sure whether a change requires an RFC proposal or not, you are encouraged to initially float your idea within one of our community forums, then consolidate the idea within an RFC proposal.

After a period where the RFC proposal is open for community comment, the [project steering committee](https://thegooddocsproject.dev/who-we-are/) will vote whether to accept or reject the proposal.
General community members may also add their vote, but their votes will be treated as non-binding.


## Why do we use RFC proposals?

Many mature open source projects use request for comment (RFC) processes to help them make major decisions.

RFC processes have many benefits, including:

- Empowering community members to share their ideas for improving our project.
- Notifying individual contributors of potential impacting changes.
- Providing all community members a chance to collaborate on key decisions.
- Gathering feedback to improve proposals or reduce the risk from the decisions being made.
- Allowing our community to govern itself democratically without making any single individual a bottleneck or gatekeeper.


## Overview of the RFC proposal process

The RFC proposal process has these basic phases:

1. **Propose** - The proposer submits an RFC proposal and notifies the community.
2. **Discuss** - The community is invited to comment on the RFC proposal, typically for 2-4 weeks.
3. **Modify** - The proposer may choose to revise the original proposal based on community feedback.
4. **Final comment and vote** - After the proposal is modified, the community is invited to offer their final comments for 1-2 weeks. The [project steering committee](https://thegooddocsproject.dev/who-we-are/) and community members will vote to accept or reject the proposal during this period.
5. **Implement** - If accepted, the community is notified and the proposal is implemented.


### 1. Propose

In this phase, the proposer submits a request for comment (RFC) proposal and notifies the community.

To submit an RFC:

1. Fork and clone the `request-for-comments-rfc` repository to your local machine.

   If you are not yet comfortable using Git or GitHub, write your proposal in a Google Doc and ask a member of the [project steering committee](https://thegooddocsproject.dev/who-we-are/) to open the pull request on your behalf.

2. Copy the `rfc-template.md` file from the root directory of this repository.

3. Rename the copied file with a short name describing the RFC proposal, such as `release-branching.md`.

4. Fill in the required sections of the template with details about your proposal.

5. Open a pull request in the `request-for-comments-rfc` repository that includes your proposed file.

   Ensure that maintainers are allowed to make modifications to your pull request so that they can assign the RFC proposal a number. Do not submit more than one proposal per pull request.

6. Once the pull request is open, notify the community by posting a brief summary and link to your pull request in:

   - The `#proposals` Slack channel
   - The `#general` Slack channel
   - The [Good Docs groups.io mailing list](https://thegooddocsproject.groups.io/g/main/topics)
   - An email or Slack DM to the current [Good Docs Project chair](https://thegooddocsproject.dev/who-we-are/).

After submitting the pull request, a member of the project steering committee who is in charge of the RFC process will take over community reminders and notifications.


### 2. Discuss

The RFC proposal will be open for community discussion for 2-4 weeks after the community was notified.

During this time, anyone in the community may comment on the proposal by posting comments on the pull request thread.

The length of the open comment period will depend on comment activity.
If the community is actively commenting on the RFC proposal after 2 weeks, the commentary period will extend up to a maximum of 4 weeks to allow the discussion to continue.

When making comments, community members should be aware that:

- Our [decision process](https://thegooddocsproject.dev/decisions/) is based on the [rough consensus model](https://blog.doist.com/decision-making-flat-organization/) in which critical, blocking objections are given more consideration than minor, nit-picking objections.
- To that end, community members are encouraged to use the [Conventional Comments](https://conventionalcomments.org/) labels, especially if you consider your comment to be a blocking objection.
- Remember to follow our [Code of Conduct](https://thegooddocsproject.dev/code-of-conduct/) and ensure everyone feels safe to participate and express their ideas. Avoid making any personal insults when expressing disagreement.


### 3. Modify

During or after the general discussion period, the community member that originally submitted the RFC proposal may revise the proposal to incorporate feedback or suggestions from the community.

The proposer makes the final call whether to adopt or reject feedback:

- If they **adopt** the feedback, the proposer incorporates it into the RFC draft before the final comment period begins and notes it in a comment on the pull request threads and in their commits.
- If they **reject** it, they note it in the feedback section by copying the comments verbatim and stating their reason for rejecting the feedback.


### 4. Final comment and vote

Once the initial comment period has ended, the RFC proposal will enter the final comment status, which typically lasts 1-2 weeks.
During the final comment period, the members of the [project steering committee](https://thegooddocsproject.dev/who-we-are/) and community members may make any final comments and indicate their vote on the proposal:

| Vote   | Meaning                                                           |
| ------ | ----------------------------------------------------------------- |
| **+1** | In favor of the proposal                                          |
| **+0** | Mildly for, but mostly indifferent                                |
| **0**  | Indifferent                                                       |
| **-0** | Mildly against, but mostly indifferent                            |
| **-1** | Strongly against. This is expected to be accompanied by a reason. |

In order to be accepted, at least half of the current project steering committee members must vote in favor of the proposal.
Votes from general community members are non-binding, but will be taken into consideration.

Abstaining or absent votes from project steering committee members will be treated as indifferent votes.

Project steering committee members should indicate their vote by commenting on the pull request thread.
The proposer is responsible for recording how PSC members voted by updating their RFC prior to merging it into the repository.


### 5. Implement

If the RFC proposal is accepted, a member of the project steering committee will merge the proposal and add it to the `accepted` folder of the `request-for-comments-rfc` repository.

The proposal is then implemented in the project. If the proposal requires modifying any project documents or repositories, those actions should be taken shortly after the RFC proposal is accepted.


### Other RFC proposal outcomes

The proposer may choose to withdraw the proposal at any point during the process.
It is also possible that the RFC may be accepted, but the implementation may be deferred for a later date.


## Resources

In creating the RFC proposal process, the authors adapted or were inspired by the following resources, listed alphabetically:

- [Conventional Comments](https://conventionalcomments.org/)
- [GeoServer Improvement Proposals](https://docs.geoserver.org/latest/en/developer/policies/gsip.html)
- [No Kings: How Do You Make Good Decisions Efficiently in a Flat Organization?](https://blog.doist.com/decision-making-flat-organization/)
- [Salt Enhancement Proposals](https://github.com/saltstack/salt-enhancement-proposals)
- [Six lessons on using technical RFCs as a management tool](https://opensource.com/article/17/9/6-lessons-rfcs)

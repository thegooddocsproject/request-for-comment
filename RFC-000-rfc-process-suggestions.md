# RFC Zero - Open for suggestions to the RFC process

## Proposed by

[Alyssa Rock](https://thegooddocs.slack.com/team/U012KCMPP0V)

## Current status

- [x] Draft
- [x] Under discussion (until 2021-07-28)
- [x] Final comment and voting (until YYYY-MM-DD) {{Add date after selecting this status.}}
- [ ] Accepted
- [ ] Rejected
- [ ] Implemented
- [ ] Deferred
- [ ] Withdrawn


## Proposal overview

This RFC is open to suggestions from the community for minor and major suggestions to improve the RFC process.
To make your suggestion to the process, add a comment to the "Feedback" section of this file or to this PR.


## Motivation

We've completed the RFC process with at least one RFC now and we've learned a few lessons along the way.
Some members of the community expressed a desire to make a few minor tweaks and improvements and this RFC is designed to facilitate that discussion.


## Proposal

Based on suggestions from the community, the following suggestions to the RFC process will be implemented:

- **YAML front-matter text** - To make our RFCs machine-readable by static-site generators and our doc-tooling system, we'll include some YAML front matter to track various elements of the RFC. Morgan will implement this functionality.
- **Status updates** Rather than track the status inside the RFC itself, we will track it in the PR description or in the YAML front matter.
- **New sections** - We'll add the following sections to the template:
  - Open Questions
  - Decisions Deferred
  - Consequences
- **Feedback** - The proposer makes the final call whether to adopt or reject feedback. If they adopt the feedback, they incorporate it into the RFC before the final comment period begins. If they reject it, they note it in the feedback section.
- **Voting** - We will put responsibility on the RFC proposer to record how PSC members voted in the actual RFC. PSC members can also open a pull against the file to indicate their votes.
- **Rename heading** - We'll rename the "Links" heading to "Links and prior art."
- **Statuses** - We might possibly need to add some additional statuses to the RFC to allow for revision periods and second comment periods. I also wonder if we need some statuses for "on hold" or "blocked by" or something. For example, the Procope proposal is currently blocked by another RFC. How do we represent that?


## Links

No links necessary!

## Feedback

Suggestions:

- Morgan writes: Are we expecting folks to update their own vote, or the rfc author updates their markdown with all the votes? I have some ideas around how this might get automated. I love the idea the votes would go in here inside of the markdown so it gets immortalized with the document. But it is lots of extra work for the RFC author.
- Alyssa commented tn this Links section under feedback: As I look at this section of the template, I find that our process is a little unclear about how to handle feedback:
  - Is the proposer the person who makes the final call on whether to adopt or reject feedback? If so, do they resolve the conversation?
  - If they adopt it, do they just incorporate it into their draft and provide attribution for the idea?
  - If they reject it, do they note that in the feedback?
  - At what stage do they do it they need to resolve the conversations and adopt/reject the feedback?
- In reply to the previous conversation, Morgan writes: yeah interesting points, I think it can be valuable to capture feedback that is meaningful and to re-incorporate back into the RFC especially if it belongs to another sections. For instance, I mentioned above Open Questions those usually get added as I get comments on the RFC so I update that section with the questions being asked. And then work to update the main proposal sections as I answer those questions. As for the Feedback section -- I do think this could be helpful to have if there are conversations that we want to capture that didn't fit into any of the other sections.
- Morgan writes: I'm a 100% fan of the checklist, torn on where I like it. I think it is perfect in the pull-request description so that it can be easily checked/actioned by folks(github-members). And we keep track of the status as a field inside of the YAML when applicable. Open to discuss.
- In response to the previous conversation, Alyssa writes: I agree that it should be either a field inside YAML or included in the description for the pull request.
- In the Proposal overview section, Morgan writes: For Proposal Overview, not sure what the default text is here. Recommend we have a suggestion to keep it short.
- In the Motivation section, Morgan writes: I like motivation to capture the context or the why of the proposal.
- In the Links section, Morgan writes: I've called mine 'Prior Art' in the past, but Links communicates the same.
- Morgan writes: Section Proposal Potentials - These are sections I've used in other RFC processes I found helpful:
  - Open Questions
  - Decisions Deferred
  - Consequences
- In the Implementation checklist section, Morgan writes: Not sure how useful this is here, and think it might fit better into the PR description as a checklist. Probably an RFC to write a PR_TEMPLATE.
- Morgan writes: Add in a sample yaml block for front-matter, and we set some default values. I think a discussion around what fields we have here could be a followup. I'd propose we start with proposalDate and status. Happy to add more now, but we could keep it simple for now. Example:

---
proposalDate: <yyyy-mm-dd>
status: <proposal|accepted> _we could add more versions_
---
By adding the above yaml, it allows the RFC to be machine-readable by static-site generators and our doc-tooling.


## Implemention checklist

If this proposal is accepted, the following tasks must be completed:

- [ ] Make indicated changes to the RFC template and README
- [ ] Follow up with Morgan about YAML front-matter automation


## Votes

Votes as per our [decision process](https://thegooddocsproject.dev/decisions/}:

Project steering committee (listed alphabetically by first name):

- Aaron Peters: 
- Aidan Doherty: +1
- Alyssa Rock: +1
- Ankita Tripathi:
- Bryan Klein: +1
- Cameron Shorter: +1
- Carrie Crowe:
- Erin McKean: +1
- Morgan Craft: +1
- Ryan Macklin:
- Viraji Ogodapola:

Community members who voted (non-binding):

- {{Your name}}: {{Your vote}}

# Migrate Good Docs Project Git repositories to GitLab

## Proposed by

Alyssa Rock - https://thegooddocs.slack.com/team/U012KCMPP0V

Co-sponsored by:

- Bryan Klein
- Deanna Thompson

## Current status

See the status indicated on the pull request description.


## Proposal overview

The Good Docs Project should migrate its Git repositories from GitHub to GitLab.
Although the migration would involve some initial disruption to our community's workflow, the many advantages that GitLab offers would make the move worth it in the end.


## Motivation

Migrating our project to GitLab would involve many significant advantages, as explained in the following sections.

### Ease of use and improved review workflows

GitLab has [feature parity](https://about.gitlab.com/devops-tools/github-vs-gitlab/) with many of GitHub's features but it's much easier to do merge request (pull request) reviews of text documents in GitLab, which will improve and streamline our template review process. 

It is currently quite difficult to review template PRs in GitHub. The reviewer often needs to look at and switch between various points of the document during a review. Scrolling is tiresome, and opening multiple browser tabs to view the same document, or to view multiple files in the same PR, is cumbersome.

By contrast, GitLab gives the ability to use a file explorer view and see changes across multiple files, which reduces the complexity of reviewing text-based documents.
GitLab allows you to toggle between seeing all of the changed files vs. one file at a time makes the review process significantly easier.

Another nice GitLab review feature is the ability to turn a comment on a merge request into an issue if you like the suggestion, but won't immediately implement it.
[GitLab flavored Markdown](https://docs.gitlab.com/ee/user/markdown.html) also has some additional features such as the ability to add a built-in table of contents, front matter, and graphs.

Various members of our community have been working in GitLab for some time, and find it significantly easier to use than GitHub when working with text documents.


### Improved project management tools

GitLab provides us with a lot of the project management tools that were proposed in [RFC-001](https://github.com/thegooddocsproject/request-for-comment/blob/main/Accepted-RFCs/RFC-001-zenhub.md) out of the box without requiring additional integrations.

GitLab provides the ability to view all the issues for the entire project all at once or to view all the issues for one repository or working group.
It also has sophisticated [kanban board features](https://docs.gitlab.com/ee/user/project/issue_board.html#multiple-issue-boards).
In GitLab, you can create custom kanban boards that display issues with certain labels or other filters as needed.


### Project history can be retained

It is definitely possible to migrate repositories in ways that retain project history.
Alyssa has participated in various GitHub to GitLab migrations where all the issues, comments, and past information on pull requests have been retained.
The only loss of data is that sometimes it shows the person who migrated the repository as the person who opened a issue or pull request, but it indicates in a comment the GitHub handle of the person who originally opened the issue or pull request.

Be aware that one disruption to our community is that repositories can't have any open pull requests at the time of the migration.
That means we would have to merge in or close any open pull requests and implement a pull request freeze during the migration.


### Additional benefits

In addition to these main benefits, several members of our project also have stronger professional network connections to the GitLab organization than we do to GitHub.
For example, Alyssa has a good working relationship with GitLab's lead tech writing manager and Bryan knows prominent members of their engineering team.
Down the road (i.e. 5 years or so), we could consider leveraging these connections to integrate our templates and tools into GitLab's offerings for new open source projects, which would significantly increase our project's visibility and ability to fulfill our project's overall mission.

It's also worth noting that GitLab is an actual open source project.
GitHub, although free to use for open source, is a closed source project.


## Proposal

To migrate our repositories to GitLab, we would need to:

1. Form an ad-hoc working group of about 3-5 community members that will work on the migration.
2. Research how to do the migration. See [Import your GitHub repository into GitLab](https://docs.gitlab.com/ee/user/project/import/github.html) for more information.
3. Develop a plan for migrating the repositories in a way that will minimize project disruptions. This plan could also include a communication strategy for notifying our community of this change, training them on differences between the two platforms, creating GitLab accounts, creating new project forks, etc..
4. Implement the plan and check that the migration was successful.
5. Temporarily hide the Good Docs Project repositories on GitHub so that they are still accessible to project owners.
6. After about a year's time, delete the Good Docs Project repository from GitHub.


## Consequences

See the positive benefits listed in the **Motivation** section.

We fully acknowledge that this migration will cause some delays and disruption to our community during the migration process.
Hopefully the migration working group can develop a plan that will minimize these disruptions.


## Links and prior art

- [GitLab vs. GitHub](https://about.gitlab.com/devops-tools/github-vs-gitlab/)
- [GitLab-flavored Markdown](https://docs.gitlab.com/ee/user/markdown.html)
- [GitLab agile delivery project management](https://about.gitlab.com/solutions/agile-delivery/)
- [GitLab kanban boards](https://docs.gitlab.com/ee/user/project/issue_board.html#multiple-issue-boards)


## Open questions

{This section is optional and is where you can list questions that won't be resolved by this RFC, including those raised in comments from community members.}


## Decisions deferred

{This section is option and is where you can list decisions that won't be resolved by this RFC, but which should be raised at a later time.}


## Feedback

{If you accept feedback from a community member, you will incorporate it into your RFC before it is accepted.
If you reject feedback, note that rejected feedback here before resolving the conversation.}


## Implementation checklist

See **Proposal** section.


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

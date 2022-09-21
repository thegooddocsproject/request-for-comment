# RFC-011: News & announcements on site

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

We could use a place on our site where we announce news about the project as warranted. This has been talked about a bit over the last year, as part of blog conversations, then social media conversations, and some content strategy conversations. So here's a RFC that's about how we can approach it.

## Motivation

We could use a place where we host announcements about the project. For instance, we want to get more people from EMEA into our Community Docs working group. There was a comment about announcing that on Twitter. It would be great if there was a link to a page on the site about it—one that is temporally relevant about this initiative, beyond just linking to a general working group page.

## Organizational dependency: Content Strategy

This is ultimately intertwined with Content Strategy (and related social media efforts), and needs to be intentionally a part of that. Thus, at the time of drafting this RFC, it's a placeholder that needs the Content Strategy team to vet and determine various elements before it fully goes to the PSC for debate and approval.

## Proposal

We have a place on the site, such as thegooddocsproject.dev/news, that holds our news posts. We'd use a format *similar to* but not the same as the blog—similar because unified branding is important, but not the same so as to differentiate the content appearance.

[That gets into defining what our unified visual branding *is*. Which is a conversation beyond the scope of this RFC.] 

We'd use the same system for publishing news posts as blog posts: pushing a markdown file to a folder, and the Hugo site handling the rendering of changes.

### Types of content

The news site would handle two types of content: announcements and heartbeats.

Announcements are straightforward: they're announcements from our community to the wider interested-in-documentation community (whether other tech writers, developers interested in docs, or whoever else subscribes to us). This could be calls to action (such as recruitment or activity drive), or community celebration (such as talking up a GDP member speaking elsewhere).

Heartbeats are periodic posts where we talk about the states of different working groups, as relevant to our wider audience of users or prospective contributors. These would be ideally no more than every two or three months, and drafted from a perspective of PR to keep showing in between release cycles that we're passionate about our work.

Heartbeats could also possibly showcase an individual contributor, like a "meet the team" sort of vibe. This has been declined as a blog post topic, as that doesn't fit the purpose of the blog, but it could fit here at the tail end of heartbeat posts.

(That also gives those individual contributors featured a different sort of call to action on publicizing their related post, as friends/colleagues of that contributor may be interest in the post for relationship reasons, then find the other content or project in general interesting enough to follow on its own.)

#### What this isn't

This wouldn't be a place for internal communications, meeting notes, etc. 

This also wouldn't be a "second blog" or similar.

### Why not use the blog?

The blog is about "docs advocacy & education," so if people subscribe to the blog/look out for new posts, they should expect material that's education, not that's purely about our group marketing.

The other elements of the blog, like its particular formatting/visual branding, focus on author, everything about CC licensing, etc. do not and should not apply to this content bucket.

### Specifics

The main page should show the most recent post, so when one clicks on "News" in the header, they don't have to click on a second link to see what's the most recent.

The sidebar would have the most recent 5 or so posts, with a "see all" that would just show a list with short versions, akin to what is seen in the [Write the Docs newsletter archive page](https://www.writethedocs.org/blog/archive/tag/newsletter/).

The posts should be short: 500 words or so. Something that would take on average less than 5 minutes to read. We may deviate from this as needed, but the core concept is that our newsletters shouldn't take significant resources to craft and review, and we shouldn't demand significant time expenses from our audience in this manner.

It should allow for links, embedded media, etc. We might not make much use of that, but given things like opportunities to promote talks and releases, let's make sure we don't design ourselves into a corner.

Unlike how we handle the blog, authors wouldn't link to "about the author" pages as we do in the blog—and in fact we may decide there are no listed individual authors, to keep the news to appear to always be from the community.

Unlike how we handle the blog, there wouldn't be any commenting feature. 

Unlike how we handle the blog, there wouldn't be any banner or hero images.

### Slugs & timeliness

Because news is timely, the individual post URLs would use some date component rather than just a title.
Ideally we don't want more than one news post a day, but the potential need for crisis managament comms (such as a public apology, an emergency rollback, etc). means we should support multiple posts per day. With a content policy of "only for crisis management."

It's better to support and never need than kick ourselves for not having it, right? As long as it doesn't turn into overengineering. (I'm okay to engineer for contingencies we need to support as the org grows, as long as they're reasonable to consider, and it's less costly to implement them now than later.)

Per Aaron: "There's probably other valid reasons for multiple posts per day, e.g. what we're doing/have done during WTD conferences. I'd argue that just appending a "-2" or similar would be sufficient, but using a timestamp works too."


### Why not use the blog?

Two reasons:  First, it would split the purpose and publishing resources of the blog. The blog's purpose is supporting docs advocacy and education.

Second, while the framework might be similar, it isn't exactly the same. So we can reuse a lot of the work on the blog, but it has different content needs.


### "Creating" the News Team

The team that would handle this would be the "News team," and essentially be our PR team. But functionally, that doesn't end up being a new team, as we already have a de facto PR team between those who run our social media (namely Felicity and Carrie), people planning Content Strategy, and the co-chairs.

This team would just be a formalization of who vets news posts before going on, to make sure news is on message. The ideal people for this are journalism and communication studies nerds. We happen to already be well stocked in that regard. :)

### Forward facing: emailing newsletters

If we want to get to a point of having a mailing list to keep our users informed, this is the content we'd use. And by having two categories, people could opt into different types of content. However, that isn't a requirement to execute on this idea.

## Consequences

This allows us a space to write about upcoming changes for users to experiment with (such as if we start playing in the space of having "dev branches"), announcements for recruiting, celebrating our contributors' efforts elsewhere (like announcing them being Write the Docs speakers), and upcoming meetups (like holding writing days at Write the Docs).

This would be an additional effort set for the Tech Team, to take the blog and tweak it for another subfolder. That might involve refactoring material to be shared, or not—details on the code execution part of this effort is beyond the scope of the RFC, barring noting any concerns, issues, or plans that the Tech Team might share upon reviewing this.

This could also play into future endeavors as we potentially expand, such as announcing Good Docs-hosted talks (which are themselves ways of passive recruiting).

And this would be some additional ongoing effort on the part of the News team, though the effort should be light, and the payoff for that effort well worth it.

## Links and prior art

[How Write the Docs does their newsletters](https://www.writethedocs.org/blog/archive/tag/newsletter/), which as an index page feels like it works as email-delivered newsletters first, site-formatted news second.

## Open questions

{This section is optional and is where you can list questions that won't be resolved by this RFC, including those raised in comments from community members.}


## Decisions deferred

* Good ideas that don't need to be implemented as v1:
  * Atom/RSS implementation
  * Social media share buttons
* Ideas that are non-trivial to consider, and should be punted until the news efforts have found footing:
  * Future news efforts (like mailing lists)
  * Tying news posts to automated social media posts

## Feedback

### Miscellaneous feedback on execution

This feedback is recorded for implementation purposes, but doesn't affect the RFC at this higher-view intent:

- Bryan: "This could also all be stored in a structured JSON data file, with a nice little editor for each entry in the file."
- Bryan: "I'm thinking of something small like twitter cards for the layout."
- Bryan (re newsletter): "It would be easy to create a 'filtered' set of posts from this data/file set for automated collection of updates in a newsletter."
- Bryan: "There are some built in Hugo shortcodes that could come in handy here. https://gohugo.io/content-management/shortcodes/#use-hugos-built-in-shortcodes"

## Organizational dependencies

* Content strategy in involved in such decisions & nuance
* The tech team would be involved in implementation

## Implementation checklist

If this proposal is accepted, the following tasks must be completed:

- [ ] Governance list
  - [ ] Create issues
  - [ ] Sketch timeline
- [ ] Organization list
  - [ ] News team composition
  - [ ] Naming conventions/content strategy (including "is 'news' the right header for this?")
  - [ ] Document process for posting
  - [ ] Content moderation policies
  - [ ] Document the subsite's purpose and content guidelines
- [ ] Technical list
  - [ ] Layout design
  - [ ] Code execution (beyond anything the Tech Team wishes included in this proposal, as notes or requirements)
  - [ ] Set up the site infrastruction


## Votes

Votes as per our [decision process](https://thegooddocsproject.dev/decisions/):

Project steering committee (listed alphabetically by first name):

- Aaron Peters:
- Alyssa Rock:
- Ankita Tripathi:
- Bryan Klein: +1
- Cameron Shorter:
- Carrie Crowe:
- Erin McKean:
- Deanna Thompson:
- Felicity Brand:
- Gayathri Krishnaswamy: +1
- Morgan Craft:
- Nelson Guya:
- Ryan Macklin: +1
- Tina Lüdtke: +1


Community members who voted (non-binding):

- {Your name}: {Your vote}
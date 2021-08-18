# RFC004 - Revising website licenses terms/page

## Proposed by

Ryan Macklin ([@macklin](https://thegooddocs.slack.com/team/U01DYRWG43X))
Initially submitted on 2021-07-13

## Current status

- [ ] Draft
- [x] Under discussion (until 2021-08-11, assuming 2-4 weeks post initial submission)
- [ ] Final comment and voting (until YYYY-MM-DD) {{Add date after selecting this status.}}
- [ ] Accepted
- [ ] Rejected
- [ ] Implemented
- [ ] Deferred
- [ ] Withdrawn

## Proposal overview

I believe we should rethink the licensing terms for website content, as listed on [thegooddocsproject.dev/licenses/](https://thegooddocsproject.dev/licenses/). As they're currently written, they provision everything as [Creative Commons Attribution 4.0](https://creativecommons.org/licenses/by/4.0/) (a.ka. "CC BY 4.0), including all text, images, HTML code, and anything else.

We may not always have the rights to relicense what we put on our page, and not every contributor is comfortable with having their info and likeness released as publicly usable.

### Scope

The scope of this is about the website's content. Licensing for our products (templates, doc tools, etc.) aren't part of this discussion, though this proposal does indicate where the primary home for those licenses should be.

## Motivation

For the upcoming blog, not everything we release will be ours. If we use stock photos for the purposes of social media optimization, we won't have the rights to relicense that content. We also may not have the rights to relicense other content we'll reuse, including any HTML/CSS/scripting to generate the pages.

On a personal level, I don't release my likeness to public use, and the current website license terms makes me wary of continuing with the project. I used to work in games (and still do at times), and I've had too many death threats (honestly, one such threat is too many) and have seen too many friends be impersonated to want to give bad actions a contractual right to use my likeness however they like. (Bad actors will still use likenesses, but at least they can't defend their actions by citing a license that allows them to use one's info.)

### Blocking

[RFC002 (Procope/blog & video)](https://github.com/thegooddocsproject/request-for-comment/pull/3) is blocked by this proposal.

## Proposal

I'd like to shift the burden of licensing to the individual elements, rather than have a pure blanket. That means:

- Our products (templates, doc tools, etc) have the BSD0 license in their readme or license text files, and not rely on the license website page for that notice. This concept covers all **replicated content**—anything we build that's meant to be copied, redistribted, and modified as part of execution.
- For cognitive content-based subprojects (example: blog posts), individual pages/items with licensing requirements would default to have something like "`This piece's original text is (c) [year] [author name], and licensed under CC BY 4.0`". Currently, the blog is set up to allow for this default, with other changes allowed. Ryan and Bryan worked together to make sure this could be modular.
- **Cognitive content** is content meant for people to read, internalize, and add to their sense of knowledge and practices without necessarily being about copying and republishing. Blog posts, white papers, videos, podcasts, posters, diagrams, all of that is "human content." Execution for this is about shaping thought patterns and discourse.
- For the above example: "Original text" covers not opening any quoted text (like in referencing a book's text) as being CC, and doesn't open any stock images from being CC. If a custom image is created by the author, we can add that to the CC license, which is part of why Ryan and Bryan worked to make the license field in the blog subproject modular.
- For everything else on the website, we leave the material either unlicensed, under whatever licenses already exist for that material, or make some other decision as part as a subproject's RFC. Thus, our default state is to not specify a license. (See What's currently CC BY content below.) It's better to not specific a license initally and add one later, than it is to specify the *wrong* license or inccorect details at any point.

Since the licenses page wouldn't be the declaration of broad license anymore, it would become the page that explains what licences are used: BSD0 for our products, CC BY for "various pages" on the site. The licenses page wouldn't be the *primary authority* for this information, but instead a *single page to set expectations* for contributors and consumers regarding using elements of this project.

*Individual project's RFCs would define what sort of license scheme it has: BSD0 for replicated content, CC BY, or none. And it would include how/where it would include licensing info. This RFC is just about building that framework and disambiguating this issue.*

### Keeping it simple

Cameron mentioned wanting to keep this scheme simple. Here's how we keep to minimal labor:

- There are defaults, and we assume them. I've proposed those defaults above.
- For the generated content (like blog posts), the generator adds the license text. No need to sweat it.
- For products, they should already have licenses as part of the pages, because once downloaded or forked the license needs to be attached rather than disconnected on an external site
- Having the license attached to the website content means readers see the license alongside the text, and don't have to wonder or ask or hunt around for licensing info

### Some clarity

Note that you can specify with CC BY what content is covered under the license. It isn't inherent to the license that everything in a work is covered. You always say what's covered, whether it's "`This work is licensed under…`" or "`The text of this book is licensed under…`" or "`The text of chapters 1 to 6 are licensed under…`" or "`All text aside from that appearing on pages 66-67 are licensed under…`". (All instances I've used/seen used in games.)

To illustrate this point, here's text from the Creative Commons site's footer: `Except where otherwise noted, content on this site is licensed under a Creative Commons Attribution 4.0 International license.`

### We can't un-CC existing content

Part of the CC licenses is that we can't revoke the license or otherwise release something under a more restrictive license. Per the human-readable page, "The licensor cannot revoke these freedoms as long as you follow the license terms."

By changing the licenses page, we aren't "undoing" any license terms for the content at the moment. What we're doing instead is saying all changes going forward on the site are under the new terms (including not released at all in some cases).

If someone goes to a version of the site with the current license page (via github, archive.org, etc.), all of that material is still CC BY 4.0. We don't need to spell this out on the license page, but if someone inquires that's the answer.

## Open questions

* Is there an license that content files inherent by virtue of being in our repo? (Such as markdown files for the blog.) If so, this may pose a problem for us that we'll either need to account for or resolve.

## Links

* [Creative Commons Attribution 4.0](https://creativecommons.org/licenses/by/4.0/)
* [Good Docs Project licenses page](https://thegooddocsproject.dev/licenses/)
* [Current RFC002 file, with prior discussions about licenses](https://github.com/thegooddocsproject/request-for-comment/pull/3)

## Feedback
Bryan Klein:
- I suggest that we increase the specificity of the license terms in the LICENSE.md file and on the License page of the website.  Where we identify folders within the project that the content and byproducts of which the build process creates as `CC BY 4.0` and all other files in the repository are Apache 2.0 unless otherwise specified in the source file.  We can identify any number of files and folders as needed.  For example: `/content`, `/data', `/static/images`, etc.
    - {{Community member name}}: {{Additional comment on same topic.}}
    - {{Proposer name}}: {{Addressed by ... / Ignored because ... / ...}}
    
{{Reviewer name}}:
- {{I suggest that ...}}
    - {{Community member name}}: {{Additional comment on same topic.}}
    - {{Proposer name}}: {{Addressed by ... / Ignored because ... / ...}}

## Implementation checklist

If this proposal is accepted, the following tasks must be completed:

- [ ] Revise license page on website
- [ ] Have documented our license info, procedures, assumptions, whatever we need to have documented as an org to make all of this known to all contributors
- [ ] Merge and deploy license page revisions
- [ ] Ensure any relevant site pages or documents has their license terms in them, and not relying on the site's license page
- [ ] Define and address site repos' stucture needs and code/internal licencing needs based on content licensing

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






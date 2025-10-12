---
{"dg-publish":true,"permalink":"/idk/trees/doc-revision-struggles/","created":"2024-12-14T14:00:20.942-05:00","updated":"2025-04-10T23:20:45.409-04:00"}
---

#path/lessons-learned #notes/writing #notes/process
# Struggles of revising and rewriting
When I began to rewrite one of our major platform/process guides in July 2022, it was such an exciting event for me that I took notes on what I learned. There was a lot to unpack and decompress about what I found and it was extremely helpful to identify gaps in documentation training – how to approach additions, styling and formatting, etc.

## Context: Guide Versions

V1: The first version of this master guide was written almost entirely by one person (not me) as a discovery and troubleshooting document containing all of the information the team had learned about it up to that point. Issues:

- Though the process was explained thoroughly, it lacked some of the more technical context required for troubleshooting new issues.
- Lots of information was still locked inside the brains of those who had been doing the work for a while – an outline was created and filled out, but completeness wasn’t a concern at the time.

This version of the guide stayed with our team for about 5 years, but required rewrite due to major updates to the process and application.

> [!Review in more detail]
> [[idk/x archive/Master Guide Approach\|Master Guide Approach]]
> 
> [[idk/x archive/Master Guide Revision Steps\|Master Guide Revision Steps]]

V2: As a project and writing upskilling exercise, the second version of the guide was written by four team members who didn’t normally write. They were tasked to review V1, keep what was not changing, add content about the updates, and then fill in any gaps in knowledge by interviewing senior support team members or developers. They got to define most of the structure in how they worked with each other, and were provided with guide requirements laid out clearly. This assignment was the first where I played role of the documentation mentor, rather than the author-SME-editor.

**This post goes over some of the issues that were identified for improvement during editing for V3.**

V3: I began the rewrite/revision to match the structure and formatting of the rest of the team’s guides, including filling in gaps in content and fixing the issues noted below.

## Issues from Version 2

When the V2 crew came together, their approach was to divide the guide in half – product vs process – and work in teams of two to fill out the outline. **At the end they had created a version of the guide that was somewhat comprehensive in content, but with a few major issues.**

Unfortunately, budget for time and resources was thin so most of these issues stuck around until I was able to prioritize my review 4 years later. (This is one of the pitfalls of volunteering to manage documentation as part of your job: it’s always at the bottom of the priority list.)

**Writing process**

- They left out an entire process that we still do – they thought that the new application got rid of that. **They didn’t ask to confirm before making the decision to remove this process content.** (Once we discovered this was left out, it was prioritized to fix/readd.)
- It was clear the product writing team did not communicate with the process writing team, and **it also seemed evident that all four writers worked independently**.
- Based on the inconsistencies (and questions we asked after), **they didn’t leave time for editing before the guide due date**.

**Guide content**

- There was **little coherence/consistency across product or process**, or even within sections that were presumably written by the same author. Most of the consistency was copy/pasted from the previous version of the guide.
- They didn’t consider who was going to use the content – or that anyone was going to. Sometimes the instructions made no sense. **They didn’t test the steps**. A strong emphasis on getting instructions down on paper – not much emphasis on organizing it in a way that makes sense/flows, and almost no emphasis on communicating it clearly.
- It seemed some content was copy/pasted from another source using different fonts/styles, so it was **hard to follow**.
- Some **information was inaccurate or incomplete**.
- Lots of repeated info (rather than referencing other sections of the guide). **Repeated content used different terms** (and sometimes incorrect terms) than the first time you saw that info within that guide.

**Images and examples**

- **Every step had a screenshot**, even if the screen doesn’t change from one to the next.
- Screenshots are emphasized all over the place and in different ways which makes it **difficult to figure out what to look at or why**.

## Accountability

I know my part in these issues. When putting together this exercise, their manager and I might have given clearer expectations. We wanted them to feel flexible to get creative and execute the project in whatever way made sense for them as a team, so we weren’t strict on how they might do so. All of them had led assignments and projects in the past, but none had to do a self-directed project like this one before.

Some of the guide content and image issues were likely my fault for not giving enough up-front knowledge in the style guide, but the main gap that became obvious very quickly was the lack of a review/edit. It was a lesson learned for everyone and luckily we had time to help them correct the major errors and learn from the process before anyone was expected to use the guide.

This experience helped me truly understand how much I knew about writing from my history with writing, and I also had to admit I was assuming everyone had the same level of knowledge.

Getting honest feedback from the team on this project overall was a game changer for me. **It never occurred to me that other people hated writing.** I can understand “not enjoying it” but _hating_ it was so foreign to me. Writing brings me so much joy! I shed all of my imposter syndrome after this project and grew an appreciation for the non-writers on my team, since they have to constantly write stuff (docs or otherwise).

This discovery was an invigorating moment in my career path knowing that writing is something I could easily do every day for the rest of my life, and in doing so I’d contribute unique value because everyone else dislikes it!

## Lessons Learned

I doubt we’d do a project like this again, but if we did I’d change the following:

- **Provide structure for the project that has flexibility and room for creativity within it.** Example: Give guidance for general project tracking and status updates, using internal tools, etc., but leave stuff like “how and what to communicate” up in the air. That way they can be creative within some boundaries, rather than learning and innovating at the same time. (This was a project given among a high level of other work, so we can relieve them of some of the “thinking” involved while still encouraging new ideas.)
- **Clearer roles/responsibilities within the project**, especially as compared to day-to-day work. At the time my role in docs was not very well defined, but going forward I’d want to make the delineation clear since that caused some confusion for a while: a few team members thought my role on the project was my role going forward and that they’d be writing all guides. Imagine the panic!
- **Provide project-specific documentation guidance**, not just the general stuff available for all guide maintenance. This was a different kind of update than simply adding a section or updating content in an existing guide which is what this team was used to doing. This might also include resources on the documentation standards/styles and a glossary so terminology and descriptions would remain consistent.
- **Provide documentation workflow guidance so they know what to plan for when they determine their deadlines.** This would ensure they’d leave time for editing (and also know up front that they need to edit). This may look something like: Draft, Review/Update for Accuracy, Test/Update for UX, SME Review, Edit, Publish. How many non-writers think to test and verify the steps, or update for the experience of the person using the guide? This sort of guidance will keep them mindful of the full document lifecycle.
- **Provide escalation path for removing content**, e.g., whole sections/processes. Even with regularly scheduled doc updates they should be having that kind of stuff reviewed and approved, but maybe it wasn’t clear that we’d follow the usual processes in this project.

_Note: Though this post was written to log gaps I identified in our docs, and provide an idea of the kind of guidance non-writers need when contributing to docs… it does sort of focus on the negative a bit. I’ll add that the writing team did initially create a pretty comprehensive outline and even though the guide lacked consistent communication overall, it also wasn’t consistently bad! If they had edited, many of these issues would have been caught and dealt with before I even saw the doc._

---
Created: 11/6/23
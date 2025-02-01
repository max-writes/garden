---
{"dg-publish":true,"permalink":"/garden/trees/master-guide-revision-steps/","created":"2024-12-14T13:59:14.763-05:00","updated":"2025-01-31T23:07:02.921-05:00"}
---


#topic/writing #topic/process #max/lessons-learned 

# Master Guide Revision Steps 

Imagine you’re working on a support team of 6 people, all with various knowledge about the products you’re supporting. Some are more technical than others. Half were in the job already for three years, the other half just joined. There is some documentation but that’s not the focus of anyone’s job. Most processes are not documented; everyone holds them in their heads.

Without good guidance, a team like this may never write documentation despite having access to Google Drive or Microsoft Office.

In this scenario, one of the team members is a natural-born writer. They’ve been writing stories since they were a child and wrote user guides (for fun) in their free time as a _teenager_. Naturally, this person is going to write guides. They may share the desire with other teammates, and then eventually, they’ll get other team members to start writing down what they learn too.

This scenario is the history of documentation at my current job. Between 2013 and 2018, we created about 300 separate guides to remember and reference as our document library grew exponentially over the team’s first 5 years.

This was frustrating. In 2018, the team requested a single document they could Ctrl+F to find what they needed. **This post is a review/reflection of the “master” guide strategy I kept in a previous position which documented all content related to a platform in one guide, including my lessons learned from the approach.**

## What’s a Master Guide?

**The “platform master” guides include all instructions and information related to each platform the operations team supports**. At the time of writing this article (Nov 2023), there were 4 total master guides and, as you might imagine by the description, they were very long (between 115 and 150 pages).

They were by necessity long. **The master guide is meant to be a one-stop shop for that platform, including all guidance related to process, configuration, expected behavior and background, how-to, scope, support, and troubleshooting.** If it does not include the instructions you needed, it links to them instead.

These guides had their own problems – they’re huge, took forever to load, and if you weren’t on the team when they were written then there’s a heavy learning curve to navigating and finding information. I wanted to write about my experience with editing and maintaining a guide of this nature and length.

> [!Review in more detail]
> [[garden/trees/Master-Guide-approach\|Master-Guide-approach]]


## Editing the Master Guides

Editing the master guides was a huge process, especially as the team’s solo writer. **A full revision took about 3-5 months.** Minor edits were easy to implement as processes changed and we documented new ticket scenarios, but eventually it would get messy and be hard to follow after multiple contributors added their different voices to the guide, with various levels of writing experience.

One issue (later resolved) – we didn’t have a documentation process that required SME review. No one was officially “in charge” – I was writing these guides in my free time at work. I’ll talk about the team documentation process I developed some other time.

This post reviews my process for reviewing these volumes of information in my pockets of free time.

### Step 1: Create a draft doc with the new outline.

**My first step is to create a new document with the new outline.** I’ll fill out as many sub bullets as I can to guide the content, though I know those may change, or might not even be headers long-term.

The master guides all generally follow the same outline, so as a reader, once you learn one you don’t have to do too much brain work to understand how the rest are organized. I did 6 months of research on technical writing best practices before I decided on this outline and will revisit all my reasons for it later.

Briefly, here is the general outline the master guides followed in the most recent revision:

- Overview & Process
- Instructions & Troubleshooting
- Reporting
- Support
- Glossary

### Step 2: Fill out the new outline.

**Create a copy of the current version of the guide, and then pull content from the current guide to fill in the new outline.** This is a task that requires endurance and focus. You’re essentially reorganizing the content as you migrate, then cleaning it up later. It can be difficult to ignore things and stop yourself from filling in gaps that you notice – keep your notebook handy to jot those down for later.

Make a copy of the current guide (don’t work in the live guide!) and then open it side by side with the draft doc you created and populated the new outline. Then, cut the content from the “current guide copy” (CGC) and paste it into the “new outline draft” (NOD), wherever it fits in the new outline.

As you do so, leave the headers in the CGC. After you move the content, type the updated path (where the content lives in the NOD). Right now this is a notes doc but later you’ll clean it up and it will serve as a helpful transition resource to the team that shows them where the content was previously, and where they can find it in the new outline.

**You’ll hit some roadblocks**, and here’s what I did about them:

- Content in the CGC doesn’t fit in the new outline
    - Does it need to be a new header?
    - Should it be a separate guide (aka, “satellite doc”)
    - Can we archive it?
- If separate guide or archived
    - Extract the content and paste it into a separate doc
    - Instead of the path to the content in the NOD, add the link to this new satellite doc to your CGC so you are reminded to review it later
    - If it’s archived content, put ARCHIVED in the title (later you will move all archived content to an archived folder so it’s out of the way)

### Step 3: Edit each section (H1 header) as you go.

For each section/H1 header and subsections (e.g., “Overview & Process”), stop to edit. Rather than going top to bottom, my first edits **go in order of content type – topics first, then category overviews, then the summary/overview of the section**.

**Topic editing:**

- Updating/clarifying content for current team needs
- Reviewing for currency/accuracy
- Adapting to any changes in style guide
- If requested by the team, adding videos
- Linking to vendor guides where possible
- Updating supplementary or visual elements (images, tables, tips, etc.)
    - If the information can be presented better, update it
    - If screenshots don’t match, update them! Also, consolidate where you can
    - If you can add a link to a helpful guide, give a troubleshooting tip, or provide perspective – do it!
- Updating reference text that indicates where the reader can find knowledge elsewhere in guides

**Overview/summary editing:**

- Write or update so the overview explains what the reader will learn/find in the following sections under this header. This helps with keyword search and gives a quick reference for readers to find what they are looking for.
- Add links to supplementary guides that don’t live anywhere else

After the topics and summaries are edited, **review the entire section and fill in missing content:**

- Fill in gaps – write new content
- Update headers for consistency
- Review top to bottom for consistency, documentation standards alignment, and any other changes that stand out

| Tracking Updates                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Because I was completing these edits for an hour here and there over several weeks for each section, **I had a system to help me keep track of my progress**. I had the full outline at the top of the NOD doc in smaller print (so it wouldn’t take up much room). As I progressed through edits, I added emojis to each heading to help me track:<br><br>🏴 **Started:** Sections I started writing, but for one reason or another can’t finish (pending developer question, lost steam, need to revisit later).  <br>💡 **To Write:** Sections that didn’t exist before – I targeted these last. These come from gaps I identified while writing the outline draft or while migrating content.  <br>✅ **Done for now:** To be precise in my labeling, these are done “for now” because I will be doing further edits later. These are ready for the next step and I don’t need to go back and review them for any reason. |

### Step 4: Migrate changes in-progress to live guide.

It was important to get the information to the team as soon as possible, so I didn’t wait to review the entire guide before sharing my edits. **After each H1 section edit was complete, I migrated it to the live version of the guide.**

First, make sure no one else is in the live guide. Then, in the live guide, reorganize the current content to fit the new outline. In Word, you can open the Navigation panel and drag/drop headers to move them around. Update the headers to match the new outline, then copy/paste the new content from the NOD to the live document, section-by-section, adding the new outline headers as well.

As you update the live guide, communicate to your team so they know what’s happening. In the guide, I noted where the “new content” started and ended so they could follow the changes.

### Step 5: Full guide cleanup and editing.

After you’ve updated, written, and moved all the new content to the live guide, **find a few hours to dedicate to a full guide cleanup and editing session**. You will review the guide top to bottom, take a break for a few days, then review it again.

Use the new style guide to apply consistent formatting across the entire guide. You’ll have done most of this work when editing each section/H1 header, but this sweep validates and allows you to update any inconsistencies.

(Because I had 4 guides to update, I eventually began copy/pasting some features from another guide because it was faster than building it from scratch. In retrospect, I should have added it to the style guide as a template for copy/pasting purposes.)

### Step 6: Update references.

Clean up the CGC outline so it’s easy for the team to read/use (later renamed “Doc Transition Outline”). I kept the headers so they could use Word’s Table of Contents features to navigate. **When a reader visited a section in the former Doc Transition Outline, they would find instructions on where to find that content in the new outline/live guide.**

I found that by the time I got to the third master guide revision, the team didn’t need the Doc Transition Outline. They were comfortable using the new outline and knew what type of information to find where after using two guides with the new structure.

After updating the guide you just revised, skim through remaining guides to update the references. References usually include a full breadcrumb, unless referencing a section preceding or subsequent the one the reader is currently reading (those would have been updated in Step 3). Use the outline as a map to guide you on which references to update across all guides. You can ctrl+F the old heading in each guide and replace it that way.

### Step 7: Clean up satellite docs.

**Clean up the guides that the master guide links to.** This may seem odd to leave for last, but remember, the content was already written out; you identified a need for this to be a separate guide. Satellite docs are usually 1-5 pages (including many 1-pagers for quick reference).

At this time you’ll also click every link in the guide to a) verify it works and b) verify it’s up to date.

This requires a little cleanup because it was a section within an outline, but is now its own document. Headers might change, and the summary or presentation of content may need updates. Editing includes the same considerations as topic editing in Step 3, though these shorter guides don’t often include many images or callout boxes.

### Step 8: Launch and support!

I like to leave the satellite docs for last because it gives me a clear ending on a master guide revision. **Once the revision is complete, communicate to your team/stakeholders!** Provide a walkthrough of everything that’s new about the guides, and briefly describe where they might find commonly accessed information.

Follow up in subsequent team meetings for a few weeks so everyone feels supported as they learn how to navigate and use the new guide. Even with the Doc Transition Outline, they’ll have questions on where to find content for about a month or two.

Because the team has such a huge documentation library, I get to be part of every team member’s onboarding by showing them how to use it and where to access all their resources. I also do a documentation refresher for the team at large once or twice a year, not only as a presentation but also as a “sharing is caring” session where they can talk about how they use the guides and trade tips.

## On to better things…

I am overall ecstatic that the master guides are retiring in favor of a new approach which will allow us to reuse content and bookmark topics.

It’s nice to reflect on the work that I’ve accomplished over time – writing this out has made me realize what a huge endeavor it is to edit a 150 page document in just a few months. It was work I really enjoyed – and now, as I restructure the master guides into their new and probably final outline, I’m excited for what’s ahead.

---
Created: 11/30/23
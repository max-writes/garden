---
{"dg-publish":true,"dg-path":"fragments/library/Accessibility Trainings.md","permalink":"/fragments/library/accessibility-trainings/","created":"2025-05-17T17:22:50.168-04:00","updated":"2025-06-26T10:09:00.497-04:00"}
---


# Accessibility Trainings
These were employer-provided accessibility trainings from https://eliquotraining.com during May 2025 - 6 days (15 hours total) of intense training covering various topics.

The training went to a group of employees in various roles: content support teams, learning technologists, instructional designers, faculty support, and more. All of these humans touch course content, documentation, or other parts around the classroom or faculty/student experience. Everyone's takeaways will be different depending on their day to day needs/what their role requires.

I am building this page with my notes, questions, and takeaways related to not just my position writing user guides and release notes, but also my website-making hobby.

*In progress:* The notes are getting typed up post-training but with holidays and vacations things keep getting in the way!

## Sessions 1 & 2

- Headers and structure
	- Accessibility rules for headings are the same everywhere - HTML files, docs, powerpoints, etc. How you apply the headings will be different per format.
	- Proper structure is the number 1 way to make a document accessible
	- If there is no structure, a screenreader user (SRU) will not be able to navigate through the doc without reading literally everything. Headers allow them to skip through the document to find the topic they need (similar to what a table of contents does for a visual user). For accessibility purposes, the Table of Contents isn't mandatory (but it is nice for visual users)
	- In Word the "Title" style has no semantic value, no information is passed to SRU; this is why it's recommended to use Header 1 (H1).
	- Use headers in order. H1-H6 have semantic meaning (you shouldn't have more than that anyway for readability and document use best practices). SRU can use keyboard shortcuts and press 1 (or Shift+1) to navigate through the document H1s, 2 (or Shift+2) to navigate between H2s, and so on. 
	- There should only be one H1 on the page: the title
	- Consistency in document presentation, templating, styles, colors, tones, voice, etc., is accessible because it reduces cognitive load. (Consistency is also a knowledge library best practice.)
	- Use the lists feature when making lists and don't use a table to make it 3 columns. You can use the layout feature in Word desktop version to make a list display in 3 columns. The SRU experience is horrible if you put content in a table other than relational data.
	- Always add alt text to images unless it's decorative.
		- Not decorative: Home icon or icons without words next to them (icon is the meaning of the link), company/business logos, images in content that are contextually vital for understanding the content
		- Decorative: Wordless banners that aren't meaningful to the content (if you removed them, it'd make no difference contextually), design or layout graphics/icons with other indicators of purpose (e.g., in the classroom each content type has an icon next to it, but is also labeled with the content type using text - the icon is not the only item holding meaning). 
	- Alt text language standards are a gray area because appropriate alt text changes depending on the context and audience
	- Stick to 120 characters or less because some SRs will cut off after that
	- SRs will skip decorative images entirely so don't label something decorative if it actually isn't.
	- Italics - don't use it for emphasis. Use bold instead.
	- Link formatting - if it's clearly a link in greyscale (accessible for low vision users) then you don't need to underline it. Otherwise all links should be underlined.
		- I have questions - what about when people apply different text decorations (like background color or something) - what is/isn't accessible with that?

After the session I started writing some user guides for our new Pearson Mastering integration and I immediately saw how inaccessible the template is, using italics everywhere, two H1 headers, many more little details I learned after just 1 session! It held all the knowledge on accessibility that I had up to that point and I won't be beating myself up for not knowing everything, but I'm excited to compile all my learnings and adjustments to make once we've walked through doc and PDF accessibility.

Some questions that I'm excited to ask when we get to the in-depth alt text section:
- How to write good alt text for screenshot images
- Do they need alt text? the point of them is to show the user what they should be looking at on screen - they are for visual users. I am not sure how it'd serve a low or no vision user when the instruction is already in context too, to describe what they should click/do.

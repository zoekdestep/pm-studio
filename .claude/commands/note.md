---
description: Capture a note to the knowledge base
arguments:
  - name: content
    description: The content to capture (can be a topic, idea, or full text)
    required: true
---

You are helping capture a note: **$ARGUMENTS.content**

## Process

1. **Understand** — If the content is brief or unclear, ask clarifying questions (context, source, follow-ups).

2. **Categorize** — Determine the best folder:
   - `/notes/ideas/` — Raw ideas, hunches, things to explore
   - `/notes/research/` — User research, competitor analysis, data findings
   - `/notes/reading/` — Articles, books, learnings from external sources

3. **Enrich from WorkIQ** — Always offer to pull related context:
   - If the user is capturing meeting takeaways: pull the meeting transcript/summary from WorkIQ as source material
   - If the topic relates to ongoing discussions: search for relevant emails or documents
   - If the user is capturing research: search for related internal docs

4. **Enrich from other connectors** (if available):
   - If ~~user feedback is connected and user is capturing research: offer to pull related support tickets or feedback

5. **Format** — Structure with title, date, source, content (kept raw), tags, and open questions. Never clean up notes for tone or clarity.

6. **Save** — Generate filename `YYYY-MM-DD-descriptive-title.md` and save to the appropriate `/notes/` subfolder.

7. **Connect** — Surface any connections to other notes, ongoing work in `/output/`, or context files.

---
description: Capture a note to the knowledge base
arguments:
  - name: content
    description: The content to capture (can be a topic, idea, or full text)
    required: true
---

You are helping capture a note: **$ARGUMENTS.content**

## Process

### 1. Understand the Note

If the content is brief or unclear, ask clarifying questions:
- What's the context for this thought?
- Is this from a meeting, reading, or your own thinking?
- Are there any follow-up thoughts or open questions?

### 2. Categorize

Determine the best folder:
- `/notes/ideas/` - Raw ideas, hunches, things to explore
- `/notes/research/` - User research, competitor analysis, data findings
- `/notes/meetings/` - Meeting notes, decisions, action items
- `/notes/reading/` - Articles, books, learnings from external sources

Suggest the category and confirm with the user.

### 3. Format the Note

Structure the note with:
- **Title**: Descriptive, searchable title
- **Date**: Today's date
- **Source**: Where this came from (meeting, article, own thinking)
- **Content**: The main content, but never clean it up for clarity
- **Tags**: Relevant topics for future searching
- **Open questions**: Any follow-ups or things to explore

### 4. Save

Generate a filename: `YYYY-MM-DD-descriptive-title.md`

Save to the appropriate folder in `/notes/`.

### 5. Connections

After saving, check if this note connects to:
- Other notes in the knowledge base
- Ongoing work in `/output/`
- Context in `/context/`

Surface any interesting connections.

## Example Output

```markdown
# [Title]

**Date:** [Today's date]
**Source:** [Meeting / Article / Own thinking / etc.]
**Tags:** #topic1 #topic2

## Content

[The main content of the note]

## Open Questions

- [Any follow-up questions or things to explore]
```

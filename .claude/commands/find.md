---
description: Search across all notes and context for relevant information
arguments:
  - name: query
    description: What you're looking for
    required: true
---

You are helping find information about: **$ARGUMENTS.query**

## Search Process

### 1. Clarify if Needed

If the query is ambiguous, ask:
- Are you looking for a specific document or general information?
- What's the context - are you writing something or just exploring?
- Any particular time period or topic area?

### 2. Search Locations

Search across all knowledge in this order:

**Notes** (`/notes/`)
- `/notes/ideas/` - Raw ideas and hunches
- `/notes/research/` - Research findings and analysis
- `/notes/meetings/` - Meeting notes and decisions
- `/notes/reading/` - External learnings

**Context** (`/context/`)
- Product and technical context
- Example documents

**Output** (`/output/`)
- Previous specs, strategies, and shipping decisions

### 3. Present Results

For each relevant finding:
- **Source**: File path and name
- **Relevance**: Why this matches the query
- **Excerpt**: Key relevant content
- **Date**: When it was created/modified

### 4. Synthesize

After presenting individual results:
- Summarize what you found across sources
- Surface any contradictions or tensions
- Note any gaps - what's NOT in the knowledge base
- Suggest follow-up queries if relevant

## Output Format

```
## Found in [filename]
**Relevance:** [Why this matches]

> [Relevant excerpt]

---

## Found in [filename]
...

---

## Summary

[Synthesis of findings across sources]

### Connections
- [Any interesting links between findings]

### Gaps
- [What's missing from the knowledge base on this topic]
```

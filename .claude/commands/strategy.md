---
description: Write a research-backed strategy doc exploring an opportunity or problem space
arguments:
  - name: topic
    description: The topic, opportunity, or question to explore
    required: true
---

You are helping write a strategy document on: **$ARGUMENTS.topic**

Follow all instructions in CLAUDE.md (context loading, research, askback, voice, quality checklist, auto-save, agent offering).

## WorkIQ Research

Always query WorkIQ for:
- Related emails, meeting notes, and strategy discussions
- Recent meeting transcripts on the topic
- Existing strategy docs, research, and decision records in SharePoint/OneDrive
- Team discussions and decisions on the topic

## Additional Connectors (if available)

If ~~product analytics is connected:
- Pull relevant usage metrics, trends, behavioral data

## Write

Check `context/examples/` for strategy doc examples to match structure and voice. Key sections: compelling title, introduction, purpose, research/framework sections with evidence, principles, application, next steps, open questions, sources.

**Auto-save** to `/output/strategies/$ARGUMENTS.topic.md`.

## Agents

After writing, suggest: **reviewer**, **question-generator**, **editor**.

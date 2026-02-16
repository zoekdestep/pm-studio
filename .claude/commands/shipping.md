---
description: Write a shipping decision doc with learnings, metrics analysis, and recommendation
arguments:
  - name: feature
    description: The feature to make a shipping decision about
    required: true
---

You are helping write a shipping decision document for: **$ARGUMENTS.feature**

Follow all instructions in CLAUDE.md (context loading, research, askback, voice, quality checklist, auto-save, agent offering).

## WorkIQ Research

Always query WorkIQ for:
- Related emails, meeting notes, and customer feedback threads
- Meeting transcripts discussing this feature's rollout
- Documents and decision records related to this feature

## Additional Connectors (if available)

If ~~product analytics is connected:
- Pull actual metrics for the feature (adoption, engagement, errors, performance)

If ~~user feedback is connected:
- Pull customer sentiment, support tickets, feature requests related to the feature

If ~~project tracker is connected:
- Pull rollout status, remaining work items, bugs

## Write

Check `context/examples/` for shipping decision examples to match structure and voice. Key sections: introduction with current state, learnings (business metrics, customer sentiment, partner learnings), road ahead (recommendation with reasoning, success criteria, future steps).

**Auto-save** to `/output/shipping-decisions/$ARGUMENTS.feature.md`.

## Agents

After writing, suggest: **reviewer**, **metrics-designer**, **edge-case-finder**, **editor**.

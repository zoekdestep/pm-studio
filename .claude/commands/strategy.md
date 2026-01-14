---
description: Write a research-backed strategy doc exploring an opportunity or problem space
arguments:
  - name: topic
    description: The topic, opportunity, or question to explore
    required: true
---

You are helping write a strategy document on: **$ARGUMENTS.topic**

## Phase 1: Internal Research

First, search for relevant context within the workspace:
1. Check `/notes` for any research, ideas, or background on this topic
2. Check `/context/product-context.md` for strategic alignment
3. Check `/context/examples/` for any strategy doc examples (if available)

Report what you found that's relevant.

## Phase 2: External Research & Competitor Analysis

Before interviewing the user, conduct external research:
1. **Competitor landscape** - How are competitors (Google, Notion, Adobe, etc.) approaching this space? What strategies are they pursuing?
2. **Industry research** - What academic research, industry reports, or expert perspectives exist on this topic?
3. **Market trends** - What relevant trends should inform our strategic thinking?

Use web search to gather current information. Summarize key findings:
- Competitor strategies and positioning
- Research-backed insights that should inform our approach
- Emerging patterns or opportunities

This research should be incorporated into the strategy doc with proper citations.

## Phase 3: Discovery Interview

Gather information through an askback interview. Ask 2-3 questions at a time:

**Framing**
- What's the core question or opportunity you're exploring?
- What triggered this? Why is this important now?
- Who is the audience for this doc? What decision does it inform?

**Evidence & Research**
- What research or evidence do you have so far?
- Are there frameworks or external research we should reference?
- What have you tried or considered already?

**Scope**
- What's the scope boundary - what's explicitly NOT in this doc?
- Is this doc meant to convince, explore, or document a decision already made?
- What would a successful outcome look like?

Skip questions you can already answer from context.

## Phase 4: Write the Strategy Doc

After gathering enough context, write the strategy doc using the template at `/context/templates/strategy-template.md`.

Key sections to include:
- Compelling title that frames the insight
- Introduction (context, opportunity)
- Purpose of this document
- Research/framework sections with evidence
- Principles or implications derived from research
- Application to the specific problem
- Follow-ups and next steps
- Open questions and risks
- Sources

**IMPORTANT: Auto-save the strategy doc** to `/output/strategies/` with filename `$ARGUMENTS.topic.md`. Create the directory if it doesn't exist. Do this automatically without asking.

## Phase 5: Analysis

After writing, ask if the user wants to run agents:
- **Completeness Checker** - identify gaps in reasoning
- **Connection Finder** - link to other notes and ideas
- **Editor** - polish for readability and tone

## Voice & Style

Read `/context/tone-and-voice.md` and match that tone throughout the document.

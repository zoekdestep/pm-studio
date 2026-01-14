---
description: Write a shipping decision doc with learnings, metrics analysis, and recommendation
arguments:
  - name: feature
    description: The feature to make a shipping decision about
    required: true
---

You are helping write a shipping decision document for: **$ARGUMENTS.feature**

## Phase 1: Research

First, search for relevant context:
1. Check `/notes` for any metrics, feedback, or learnings about this feature
2. Check `/output/specs/` for the original spec if it exists
3. Check `/context/examples/` for any shipping decision examples (if available)

Report what you found that's relevant.

## Phase 2: Discovery Interview

Before writing, gather information through an askback interview. Ask 2-3 questions at a time:

**Current State**
- What's the current rollout state? (% of users, which rings/audiences)
- How long has it been in this state?
- What's the proposed next step? (expand rollout, hold, pull back)

**Metrics & Evidence**
- What are the key metrics you're tracking? (activation, engagement, retention)
- What are the guardrails? (satisfaction, error rates, performance)
- What does the data show so far?

**Customer Signal**
- What customer feedback have you received? (positive and negative)
- Any escalations or compliance concerns?
- What are partner teams learning? (relevant adjacent products)

**Recommendation**
- What's your recommendation leaning?
- What would change your mind?
- What are the main risks and how would you mitigate them?

Skip questions you can already answer from context.

## Phase 3: Write the Shipping Decision Doc

After gathering enough context, write the doc using the template at `/context/templates/shipping-template.md`.

Key sections to include:
- Introduction (current state, proposed decision)
- Learnings
  - Business metrics (with specific numbers and trends)
  - Customer sentiment (balanced - both positive and concerns)
  - Partner learnings (if relevant)
- Road ahead
  - Recommendation with reasoning (pros, risks, evidence, fallback)
  - Platform-specific considerations
  - Future steps
- Success criteria for this rollout phase
- Technical appendix (error analysis, etc. if relevant)

**IMPORTANT: Auto-save the shipping decision** to `/output/shipping-decisions/` with filename `$ARGUMENTS.feature.md`. Create the directory if it doesn't exist. Do this automatically without asking.

## Phase 4: Analysis

After writing, ask if the user wants to run agents:
- **Completeness Checker** - ensure all key metrics are covered
- **Metrics Designer** - validate guardrails and success criteria
- **Edge Case Finder** - surface rollout risks
- **Editor** - polish for readability and tone

## Voice & Style

Read `/context/tone-and-voice.md` and match that tone throughout the document.

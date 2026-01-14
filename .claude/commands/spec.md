---
description: Write a product spec with goals, workstreams, milestones, and metrics
arguments:
  - name: feature
    description: The feature or capability to spec out
    required: true
---

You are helping write a product spec for: **$ARGUMENTS.feature**

## Phase 1: Internal Research

First, search for relevant context within the workspace:
1. Check `/notes` for any background on this topic
2. Check `/context/product-context.md` for strategic alignment
3. Check `/context/technical-context.md` for technical constraints
4. Check `/context/examples/` for any spec examples (if available)

Report what you found that's relevant.

## Phase 2: Competitor & Market Research

Before interviewing the user, conduct external research:
1. **Competitor analysis** - How are competitors (Google, Notion, Adobe, etc.) solving this problem? Check `/context/product-context.md` competitive landscape section for known competitors.
2. **Industry patterns** - What patterns or best practices exist for this type of feature?
3. **User expectations** - What do users expect based on experiences with similar products?

Use web search to gather current information. Summarize key findings:
- What competitors do well that we should learn from
- Gaps or opportunities competitors haven't addressed
- Relevant patterns or research that should inform our approach

This research should inform the spec's positioning and differentiation.

### Research Quality Standards

**For any key claims or assumptions, prioritize sources in this order:**

| Tier | Source Type | Examples |
|------|-------------|----------|
| 1 | Peer-reviewed academic papers | CHI, CSCW, journals |
| 2 | Preprints from reputable institutions | arxiv from Stanford, MIT, Microsoft Research |
| 3 | Industry analyst reports (with methodology) | Gartner, Forrester, McKinsey |
| 4 | Primary research from credible orgs | NN/g studies with sample sizes, Pew Research |
| 5 | First-party data | Internal telemetry, user research |

**Avoid relying solely on:**
- Vendor/marketing content (potential bias)
- Blog posts and opinion pieces without data
- Practitioner articles without methodology

**After gathering sources:**
1. Explicitly note the credibility tier of each source
2. Flag any key claim that relies only on Tier 5+ sources
3. For critical assumptions, actively search for stronger academic evidence

## Phase 3: Discovery Interview

Gather information through an askback interview. Ask 2-3 questions at a time:

**Problem & Context**
- What problem are we solving? Why now?
- Who experiences this problem? How painful is it?
- What's the current state or workaround?

**Solution Direction**
- Do you have a solution in mind, or should I propose options?
- Any constraints I should know? (technical, timeline, dependencies, team capacity)
- What's explicitly out of scope?

**Success & Measurement**
- How will we know this worked? What are the success metrics?
- What are the guardrails (metrics that shouldn't regress)?
- Is this a bet (uncertain outcome) or a known improvement?

Skip questions you can already answer from context. Adapt based on what you learn.

## Phase 4: Write the Spec

After gathering enough context, write the spec using the template at `/context/templates/spec-template.md`.

Key sections to include:
- Introduction (context, opportunity, case for this work)
- Purpose of this document
- Vision (long-term and short-term priorities)
- Goals with specific metrics
- Workstreams with Crawl/Walk/Run milestones
- Dependencies and risks
- Open questions and unknowns
- Team

**Include a Competitive Context section** that summarizes:
- How competitors approach this problem
- What we're learning from or differentiating against

**IMPORTANT: Auto-save the spec** to `/output/specs/` with filename `$ARGUMENTS.feature.md`. Create the directory if it doesn't exist. Do this automatically without asking.

## Phase 5: Analysis

After writing, ask if the user wants to run agents:
- **Completeness Checker** - identify missing sections or gaps
- **Edge Case Finder** - surface scenarios that might be missed
- **Metrics Designer** - refine success criteria and guardrails
- **Editor** - polish for readability and tone

## Voice & Style

Read `/context/tone-and-voice.md` and match that tone throughout the document.

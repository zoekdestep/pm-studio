# Product Context

This file helps PM Studio understand your product domain. It provides context for writing specs, strategies, and decisions.

---

## Product Overview

**Product:** [Your product name]
> *Example: Acme Collaboration Platform*

**Focus area:** [Your specific area within the product]
> *Example: Real-time collaboration features*

**Key experiences:**
- [Experience 1]
- [Experience 2]
- [Experience 3]

> *Example:*
> - *Live cursors - see where collaborators are working*
> - *Comments & threads - async discussion on content*
> - *Version history - track and restore changes*

---

## Strategy & Vision

### North Star

[What's the long-term vision for your product area?]

> *Example: Make collaboration feel like you're in the same room - seamless, real-time, and context-aware.*

### Current Strategic Priorities

1. [Priority 1]
2. [Priority 2]
3. [Priority 3]

> *Example:*
> 1. *Reduce collaboration friction - fewer clicks to start working together*
> 2. *Improve awareness - always know what teammates are doing*
> 3. *Scale to enterprise - support 100+ simultaneous collaborators*

### Key Bets

| Bet | Hypothesis | How We'll Know |
|-----|------------|----------------|
| [Bet 1] | [What you believe] | [Success criteria] |

> *Example:*
> | Bet | Hypothesis | How We'll Know |
> |-----|------------|----------------|
> | Presence indicators | Showing who's online increases collaboration | 20% increase in multi-user sessions |
> | Smart notifications | AI-prioritized alerts reduce noise | 50% fewer ignored notifications |

---

## User Segments

### Primary Users

**[Segment 1 name]**
- Who: [Description]
- Needs: [What they need]
- Pain points: [Current frustrations]

> *Example:*
> **Project Managers**
> - *Who: Coordinate work across 5-15 person teams*
> - *Needs: Visibility into who's working on what, easy status updates*
> - *Pain points: Too many tools, context switching, chasing people for updates*

### User Journey

[Describe the typical user journey through your product area]

> *Example: User opens shared doc → sees collaborators present → makes edit → teammate comments → they resolve together in real-time → changes auto-saved*

---

## Key Metrics

### Primary Metrics

| Metric | Definition | Current | Goal |
|--------|------------|---------|------|
| [Metric 1] | [How it's measured] | [Current value] | [Target] |

> *Example:*
> | Metric | Definition | Current | Goal |
> |--------|------------|---------|------|
> | Collaboration rate | % docs with 2+ editors | 34% | 45% |
> | Time to first collab | Minutes from share to first co-edit | 47 min | 15 min |

### Guardrails

| Metric | Threshold | Why It Matters |
|--------|-----------|----------------|
| [Guardrail 1] | [Limit] | [Reason] |

> *Example:*
> | Metric | Threshold | Why It Matters |
> |--------|-----------|----------------|
> | Sync latency | < 500ms | Collaboration feels broken if edits lag |
> | Conflict rate | < 0.1% | Lost work destroys trust |

---

## Competitive Landscape

**Tip:** You can ask Claude to research and fill out this section for you. Just say: *"Research my competitors in [space] and fill out the competitive landscape section."*

### Key Competitors

#### [Competitor 1]

| Feature | Their Approach | Our Approach | Gap/Opportunity |
|---------|----------------|--------------|-----------------|
| [Feature] | [How they do it] | [How we do it] | [What we can learn] |

> *Example:*
> #### Google Docs
> | Feature | Their Approach | Our Approach | Gap/Opportunity |
> |---------|----------------|--------------|-----------------|
> | Real-time sync | Sub-100ms, feels instant | 300-500ms, noticeable | We need to invest in sync infrastructure |
> | Presence | Colored cursors + name labels | Just cursors | Add name labels, differentiate with activity status |

### Industry Trends

**Tip:** You can ask Claude to research and fill out this section. Just say: *"Research the latest trends in [your space] and update the Industry Trends section."*

1. [Trend 1 and implications]
2. [Trend 2 and implications]

> *Example:*
> 1. *AI-assisted collaboration - auto-suggestions, smart summaries (we should explore)*
> 2. *Async-first culture - comments becoming as important as real-time (expand our threading)*

---

## Constraints & Considerations

### Technical Constraints

- [Constraint 1]
- [Constraint 2]

> *Example:*
> - *Max 50 simultaneous cursors (perf degrades beyond this)*
> - *Mobile has 2-second sync delay due to battery optimization*

### Business Constraints

- [Constraint 1]
- [Constraint 2]

> *Example:*
> - *Real-time features only for paid tiers*
> - *Enterprise customers require on-prem option*

### Platform Differences

| Platform | Considerations |
|----------|----------------|
| [Platform 1] | [Specific constraints or opportunities] |

> *Example:*
> | Platform | Considerations |
> |----------|----------------|
> | Web | Full feature set, primary platform |
> | Mobile | Limited to viewing + comments (no real-time editing) |

---

## Rollout Process

### Stages

| Stage | Audience | Purpose |
|-------|----------|---------|
| [Stage 1] | [Who] | [Why] |

> *Example:*
> | Stage | Audience | Purpose |
> |-------|----------|---------|
> | Alpha | Internal team | Find major bugs |
> | Beta | 5% of users | Validate metrics, gather feedback |
> | GA | 100% | Full launch |

---

## Related Initiatives

| Initiative | Team | How It Relates |
|------------|------|----------------|
| [Initiative] | [Team] | [Relationship] |

> *Example:*
> | Initiative | Team | How It Relates |
> |------------|------|----------------|
> | Performance overhaul | Platform team | Will improve our sync latency |
> | Mobile v2 | Mobile team | Opportunity to add real-time editing |

---

## Glossary

| Term | Definition |
|------|------------|
| [Term] | [Definition] |

> *Example:*
> | Term | Definition |
> |------|------------|
> | OT | Operational Transform - algorithm for real-time sync |
> | CRDT | Conflict-free Replicated Data Type - alternative sync approach |

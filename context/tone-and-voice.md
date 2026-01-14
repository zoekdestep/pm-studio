# Tone and Voice Guide

This guide defines the writing style for your PM documents. Use it to ensure consistency across specs, strategies, and decisions.

**Tip:** You can customize this based on your own writing samples. Share a few docs you've written and ask Claude: *"Update tone-and-voice.md with documents in the examples folder to match my writing style."*

---

## Core Voice Characteristics

### 1. Research-Backed but Accessible

**Do:**
- Cite evidence and sources with numbered references
- Explain research findings in plain language
- Use phrases like "Research shows...", "Evidence confirms..."
- Include source lists at the end of documents

**Don't:**
- Write in academic jargon
- Assume readers know the research
- Over-cite (pick the most relevant sources)

---

### 2. Honest About Uncertainty

**Do:**
- Explicitly call out unknowns: "The biggest unknown is..."
- Use "we believe" or "our hypothesis is" when speculating
- Acknowledge when you don't have data
- List open questions in their own section

**Don't:**
- Pretend certainty where none exists
- Hide risks in footnotes
- Overcommit to timelines or outcomes

---

### 3. Data-Driven and Specific

**Do:**
- Include specific numbers: "+287%", "4x more", "< 300"
- Use tables to present metrics over time
- Provide thresholds and goals, not just metrics
- Show week-over-week or period-over-period trends

**Don't:**
- Say "significant improvement" without numbers
- Use vague terms like "many users" or "soon"
- Present data without context (baseline, goal, comparison)

---

### 4. Balanced Presentation

**Do:**
- Show both positive signals AND concerns
- Acknowledge tradeoffs explicitly
- Present opposing viewpoints fairly
- Include customer quotes from different perspectives

**Don't:**
- Cherry-pick only positive data
- Bury concerns at the end
- Dismiss counterarguments

---

### 5. Clear Structure

**Do:**
- Use headers and subheaders liberally
- Tables for comparisons, timelines, and metrics
- Bold for key terms and emphasis
- Bullet points for lists of 3+ items
- Numbered lists for sequential steps or priorities

**Don't:**
- Write walls of text
- Bury key information in paragraphs
- Use inconsistent formatting

**Structure patterns:**
- Introduction → Purpose → [Main content] → Next steps → Open questions
- Crawl/Walk/Run for milestone tables
- Workstreams for parallel efforts

---

### 6. Professional but Human

**Do:**
- Use first person plural: "we" not "the team"
- Occasional light touch: "it's not exact science"
- Direct language over corporate speak
- Acknowledge contributions: "analysis by [Name]"

**Don't:**
- Be overly casual or use emojis excessively
- Use jargon without explanation
- Sound like a press release

---

### 7. Avoid AI-ish Writing

**Do:**
- Use hyphens (-) for compound words and ranges
- Be concise - get to the point
- Let the reader draw conclusions from evidence
- Write like a human colleague would

**Don't:**
- Use em-dashes (—) - they're an AI tell
- Over-explain or repeat the same point multiple ways
- Add unnecessary caveats and qualifiers
- Use phrases like "It's important to note that..." or "It's worth mentioning..."
- Start paragraphs with "Additionally," "Furthermore," "Moreover,"
- Use "delve," "crucial," "robust," "comprehensive," "leverage"
- Write overly long sentences with multiple clauses

---

## Common Patterns

### Document Openings

Start with context, not conclusions:
> "[Feature] has become a [foundation/standard] in [product], offering [capability]. Currently, [problem or gap]. There is an opportunity to [improvement]."

### Recommendations

Structure recommendations with explicit reasoning:
> **Suggestion:** [The recommendation]
> - **Pros:** [Benefits]
> - **Risk:** [What could go wrong]
> - **Evidence:** [What supports it]
> - **Fallback:** [If it doesn't work]

### Success Criteria

Be specific and measurable:
> We will determine success of this rollout by:
> - [Guardrail metric with threshold]
> - [Primary metric with target]

### Open Questions

Lead with the biggest unknown:
> "The biggest unknown is [X]. We work under the assumption that [Y], but we rely on [Z] which doesn't exist today."

---

## Words to Use / Avoid

| Instead of... | Use... |
|---------------|--------|
| Leverage | Use |
| Utilize | Use |
| Delve into | Explore / Look at |
| Crucial | Important |
| Robust | Strong / Solid |
| Comprehensive | Complete / Full |
| In order to | To |
| At this point in time | Now |
| Going forward | [Delete] |
| It's important to note | [Delete - just state it] |
| Significant | [Specific number] |
| Many users | [Percentage or count] |
| Soon | [Specific timeline] |
| The team believes | We believe |
| — (em-dash) | - (hyphen) or rewrite |

---

## Formatting Conventions

- **Dates:** "15 July '25" or "27 August '24"
- **Author line:** "Author: [Name] (alias) | Last modified: [Date]"
- **Metrics:** Use % with specific numbers, stat sig notation when relevant
- **Sources:** Numbered inline references [1], [2] with full list at end
- **Tables:** Use for any comparison of 3+ items or time-series data

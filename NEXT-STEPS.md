# Getting Started: Your First Two Weeks

A recommended workflow for getting the most out of PM Studio.


## Week 1: Setup & First Use

### Day 1: Context Files (30-45 min)

The quality of your outputs depends heavily on your context files. Start with these:

| File | What to Add |
|------|-------------|
| `context/about-me.md` | Your role, stakeholders, how you work |
| `context/product-context.md` | Product strategy, user segments, metrics |

**Tip:** Don't overthink it. Start with the basics and refine over time. You can ask Claude to help fill in sections like competitive landscape.

Lower priority files (`technical-context.md`, `tone-and-voice.md`) can wait until you need them.

### Day 2: Add Your Examples (15-30 min)

Put 4-5 of your best docs in `context/examples/`:
- A spec you're proud of
- A strategy doc that landed well
- A shipping decision that was well-received
- A doc that captures your voice nicely

You can then ask PM Studio to update the templates and tone documents with your structure, level of detail, and voice from these examples.

### Day 3: First Real Use

Pick something you're actually working on:

```
/spec [feature you're speccing]
/strategy [topic you're exploring]
```

**What to expect:**
1. Claude searches your notes and context
2. Does competitor/market research
3. Asks you 2-3 questions at a time
4. Writes a draft and auto-saves to `/output/`
5. Offers to run agents (completeness checker, edge case finder, etc.)

Your first doc won't be perfect - the system improves as you add more context over time. 

### Days 4-5: Build Your Knowledge Base

**Port over existing notes:** If you have notes in another tool (Notion, OneNote, etc.), bring them over to `/notes/`. The more context Claude has, the better.

**Capture new notes from your daily work:**

```
/note Had a meeting with design today. They're concerned about...
/note Read an interesting article about how Notion handles...
/note Random thought: what if we approached this differently...
```

**Upload meeting transcripts:** If your meetings are auto-transcribed (e.g., Teams, Zoom), paste the transcript as a note.


## Week 2: Find Your Workflow

Everyone works differently. Experiment to find what works for you. If you find something you'd like to change structurally in the commands or agents, ask Claude to change it or update the files yourself. The real magic of the PM Studio happens when you make it truly yours!

### Example Patterns

**For Specs:**
1. `/spec [feature]` and answer the discovery questions
2. Run `edge-case-finder` to surface scenarios you missed
3. Run `completeness-checker` before sharing
4. Run `editor` for final polish

**For Strategy Docs:**
1. `/strategy [topic]` and let Claude do competitor research
2. Run `question-generator` to surface open questions
3. Run `connection-finder` to link ideas from your notes

**For Shipping Decisions:**
1. `/shipping [feature]` with your metrics ready
2. Be honest about concerns - the doc should show both sides
3. Run `metrics-designer` if you need guardrails


## What's Next?

After two weeks, you should have:
- [ ] Context files populated
- [ ] Examples added
- [ ] 10+ notes captured
- [ ] A few docs written
- [ ] A sense of which workflow suits you

From here, the system keeps getting better as you use it. Your knowledge base grows, you keep refining commands and agents, and Claude gets better at understanding your product and style.


## Tips for Success

**Keep feeding your knowledge base** - after meetings, when reading, random shower thoughts. Notes are fuel for future docs.

**Keep context files updated** - especially when strategy or priorities change.

**Run multiple agents** - don't stop at one pass. Completeness checker, then critical reader, then editor.

**Ask Claude to help with setup** - "Research competitors in [space] and update product-context.md"

**Push to GitHub** for version control - makes it easy to sync across machines and track changes over time.

### Recommended Setup

For best results, I personally use:
- **Claude Opus 4.5** with extended thinking enabled
- **VS Code** with the Claude Code extension
- **Superwhisper** for brainstorming - typing random thoughts is hard, talking is easier


## Updates

- Star the [GitHub repo](https://github.com/zoekdestep/pm-studio) for updates
- Check for new commands and agents periodically
- Share improvements back to the project - PRs are very welcome!


## Questions?

If something isn't working or you have ideas for improvement, [open an issue on GitHub](https://github.com/zoekdestep/pm-studio/issues).

Happy PMing!
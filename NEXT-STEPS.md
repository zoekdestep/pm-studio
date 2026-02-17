# Getting Started

A step-by-step guide to setting up PM Studio and running your first end-to-end workflow.


## Step 1: Install Dependencies

**Claude Code** (if not already installed):
- VS Code: Install the [Claude Code extension](https://marketplace.visualstudio.com/items?itemName=anthropic.claude-code)
- CLI: Follow the [Claude Code docs](https://docs.anthropic.com/en/docs/claude-code)

**Product-management plugin** (required):
```bash
claude plugin marketplace add product-management@knowledge-work-plugins
```

**WorkIQ for M365** (required):
WorkIQ is pre-configured in PM Studio's `.mcp.json` and starts automatically. On first use, you'll be prompted to accept the EULA and sign in with your Microsoft account. Every command queries WorkIQ by default for relevant emails, meetings, and documents.

**Open PM Studio:**
```bash
cd pm-studio
code .
```
Then open the Claude Code panel in VS Code.


## Step 2: Personalize

Fill in your context files. These are what make PM Studio's output sound like you, not a generic AI.

| File | What to add | Time |
|------|-------------|------|
| `context/about-me.md` | Your role, stakeholders, how you work, current priorities | 10 min |
| `context/product-context.md` | Product strategy, user segments, metrics, competitors, technical constraints | 15-20 min |
| `context/tone-and-voice.md` | Your writing style (good defaults included, customize as needed) | 5-10 min |

**Add examples:** Put 4-5 of your best docs in `context/examples/`. These are the most important input for voice matching. Specs, strategy docs, shipping decisions, anything that captures how you write.

**Tip:** Don't overthink it. Start with the basics and refine over time. You can ask Claude to research competitors and fill out the competitive landscape section.


## Step 3: Try It End-to-End

Pick something you're actually working on and run a plugin command from inside the workspace:

```
/product-management:write-spec
```

**What happens:**
1. CLAUDE.md kicks in: reads your context files, searches notes, loads your voice guide
2. The plugin's feature-spec methodology drives the spec writing process
3. Claude asks you discovery questions (2-3 at a time)
4. A draft is generated matching your voice and style
5. The doc auto-saves to `output/specs/`
6. Claude offers to run agents (reviewer, edge-case-finder, metrics-designer, editor)

Try running an agent on the output:
```
Run the reviewer agent on the spec we just wrote
```


## Step 4: Build Your Knowledge Base

Start capturing notes from your daily work:

```
/note Had a meeting with design today. They're concerned about the navigation redesign...
/note Read an interesting article about how Notion handles real-time collaboration...
/note Random thought: what if we approached pricing differently for enterprise?
```

Notes are fuel for future documents. The more context Claude has, the better your output gets.

If you have notes in another tool (Notion, OneNote, etc.), bring the important ones to `/notes/`.

WorkIQ will automatically offer to pull meeting transcripts as source material when you're capturing meeting takeaways.


## Step 5: Explore the Full Command Set

Try the other commands:

```
/strategy competitive-positioning
/shipping dark-mode
/product-management:roadmap-update
/product-management:stakeholder-update
/product-management:metrics-review
/product-management:competitive-brief
/product-management:synthesize-research
```

Each command benefits from the same enhancement layer: context, voice, notes search, auto-save, and agent offering.


## Ongoing

- **Feed notes constantly** — after meetings, when reading, random thoughts. Notes compound over time.
- **Keep context files updated** — especially when strategy or priorities change.
- **Upload more examples** — as your writing evolves, update `context/examples/`.
- **Run multiple agents** — don't stop at one pass. Reviewer, then editor is a good default.
- **Customize** — add agents, adjust commands, update examples. Ask Claude to help.


## Opting Out of WorkIQ

WorkIQ is queried by default for every command. If you don't want WorkIQ data for a specific command, just tell Claude to skip it (e.g., "write this spec without pulling from WorkIQ"). Other optional connectors (`~~product analytics`, `~~user feedback`, `~~project tracker`) are only used when available.


## Recommended Setup

For best results:
- **Claude Opus** with extended thinking enabled
- **VS Code** with the Claude Code extension
- **[Handy.computer](https://handy.computer/)** for voice-based brainstorming (typing random thoughts is hard, talking is easier)


## Questions?

If something isn't working or you have ideas for improvement, [open an issue on GitHub](https://github.com/zoekdestep/pm-studio/issues).

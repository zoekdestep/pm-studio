<p align="center">
  <img src="assets/pmstudio.png" alt="PM Studio" width="600">
</p>

# PM Studio

A Claude Code workspace for product managers to write high-quality specs, strategy docs, and shipping decisions through collaborative AI dialogue.

## What This Is

PM Studio is a structured environment for PM "deep work" - writing that requires focused thinking, research synthesis, and clear reasoning. Instead of generating docs from thin prompts, it acts as a **thinking partner** that:

1. **Researches before writing** - Checks your notes, context, and does competitor/market research
2. **Asks before writing** - Conducts discovery interviews to understand your goals
3. **Matches your voice** - Applies your tone guide (except for raw notes)
4. **Auto-saves to the right place** - Specs, strategies, and shipping decisions go to `/output/`
5. **Catches gaps** - Runs specialized agents to find missing pieces


## Prerequisites

Before you begin, make sure you have:

- [ ] **VS Code** installed → [Download VS Code](https://code.visualstudio.com/download)
- [ ] **Claude Code extension** installed in VS Code (search "Claude Code" in the Extensions panel)


## Quick Start

### 1. Get the Project Files

#### Option A: Clone with Git (Recommended)

If you have git installed, open your terminal and run:

```bash
git clone [this-repo-url]
```

**What this does:** Creates a copy of the project on your computer. The advantage of cloning is you can pull updates later.

#### Option B: Download as ZIP (If you're not familiar with git)

1. Go to the GitHub repository page
2. Click the green **"Code"** button
3. Select **"Download ZIP"**
4. Unzip the downloaded file to a location you'll remember (e.g., your Documents folder)


### 2. Open in VS Code

1. Open VS Code
2. Go to **File → Open Folder**
3. Navigate to the `pm-studio` folder you downloaded/cloned
4. Click **Open**

You should see the folder structure in the left sidebar.


### 3. Start Claude Code

Click the **Claude Code logo** in the top-right corner of VS Code to open the Claude Code panel.


### 4. Fill in Your Context

PM Studio works best when it knows about you and your product. Fill in these files:

| File | What to Add | Tips |
|------|-------------|------|
| `context/about-me.md` | Your role, stakeholders, priorities, PM philosophy | Examples included - just replace them |
| `context/product-context.md` | Product strategy, user segments, metrics, competitive landscape | Ask Claude to research competitors for you |
| `context/technical-context.md` | Architecture, constraints, team structure | Optional - paste a tech spec and ask Claude to fill it |
| `context/tone-and-voice.md` | Your writing style | Good defaults included - customize as needed |

### 5. Add Your Examples

Put your best docs in `context/examples/`. PM Studio can use those to learn your structure and tone.

### 6. Start Writing!

This is where the fun starts! Try one of the commands below. For example, to write a spec about citations in chat:

```
/spec citations-in-chat
```


## Commands

| Command | Purpose | Output Location |
|---------|---------|-----------------|
| `/spec [feature]` | Write a product spec with goals, workstreams, milestones | `/output/specs/` |
| `/strategy [topic]` | Write a research-backed strategy doc | `/output/strategies/` |
| `/shipping [feature]` | Write a shipping decision with metrics and recommendation | `/output/shipping-decisions/` |
| `/note [content]` | Capture a note to your knowledge base | `/notes/` |
| `/find [query]` | Search across all your notes and context | - |
| `/ideate [space]` | Generate ideas by synthesizing your notes | - |
| `/word [file]` | Export a markdown file to Word and open it | `/output/` |


## Agents

After writing, run specialized agents to improve your docs:

| Agent | What It Does | Best For |
|-------|--------------|----------|
| `completeness-checker` | Finds missing sections and gaps in reasoning | All docs |
| `edge-case-finder` | Surfaces scenarios and "what ifs" you might miss | Specs |
| `metrics-designer` | Suggests KPIs, guardrails, measurement approaches | Specs, Shipping decisions |
| `editor` | Polishes for readability, clarity, and tone | All docs before sharing |
| `tone-editor` | Compares against your voice examples | When tone feels off |
| `connection-finder` | Links ideas across your notes | Strategy docs |
| `question-generator` | Surfaces questions worth exploring | Research, Strategy |
| `critical-reader` | Finds gaps, assumptions, and logical flaws via Socratic questions | All docs |


## Best Practices

### 1. Feed Your Knowledge Base

The more you use `/note`, the smarter PM Studio gets:
- After every meeting with insights -> `/note`
- When you read something interesting -> `/note`
- Random shower thought -> `/note`

### 2. Keep Context Files Updated

Update `product-context.md` when:
- Strategy changes
- New competitors emerge
- Metrics evolve

### 3. Add Your Best Docs as Examples

Put 4-5 of your best specs/strategies in `context/examples/`. PM Studio learns:
- Your structure preferences
- Your level of detail
- Your tone and voice

After uploading the documents, don't forget to tell PM Studio to update the templates and voice documents from these.

### 4. Use Agents Iteratively

Don't just run one agent. Common flow:
1. Write a draft using one of the commands
2. Run **Edge Case Finder** - add scenarios
3. Run **Completeness Checker** - fix gaps
4. Run **Editor** - polish before sharing

### 5. Let Claude Do the Research

The competitive landscape and industry trends sections can be filled by Claude:
- "Research my competitors in [space] and fill out the competitive landscape"
- "What are the latest trends in [area]?"


## Folder Structure

```
pm-studio/
├── .claude/
│   ├── commands/       # Slash command definitions
│   └── agents/         # Agent definitions
├── context/
│   ├── examples/       # Your example docs (for tone/structure)
│   ├── templates/      # Doc templates
│   ├── tone-and-voice.md
│   ├── about-me.md
│   ├── product-context.md
│   └── technical-context.md
├── notes/
│   ├── ideas/          # Raw ideas, hunches
│   ├── research/       # User research, data findings
│   ├── meetings/       # Meeting notes, decisions
│   └── reading/        # External articles, learnings
├── output/
│   ├── specs/          # Generated specs (auto-saved)
│   ├── strategies/     # Generated strategy docs (auto-saved)
│   └── shipping-decisions/  # Generated shipping decisions (auto-saved)
├── CLAUDE.md           # Instructions for Claude
├── README.md           # This file
└── NEXT-STEPS.md       # Recommended workflow to get started after installing
```


## Customization

### Adding Your Voice

1. Put your best docs in `context/examples/`
2. Edit `context/tone-and-voice.md` to capture your style
3. The Editor agents will help match them

### Modifying Templates

Templates in `context/templates/` define the structure for each doc type. Customize them to match your own or your organization's standards.

### Creating New Commands and Agents

Make PM Studio your own! Add new `.md` files to `.claude/commands/` or `.claude/agents/`, with clear instructions for the command or for the agent's role and output format. Or ask Claude to do so! 


## Credits

This project was inspired by [SEOMachine](https://github.com/TheCraigHewitt/seomachine) by Craig Hewitt - a Claude Code workspace for SEO content creation that demonstrated how to structure AI-assisted writing workflows.


## License

MIT

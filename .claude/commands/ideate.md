---
description: Generate ideas by synthesizing notes and context
arguments:
  - name: space
    description: The problem space or area to ideate on
    required: true
---

You are helping generate ideas for: **$ARGUMENTS.space**

## Phase 1: Gather Context

First, search for relevant material:
1. Check `/notes/ideas/` for existing related ideas
2. Check `/notes/research/` for relevant research
3. Check `/notes/reading/` for external inspiration
4. Check `/context/product-context.md` for strategic constraints
5. Check `/output/` for related work

Report what you found.

## Phase 2: Frame the Space

Ask clarifying questions:
- What's the core problem or opportunity here?
- Are there constraints I should know about? (technical, timeline, team)
- What have you already considered or ruled out?
- What would a successful idea look like? (incremental improvement, big bet, quick win)

## Phase 3: Generate Ideas

Based on the context and constraints, generate ideas using multiple lenses:

### From Your Notes
Ideas that build on or combine existing thoughts in your knowledge base.

### From Analogies
Ideas inspired by how similar problems are solved in other domains or products.

### From Constraints
Ideas that emerge from working within or around the constraints you mentioned.

### From Inversion
Ideas from asking "what if we did the opposite?" or "what would make this fail?"

### From User Needs
Ideas focused on specific user pain points or jobs-to-be-done.

## Phase 4: Present Ideas

For each idea:
- **Name**: Short, memorable title
- **One-liner**: What it is in one sentence
- **How it works**: Brief description
- **Why it might work**: The insight or evidence behind it
- **Risks/concerns**: What could go wrong
- **Connection**: How it links to existing notes or context

## Phase 5: Refine

After presenting ideas, ask:
- Which of these resonate? Which don't?
- Should we go deeper on any of these?
- Did this spark any other thoughts?

Offer to:
- Save promising ideas to `/notes/ideas/`
- Develop a favorite into a fuller concept
- Run the **Question Generator** agent to surface open questions

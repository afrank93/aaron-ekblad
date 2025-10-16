---
description: 'Complete 6-step development workflow for solo developers with quality gates and tool integration'
applyTo: '**'
---

# Solo Developer Workflow Instructions

A simple, enjoyable 6-step workflow for independent developers who want to move from messy ideas to working features without overthinking the process.

## The Simple Workflow

**Goal**: Build stuff that works while having fun and learning along the way.

1. **Brainstorm & Organize** - Dump ideas, then sort them into buckets
2. **Define Features** - Turn problems into "I want to build X" statements  
3. **Plan & Prioritize** - Figure out what to build first
4. **Build** - Write code and make it work
5. **Test & Ship** - Make sure it works, then share it
6. **Reflect** - What worked? What didn't? What's next?

## Simple Step-by-Step Process

### Step 1: Brainstorm & Organize (15-30 mins)
**What**: Dump all your ideas, then sort them into simple buckets
**Tool**: `organize-ideas.prompt.md` 
**Input**: Your messy thoughts about what you want to build
**Output**: Clean markdown file: `brainstorm-[project-name].md`
**Done when**: You can scan your ideas quickly and they make sense

### Step 2: Define & Review Features (30-60 mins)
**What**: Turn problems into clear feature descriptions
**Tools**: `define-features.prompt.md`, `review-features.prompt.md`
**Input**: Your organized brainstorm file
**Output**: Individual feature files: `feature-[name].md` + feature summary
**Done when**: You know exactly what you're building and how you'll test it

### Step 3: Specify & Design (30-45 mins)
**What**: Create technical specifications for your features
**Tools**: `create-specification.prompt.md`, `validate-spec.prompt.md`
**Input**: Your approved feature definitions
**Output**: Technical spec files in `/spec/` directory
**Done when**: Specifications are clear enough to start coding

### Step 4: Plan & Prioritize (30 mins)
**What**: Figure out what to build first, create GitHub issues
**Tools**: `prioritize-backlog.prompt.md`, `create-github-issues.prompt.md`, `write-tests-from-spec.prompt.md`
**Input**: Your validated specifications
**Output**: Prioritized GitHub issues + test cases
**Done when**: You know what to code first and how to test it

### Step 5: Build (Most of your time)
**What**: Write code, make it work, have fun
**Tool**: `coding-assistant.prompt.md`
**Input**: GitHub issue + test cases
**Output**: Working feature that passes tests
**Done when**: All acceptance criteria are met and tests pass

### Step 6: Reflect (15 mins)
**What**: Quick check: What worked? What didn't? What's next?
**Tools**: `reflection-guide.prompt.md`, `capture-learnings.prompt.md`
**Input**: Your completed work
**Output**: Simple reflection file + key insights for next time
**Done when**: You know what to keep doing and what to change

**Input**: Completed work cycle
**Output**: Documented learnings, process improvements, updated workflow

**Quality Gate**: Key learnings captured and process updates identified

**Decision Point**:
- If significant learnings captured → Apply to next cycle
- If patterns emerge → Update workflow instructions
- Ready for next brainstorm cycle → Return to Step 1

## Quality Gates and Checkpoints

### Universal Quality Standards
- **No Lost Content**: Original ideas preserved through transformations
## Keep It Simple Guidelines

### The Golden Rules
1. **Time-box everything** - If a step takes longer than planned, move on
2. **Good enough beats perfect** - Ship working features over perfect specs
3. **One thing at a time** - Focus on current step, don't jump around
4. **When stuck, ask for help** - Use prompts to get unstuck fast

### Common Pitfalls (And How to Avoid Them)
- **Analysis paralysis**: Set 30-min timer for planning steps, then start building
- **Scope creep**: Write down new ideas for "next time", finish current thing first  
- **Tool overwhelm**: Use one prompt at a time, ignore the rest until you need them
- **Perfectionism**: Remember - you can always improve it later

### Success Looks Like
- You're building stuff regularly and having fun
- Your ideas turn into working features people can use
- You learn something new with each project
- The process feels helpful, not burdensome

## Quick Start Checklist
- [ ] Have a messy idea you want to build
- [ ] Use `organize-ideas.prompt.md` to sort your thoughts  
- [ ] Use `define-features.prompt.md` to clarify what you're building
- [ ] Use `create-specification.prompt.md` to add technical details
- [ ] Use `prioritize-backlog.prompt.md` to pick what's first
- [ ] Start coding and use `coding-assistant.prompt.md` when you get stuck
- [ ] Use `reflection-guide.prompt.md` when you finish something

That's it. The whole workflow in 6 bullets. Everything else is just details.
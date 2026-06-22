# Example: AI-Friendly Project Memory

This is a synthetic example. Do not copy private project notes into a public repository.

## Project Control Tower

```yaml
---
type: project
area:
  - projects
  - "[[Projects]]"
topics:
  - "[[AI Context]]"
description: Synthetic project used to demonstrate AI-friendly project memory.
status: active
stage: execution
next_action: Review the context brief and decide the next experiment.
repo:
lang:
  - en
created: 2026-06-22
updated: 2026-06-22
---
```

# Project Atlas

## Goal

Build a local-first research workflow that helps a person hand off project context to an AI assistant without pasting the whole vault.

## AI Context

- [[Project Atlas - Context Brief]]
- [[Project Atlas - Decision Log]]
- [[Project Atlas - Action Log]]
- [[Project Atlas - Failed Attempts]]

## Current State

The project has a working prototype and needs feedback on whether the context brief is enough for a new assistant session.

## Next Action

- [ ] Ask one reviewer to use only the context brief and identify what is missing.

## Context Brief

```yaml
---
type: note
project: "[[Project Atlas]]"
ai_context_role: context_brief
context_priority: high
status: active
lang:
  - en
created: 2026-06-22
updated: 2026-06-22
---
```

# Project Atlas - Context Brief

## Project Goal

Help users pass focused project context to AI assistants.

## Current State

The prototype works locally. The main risk is that the assistant receives too many adjacent notes and misses the real project state.

## Constraints

- Must stay local-first.
- Must not require a specific AI provider.
- Must avoid private or personal examples in public docs.

## Useful Context

- [[Project Atlas - Decision Log]]
- [[Project Atlas - Action Log]]
- [[Project Atlas - Failed Attempts]]

## What Not To Assume

- Do not assume every project needs a large memory structure.
- Do not assume AI memory is reliable unless the relevant notes are provided.

## Next Useful Action

- [ ] Compare the assistant response with and without the decision log.

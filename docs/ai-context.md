# AI-Friendly Project Memory

This module is optional.

The core starter still works without AI. The goal here is narrower: organize project notes so an AI assistant can receive less context, but better context.

## The Problem

AI assistants do not need your whole vault. They need the smallest set of notes that explains:

- what the project is;
- what is true right now;
- what decisions have already been made;
- what should happen next;
- what has already failed;
- what constraints must not be forgotten.

If those facts live only inside daily notes, meeting notes, chat transcripts, or scattered project pages, you end up pasting too much context. More context is not automatically better. Long context can make the model slower, more expensive, and less focused.

## Design Principle

Use a small project-memory layer:

- one project note as the human control tower;
- one short context brief for AI handoff;
- one decision log;
- one action log;
- one failed-attempts note when the project has enough history.

For small projects, keep these as sections inside the main project note. For long-running projects, split them into separate linked notes.

## Recommended Project Memory Notes

| Note | Purpose | When to create it |
| --- | --- | --- |
| `Project Name.md` | Human-facing project control tower. | Always, for real projects. |
| `Project Name - Context Brief.md` | Short AI handoff: current state, scope, constraints, useful links. | When you use AI across more than one session. |
| `Project Name - Decision Log.md` | Decisions, rejected options, and consequences. | When the project has technical, product, or strategic choices. |
| `Project Name - Action Log.md` | Current next actions, blockers, and review notes. | When tasks are spread across meetings or sessions. |
| `Project Name - Failed Attempts.md` | What did not work and why. | When an assistant or person might repeat old mistakes. |

Do not create all of these by default. Create the missing note only when the absence is making context expensive or confusing.

## Suggested Properties

Keep these fields optional. They are meant for retrieval and review, not bureaucracy.

```yaml
type: note
project: "[[Project Name]]"
ai_context_role: context_brief
context_priority: high
status: active
lang:
  - en
created: "{{date:YYYY-MM-DD}}"
updated: "{{date:YYYY-MM-DD}}"
```

Recommended `ai_context_role` values:

- `control_tower`
- `context_brief`
- `decision_log`
- `action_log`
- `failed_attempts`
- `constraints`
- `sources`
- `open_questions`

Recommended `context_priority` values:

- `high`: usually useful in an AI handoff.
- `medium`: useful for review, but not always needed.
- `low`: background material or archive context.

## What Belongs in an AI Context Brief

A good context brief should fit on one screen.

Include:

- current project goal;
- current state;
- non-negotiable constraints;
- links to decision/action/failure notes;
- what the AI should not assume;
- the next useful question or action.

Exclude:

- full meeting transcripts;
- long source excerpts;
- old brainstorming that is no longer active;
- personal notes;
- anything you would not paste into a public issue or support thread.

## How This Saves Tokens

This pattern reduces token waste in three ways:

1. Stable context is separated from volatile context.
2. The assistant can start from the brief and only request detailed notes when needed.
3. Repeated decisions and failed attempts do not need to be rediscovered from a long history.

For API workflows, stable prompt prefixes can also benefit from prompt caching. That does not remove the need for concise notes, but it rewards keeping shared instructions and project facts stable instead of rewriting them every time.

## Minimal Workflow

1. Start with `templates/project.md`.
2. Add a short `AI Context` section with links to memory notes.
3. When the project starts spanning multiple sessions, create `project-context-brief.md`.
4. Record decisions in `decision-log.md` as they happen.
5. Review `action-log.md` weekly.
6. Add `failed-attempts.md` only when repeated mistakes become a real risk.

## Anti-Patterns

Avoid:

- putting the whole project history in one giant prompt;
- treating AI memory as reliable without written notes;
- creating ten required project files for every small task;
- adding metadata fields that no query or assistant will use;
- mixing private journal content into public project examples;
- writing vague summaries such as "worked on the project" without decisions or next actions.

## Relationship to the Starter Philosophy

This module follows the same rules as the rest of the starter:

- folders are trays, not the main architecture;
- the note type model stays small: AI memory notes use `type: note` plus optional context fields;
- links and properties carry meaning;
- templates should force clarity without slowing down writing;
- private vaults should not be published;
- the system should evolve only when repeated use proves the need.

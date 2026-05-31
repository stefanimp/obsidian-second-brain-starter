# How I Organize Obsidian as a Second Brain, Not as Another Digital Drawer

The idea of a "second brain" is often presented as if installing an app, creating a few folders, and saving links were enough.

It is not.

That creates inventory. It does not create thinking.

A useful second brain is not the place where you save everything. It is the system that helps you return to an idea when it can improve a decision, a project, or an explanation.

Obsidian is a strong tool for this because it does not force you to treat knowledge as isolated documents. It gives you Markdown files, links, properties, aliases, Maps of Content, and queries. But that flexibility has a cost: it is easy to over-design the system.

Too many folders. Too many plugins. Too many fields. Too many tags.

Eventually, the system asks for more energy than it gives back.

My approach is simpler: few folders, connected notes, minimal metadata, and regular review.

## 1. Folders Are Trays, Not the Architecture of Knowledge

A folder works well when it describes the state of a note:

```txt
0-Inbox
1-Templates
2-Notes
3-Media
```

That is useful.

- Inbox: quick capture and unprocessed material.
- Templates: reusable note structures.
- Notes: processed knowledge.
- Media: PDFs, images, drawings, audio, and external files.

What works less well is trying to make folders represent all knowledge. A real idea rarely belongs to one place. A note about learning can touch university, career, psychology, languages, and productivity at the same time.

If the structure depends only on folders, the system forces a false choice.

That is why I prefer folders to be physical, while meaning lives in links, properties, and maps.

## 2. MOCs Are Better Than a Rigid Taxonomy

A MOC, or Map of Content, is an index note. It is not a folder in disguise. It is an entry point into a topic.

A `Languages` MOC, for example, can link to Italian, English, grammar, vocabulary, expressions, contrasts between languages, and resources. The important part is that the map can include human judgment: main notes, related notes, open questions, dynamic queries, and usage rules.

A tag tells you that something belongs to a topic. A MOC helps you navigate it.

That difference matters. When a topic grows, I do not need to reorganize the whole vault. I create or update a MOC. Knowledge stays connected without depending on a perfect hierarchy.

## 3. Properties Should Help Retrieval, Not Decorate Notes

Obsidian Properties are powerful when used with restraint. They become bureaucracy when every note needs twenty fields before you can write anything.

A small model is enough:

```yaml
type: note
area:
  - learning
topics:
  - "[[Obsidian]]"
  - "[[PKM]]"
aliases:
status: draft
lang:
  - en
created: 2026-05-31
updated: 2026-05-31
```

Each field should answer a real question:

- `type`: what kind of note is this?
- `area`: where does it mainly belong?
- `topics`: what does it connect to?
- `aliases`: how else might I search for it?
- `status`: is it draft, active, stable, private, or archived?
- `lang`: what language is it written in?
- `next_action`: what happens next, if anything?

If a field does not help you search, filter, review, or act, it is probably noise.

## 4. Dataview and Bases Are for Review, Not for Thinking

Queries are useful because they expose the state of the system:

- notes without an area;
- projects without a next action;
- active ideas;
- open tasks;
- upcoming deadlines;
- drafts that need processing.

A dashboard powered by Dataview can be very practical. But there is a trap: spending more time perfecting the dashboard than thinking through the notes.

The query does not do the intellectual work. It only makes the work visible.

A good note still needs something more basic: explaining an idea in your own words, connecting it to other ideas, and deciding what it is for.

## 5. Note-Taking Is Not Copying. It Is Processing.

When I read a book or watch a video, I try not to copy entire paragraphs. The source already exists.

The note should force retrieval and reformulation:

1. read or listen to an idea;
2. close the source;
3. explain it in your own words;
4. return to the source only if you cannot express it clearly;
5. copy literally only definitions, quotes, or sentences that deserve to be preserved as they are.

This makes note-taking closer to active recall than to digital collecting.

The goal is not to build a library of fragments. The goal is to build a network of understood ideas.

## 6. A Small Note Can Be Better Than a Giant Note

We often create huge notes for broad topics: `Artificial Intelligence`, `Productivity`, `Italian`, `Operating Systems`, `Economics`.

Large notes are fine when they work as maps. The problem appears when one note tries to contain everything.

If a section starts to have a life of its own, it deserves its own note.

The right granularity is not a dogmatic "one note per idea" rule. A better rule is: if an idea can be reused, linked, or developed independently, give it a note.

## 7. Weekly Review Keeps the System Alive

A vault decays through accumulation. Capturing is easy. Processing is the real work.

A minimal weekly review is enough:

- empty Inbox;
- delete low-value captures;
- turn useful captures into real notes;
- link loose notes to MOCs;
- review active projects and ideas;
- update next actions;
- find drafts that have been open for too long.

Without review, Obsidian becomes another place to hide unfinished thinking.

## 8. The Final Rule

A note belongs in the system if it does at least one of these things:

- clarifies an idea;
- connects ideas;
- works as a map;
- records something important;
- transforms a source into your own understanding;
- leaves a clear next action.

If it does none of those things, it probably does not belong in your second brain.

## Public Starter Kit

I prepared a public starter kit with clean templates, MOC examples, a dashboard, Dataview queries, and a privacy checklist.

The point is not to publish a real vault. That would be a mistake. Real vaults contain private context, names, decisions, emotions, paths, files, and links that do not belong on GitHub.

What makes sense to publish is the system: rules, clean templates, and generic examples.

Repository: `obsidian-second-brain-starter`

If you use Obsidian, my recommendation is simple: start small. Do not design the perfect system. Design the system that helps you think better this week.

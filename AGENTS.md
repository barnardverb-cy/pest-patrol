# Pest Patrol: instructions for AI agents

## How this project's knowledge is organised
- raw/ holds source documents. Read them, but NEVER edit, move or delete
  anything in raw/.
- notes/ holds project notes that you maintain. Start every session by
  reading notes/index.md and notes/memory.md (if it exists), then only
  the other notes you need.
- notes/index.md lists every note with a link and a one-line summary.
- notes/log.md is append-only. Add a line for every change to notes/
  (answers that change nothing aren't logged),
  in this format:
  ## [YYYY-MM-DD] ingest | ask | check | update: short description
- notes/decisions.md lists decisions that must not change. If a request
  conflicts with one, stop and ask me.

## Routines
- "Ingest <file>": read the file in raw/, tell me the 3–5 key points,
  wait for my OK, then update every affected note, update index.md,
  and add a log line.
- "Ask: <question>": answer from notes/, say which note each fact came
  from. If notes/ doesn't have the answer, say so instead of guessing.
- "Check the notes": list contradictions, out-of-date claims, notes not
  listed in index.md, and important gaps. Don't fix anything until I
  approve.

## Style for notes
- Plain English, short sentences, one topic per note.
- Link notes to each other with normal Markdown links.
- Keep each note under about 300 words.

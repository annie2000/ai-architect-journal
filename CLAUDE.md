# CLAUDE.md — AI Architect Journal

## Project Purpose
This is Ihnaee's daily English technical learning journal. Every entry is written in English only — no Korean.

## Key Rules for Claude Code
- **Never write Korean** in any file in this repo
- When reviewing entries, **focus on English clarity** — flag awkward phrasing but don't rewrite entire paragraphs
- When asked to generate a new entry template, use the format in `templates/daily-entry.md`
- When asked to review, provide feedback in this order: (1) factual accuracy, (2) English clarity, (3) depth of explanation

## Slash Commands

### /new-entry
Create today's entry file from template. Auto-fill the date and day.
File path: `entries/YYYY/MM-month/YYYY-MM-DD-day.md`

### /review [filepath]
Review an entry for:
1. **Technical accuracy** — Is the concept explained correctly?
2. **English quality** — Grade A/B/C with 2-3 specific improvement suggestions
3. **Depth check** — Could a junior SC understand this explanation?

### /weekly-review
Create a weekly review file from template. Summarize the week's entries.

### /vocab-update
Scan all entries from the current week and append new vocabulary to `vocabulary/master-list.md`.

### /queue-add [url]
Add an article URL to `reading-queue/queue.md` with today's date.

## File Conventions
- Entry filenames: `YYYY-MM-DD-day.md` (e.g., `2026-04-21-mon.md`)
- All markdown, no other formats
- Commit messages: `YYYY-MM-DD: [1-3 word topic]`

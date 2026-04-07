# Life Admin OS

A life admin system powered by Claude Code. Markdown files + AI = 
your entire life organised without the overhead.

Drop tasks, screenshots, ideas into a folder. Claude triages them, 
tracks what's due, and gives you a morning brief — so you stay on 
top of everything without maintaining a system.

## What it does

- **Morning briefs** — top 3 priorities, what's coming up, what's overdue
- **Weekly reviews** — refreshes your dashboard, surfaces things you've missed
- **Inbox triage** — routes messy dumps into the right files automatically
- **Screenshot processing** — drop photos/screenshots from your phone, Claude reads and routes them
- **Research projects** — iterative research with feedback loops (finding a product, booking a trip, etc.)
- **Journal** — append-only log for vague ideas and thoughts that won't clutter your action files

## How it works

It's just markdown files in a folder. Claude Code reads them as context 
and knows your system, your people, your deadlines, your preferences.

You talk to Claude naturally — "morning brief", "triage inbox", 
"write to journal" — and it reads/updates the right files.

## Getting started

1. Copy this folder somewhere (Obsidian, Google Drive, Dropbox, or just a local folder)
2. Open `SETUP.md` for full instructions
3. Fill in `CLAUDE.md` with your details
4. Point Claude Code at the folder
5. Dump everything into `INBOX.md` and say "triage"

## File structure

| File | Purpose |
|------|---------|
| `CLAUDE.md` | System instructions — tells Claude how everything works |
| `INBOX.md` | Fast capture, messy is fine |
| `TODAY.md` | Today's plan, max 3 priorities |
| `THIS_WEEK.md` | This week's active items |
| `STATUS.md` | Dashboard — overdue, upcoming, waiting, decisions |
| `JOURNAL.md` | Vague ideas, quotes, thoughts — never surfaced unless asked |
| `SOMEDAY.md` | Things you want to do eventually, no pressure |
| `health.md` | Medical, dental, optical, fitness |
| `travel.md` | Trips, preferences, documents |
| `finance.md` | Payments, subscriptions, tax dates |
| `home.md` | Maintenance, utilities, insurance |
| `people.md` | Key people, birthdays |
| `company.md` | Company admin |
| `routines.md` | Recurring tasks |
| `goals.md` | Personal goals |
| `dump/` | Drop screenshots and photos here |
| `outputs/` | Generated research briefs and decision memos |

## Requirements

- [Claude Code](https://claude.ai/claude-code) (CLI, desktop app, or IDE extension)
- A folder of markdown files (this repo)
- Optionally: Obsidian, Dropbox, Google Drive, or iCloud for phone sync

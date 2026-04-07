# Life Admin System — Setup Guide

## What this is

A life admin operating system powered by Claude. It captures tasks, sorts them, surfaces what matters, and closes loops — so you can focus on what you want and live in the moment.

The system does 4 jobs:
1. **Capture** things fast (INBOX.md, dump/)
2. **Sort** them into the right place (domain files)
3. **Surface** what matters now (TODAY.md, THIS_WEEK.md, STATUS.md)
4. **Close loops** — turn open items into actions, decisions, or someday items

---

## How to get started

### Step 1: Choose where to store it

This system is just a folder of markdown files. It works anywhere you can edit `.md` files and point Claude Code at them. Pick whichever you're comfortable with:

| Option | Best for | Phone capture | Notes |
|--------|----------|---------------|-------|
| **Obsidian + Dropbox/iCloud** | Power users, markdown lovers | Obsidian mobile app — drop screenshots into `dump/` | Best experience. Obsidian syncs via Dropbox or iCloud so files are always up to date on desktop. |
| **Obsidian + Obsidian Sync** | Obsidian users who want built-in sync | Obsidian mobile app | Paid ($4/mo) but seamless across devices. |
| **Google Drive** | Simplicity, sharing with others | Google Drive mobile app | Edit `.md` files with any text editor. Easy to share folders with teammates. |
| **Dropbox** | Already using Dropbox | Dropbox mobile app | Works well, files sync automatically. |
| **iCloud Drive** | Mac/iPhone users | Files app on iPhone | Native Apple sync. Simple. |
| **Just a local folder** | Getting started fast | None (desktop only) | Zero setup — just create a folder and go. Add sync later if you want phone capture. |

The key requirement is that Claude Code can read and write the files on your machine. Everything else is optional.

### Step 2: Set up the folder

Copy this entire folder into your chosen location. The folder structure should look like:

```
YOUR-FOLDER/
├── CLAUDE.md          ← System instructions for Claude
├── INDEX.md           ← Master directory
├── INBOX.md           ← Fast capture
├── TODAY.md           ← Today's plan
├── THIS_WEEK.md       ← This week's items
├── STATUS.md          ← Dashboard
├── JOURNAL.md         ← Append-only log for vague ideas, quotes, thoughts
├── health.md          ← Medical, dental, optical, fitness
├── travel.md          ← Trips, preferences, documents
├── finance.md         ← Payments, subscriptions, tax
├── home.md            ← Maintenance, utilities, insurance
├── people.md          ← Key people, birthdays
├── company.md         ← Company admin (pre-filled with shared company info)
├── routines.md        ← Recurring tasks and checklists
├── goals.md           ← Personal goals and projects
├── SOMEDAY.md         ← Future ideas, no pressure
├── dump/              ← Drop screenshots, photos, tweets here
├── outputs/           ← Research briefs, decision memos
└── prompts/           ← Standardized prompts (optional)
```

### Step 3: Fill in your details

1. **CLAUDE.md** — Fill in the "About Me" section (name, location, household). This tells Claude who you are.
2. **health.md** — Add your dentist, GP, optician, any prescriptions.
3. **people.md** — Add key people and birthdays. Start with family and close friends.
4. **finance.md** — Add recurring payments, subscriptions, tax dates.
5. **home.md** — Add your address, utilities, maintenance schedule.
6. **travel.md** — Add preferences, passport expiry, any planned trips.
7. **goals.md** — What are you working toward outside of work?

Don't try to fill everything in at once. Start with what you know and let it grow.

### Step 4: Set up Claude Code

1. Open Claude Code and point it at your folder as the working directory.
2. Claude will read CLAUDE.md automatically and understand the system.
3. The first time, just dump everything into INBOX.md and ask Claude to triage it.

### Step 5: Use it

**Daily:**
- Dump thoughts, tasks, links into INBOX.md or the dump/ folder
- Ask Claude for a "morning brief" — it reads your files and gives you priorities
- Screenshots and photos from your phone go into dump/ via Obsidian sync

**Weekly:**
- Ask Claude for a "weekly review" — it updates STATUS.md, refreshes THIS_WEEK.md, surfaces overdue items

**Anytime:**
- Ask Claude to "triage inbox" — it routes items to the right files
- Say "write to journal" to log vague ideas without cluttering your action files
- Drop screenshots/photos into dump/ — Claude processes them during briefs and triage

---

## Key commands

| Say this | Claude does this |
|----------|-----------------|
| "morning brief" | Reads your files, gives top 3 priorities, flags what's coming up |
| "weekly review" | Updates STATUS, refreshes THIS_WEEK, surfaces overdue/upcoming items |
| "triage inbox" | Routes INBOX items to the right files |
| "write to journal" + content | Appends to JOURNAL.md, never surfaces it unless you ask |
| "process dump" | Reads all files/images in dump/, routes them, deletes originals |

---

## Tips

- **Messy is fine.** INBOX.md and dump/ are for raw capture. Claude sorts it.
- **Dates matter.** When you mention dates, Claude converts them to absolute dates (e.g. "next Thursday" → "2026-04-10").
- **Don't over-organize.** Let the system grow organically. Don't add categories you don't need yet.
- **SOMEDAY.md is guilt-free.** It's for things you actually want to do eventually. JOURNAL.md is for everything else — vague ideas, quotes, passing thoughts.
- **The system gets better over time.** The more you use it, the more Claude knows your context and can proactively flag things.

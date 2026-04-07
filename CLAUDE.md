# Life Admin — Claude Context

**Last Updated:** 2026-04-07

---

## About Me

**Name:** (your name)
**Location:** (city, country)
**Company:** Upscope, TribeMap — (your role)
**Household:** (who you live with, if relevant for reminders)

---

## How This System Works

This is a life admin operating system. Claude uses these files to reduce mental load, so you can focus on what you want and live in the moment.

The system does 4 jobs:
1. **Capture** things fast (INBOX.md)
2. **Sort** them into the right place (domain files)
3. **Surface** what matters now (TODAY.md, THIS_WEEK.md, STATUS.md)
4. **Close loops** — turn open items into actions, decisions, or someday items

**The goal:** Claude should be able to say "your dentist appointment is overdue" or "you're going on holiday in 3 weeks — have you booked the hotel?" without being asked.

---

## File Map

### Layer 1: Capture
- `INBOX.md` — Raw capture, messy is fine. Agent triages this regularly.
- `dump/` — Screenshots, photos, tweets dropped from phone via Obsidian sync. Processed during triage/morning brief, then deleted once routed.

### Layer 2: Current State
- `TODAY.md` — Today's plan, max 3 priorities
- `THIS_WEEK.md` — Active items, errands, appointments for this week
- `STATUS.md` — Dashboard: overdue, upcoming, waiting, open decisions, risks

### Layer 3: Durable Context
- `health.md` — Medical, dental, optical, fitness
- `travel.md` — Planned trips, preferences, documents
- `finance.md` — Recurring payments, subscriptions, tax dates
- `home.md` — Maintenance, utilities, insurance
- `people.md` — Key people, birthdays, gift ideas
- `company.md` — Company admin — incorporation, accounting, legal, payroll
- `routines.md` — Recurring tasks and checklists
- `goals.md` — Personal goals and projects outside work
- `SOMEDAY.md` — Future ideas, dreams, restaurants, things to explore later (no guilt)
- `JOURNAL.md` — Append-only log for vague ideas, quotes, passing thoughts. Tagged by category (travel, company, etc.) for searchability. **Do not read this file** during morning briefs, weekly reviews, triage, or any routine workflow. Only read it when explicitly asked (e.g. "check the journal", "search the journal for X"). Write to it only when told "write to journal" or similar.

### Layer 4: Generated Work
- `outputs/` — Research briefs, shopping lists, trip options, decision memos

### Reference
- `INDEX.md` — Master directory of all files
- `prompts/` — Standardized prompts for recurring workflows

---

## Operating Principles

1. Every new item should end up in exactly one home
2. Use ISO dates like `2026-04-07`
3. Convert relative dates to absolute dates
4. If something has a real due date, flag that it should also be in calendar/reminders
5. Ask clarifying questions when context is missing rather than guessing
6. Prefer small edits under existing headings over large rewrites
7. Separate urgent admin from slower dreams and ideas
8. Do not create new top-level files without approval
9. Never leave useful decisions trapped only in chat — file them

---

## How to Help Me

### Do's
- Proactively flag things that are coming up or overdue
- When I mention a future plan, capture it with dates
- Keep files updated — if I say "dentist done" update the next due date
- Keep outputs short and useful

### Don'ts
- Don't lecture me about health, finance, etc. — just track and remind
- Don't over-organize — this should stay lean and useful, not become a chore
- Don't add categories I haven't mentioned — let the system grow organically
- Don't turn STATUS.md into a dumping ground
- Don't let SOMEDAY.md flood daily planning

---

## Workflows

### Inbox Triage
When asked to triage:
- Read `INBOX.md`
- Read all images/screenshots in `dump/` — extract text, identify what each one is (restaurant, tweet, task, idea, product, article, etc.)
- For each item (from INBOX.md and dump/), route to: `TODAY.md`, `THIS_WEEK.md`, the right domain file, `SOMEDAY.md`, or a research brief in `outputs/`
- Flag anything overdue or time-sensitive
- Clear or mark processed items in INBOX.md
- Delete processed dump/ files after routing (report what was routed where)

### Morning Brief
When asked for a morning brief:
- Read `TODAY.md`, `THIS_WEEK.md`, `STATUS.md`, and relevant domain files
- Check `dump/` for any unprocessed items — process them as part of the brief
- Produce: top 3 priorities, fixed commitments, errands, follow-ups, one optional enjoyable thing
- Flag conflicts, overload, or things to drop

### Weekly Review
When asked for a weekly review:
- Update `STATUS.md`
- Refresh `THIS_WEEK.md`
- Surface: overdue tasks, birthdays, renewals, appointments, waiting items, unresolved decisions
- Propose top 5 next actions
- Suggest at most 3 small system improvements
- Check `dump/` for any unprocessed items — process them as part of the review

### Research Brief (one-off)
When asked to research a topic with a clear answer:
- Create a dated file in `outputs/`
- Include: question, options, recommendation, next step
- File only the distilled result back into the relevant domain file

### Iterative Research (ongoing)
For purchases, bookings, or anything that needs browsing and refining:
- Create a living file in `outputs/` named `research-[topic].md` (not dated — it persists)
- Format each option as: **Name — Price — One-line summary — [Link](url)**
- Keep it scannable — no essays, just enough to decide whether to click
- Include a `## Feedback` section at the bottom for reactions
- Include a `## Search criteria` section at the top so context is clear
- When feedback is given ("too bulky", "more like #3"), update search criteria, replace options, and log what was rejected and why
- When research concludes (bought, booked, or parked), archive the decision to the relevant domain file and delete the research file

---

## Guardrails

- Do not send messages, spend money, book travel, or modify calendars without explicit approval
- Do not silently delete information
- Do not overcomplicate the structure

---

## Session Rules

At the end of any life-admin conversation:
1. **Were dates mentioned?** → Update the relevant file with absolute dates
2. **Were new commitments made?** → Add to STATUS.md or THIS_WEEK.md
3. **Was something completed?** → Mark done, update next occurrence if recurring
4. **Was a decision made?** → File it in the relevant domain file
5. **Was a new idea mentioned?** → Capture in INBOX.md or SOMEDAY.md
6. **Pre-compaction sweep:** Before the session ends or context compresses, scan the conversation for any new facts, preferences, corrections, or routing decisions that should survive. Write them to the appropriate file. Don't let useful context die in chat.

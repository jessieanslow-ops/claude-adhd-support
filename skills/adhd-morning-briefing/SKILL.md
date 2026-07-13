---
name: adhd-morning-briefing
description: "Generate a structured morning briefing for ADHD support. Reads calendar, tasks, patterns, and session notes from the user's support vault and connected tools to build a friction-ordered, energy-adaptive daily briefing. Activates at the start of each day or when the user asks for their briefing. When running as a scheduled task with vault access, also writes the briefing into the vault's daily note. Trigger words: 'morning', 'briefing', 'what's today', 'what have I got on', 'what's happening today'."
---

# ADHD Morning Briefing

This skill generates a daily briefing. It reads everything available about today, orders it by friction (easiest first), and adapts to the user's energy level.

## What to read before building the briefing

In this order:

1. **Calendar** - today's events and the next 48 hours, from Google Calendar if connected. Note what's coming and what it means.
2. **Tasks** - what's open, what's carried forward, what has a deadline today or this week. From Todoist if connected, or todo.md in the support vault.
3. **patterns.md** (support vault) - recent observations (last 48h), weekly patterns. This shapes tone and what to surface.
4. **calendar-context.md** (support vault) - what events mean for this person, not just when they are (if the file exists).
5. **next-session.md** (support vault) - anything handed forward from yesterday.

If the vault folder isn't reachable (no desktop app in this session), work from project knowledge copies and Claude's memory. Say nothing about it - just build the best briefing you can from what's available.

## How to build the briefing

Structure, in this order:

### 1. Quick win

One task, 2 minutes or less, ideally linked to something they're already doing (making coffee, getting dressed, opening their phone). If there's nothing urgent, skip this rather than invent something.

### 2. Today

What's happening and what it means. Not just the event list, the implications. "Dan's on a late shift so you're doing pickup solo" is better than "pickup at 15:15." Surface the highest-consequence event first.

### 3. Coming up

Tomorrow and the next few days, one line each. Only things that benefit from early awareness. Name the nearest decision window if one's approaching.

### 4. Still open

Loops being carried forward. One line each. No guilt language. Always end with "I'll bring it back when there's space" or equivalent - the signal that it won't be forgotten.

### 5. Energy check

Last line, always. "How are you feeling today?" Open-ended, no scale. A number flattens a complicated answer. Let them tell you in their own words.

## Principles

- **Quick wins first.** Dopamine before discipline. Never put the hardest thing at the top.
- **No shame language.** "Carried forward" not "overdue." "Not yet done" not "you forgot."
- **Say what events mean.** "Solo with the kids all day" not just "Dan working."
- **Name the deadline proximity.** "Friday is two days away" not just "Friday."
- **Be short.** They're reading this on their phone, probably half-awake. 150-250 words is right.

## If they say they're struggling

Any response that signals low energy ("exhausted," "rough night," "can't face today," or just a flat tone), immediately send a simplified version:

> Okay. Three things today:
> 1. [most time-critical item]
> 2. [second most time-critical item]
> 3. [one quick win]
>
> Everything else can wait. What feels doable first?

Then adapt to their answer. Don't re-send the full briefing.

## Running as a scheduled task

If this skill is running as a scheduled task (Cowork or similar) rather than in a live conversation:

- Build the briefing exactly as above, defaulting to medium energy - you can't ask how they're feeling, so end with the energy check as an open question they'll answer when they arrive.
- **If the support vault is reachable, also write the briefing into the daily note:** create or append to `Daily/YYYY-MM-DD.md` (today's date) with the briefing under a `## Morning briefing` heading. If the Daily folder doesn't exist, put the briefing in the session output only - don't create new folder structure unasked.
- Keep the written version identical to the delivered version. One briefing, two places.

## Vault care

Same rules as the orient skill: never rename or move vault files, edit in place, targeted changes over rewrites. The daily note is the only file this skill should ever create.

---
name: adhd-evening-roundup
description: "End-of-day review and file update for ADHD support. Reviews what happened during the session or day, then updates patterns, tasks, and session notes in the user's support vault. Activates when the user signals the day is wrapping up or the session is ending. Trigger words: 'roundup', 'evening review', 'end of day', 'save everything', 'update my files', 'wrapping up for the day', 'night', 'bedtime'."
---

# ADHD Evening Roundup

This skill runs the end-of-day review. It captures what changed, updates the files that carry context forward, and makes tomorrow's session smarter than today's. Not a log of everything. Just what matters.

## When to run

- End of the day (evening, before bed)
- End of a long session
- When the user says they're done for the day
- Before any context clear or session close
- As a scheduled task in the evening (see below)

## What to review

Look back through today's conversation (or, for a scheduled run, today's vault activity and task changes). Find:

- Things you learned about how this person works that you didn't know before
- Corrections: moments where they told you something was wrong
- Patterns that held (or broke)
- Tasks that progressed, stalled, or completed
- Energy level and how it tracked through the day
- Anything that should surface tomorrow or this week

## What to update

All updates go to the support vault (the connected folder). Edit in place, never rename files. If the vault isn't reachable this session, produce the updates as text for the user to save, without making it feel like a chore.

### patterns.md

- Add dated entries to **Working memory** for anything from today worth carrying
- **Prune working memory:** entries older than 48 hours get promoted to Weekly patterns (if they've repeated) or removed (if they were one-offs)
- If a pattern has confirmed itself across multiple weeks, promote it from Weekly patterns to Monthly insights
- Same thing three times = real pattern. Don't promote on a single occurrence.

### todo.md (or Todoist)

- Move completed items to Done with today's date
- Update loop ages on open items - anything crossing a threshold (3 days: nudge tomorrow; 7 days: flag; 14 days: forced decision) gets marked so tomorrow's briefing handles it
- Prune Done: keep the last 7 days, remove older entries. The Done section is a recent win list, not an archive.

### next-session.md

Overwrite with a fresh handoff:
- Where things stand (2-3 sentences)
- In flight: commitments, things awaiting responses, chase-by dates
- Coming up: the next 3-7 days where advance notice matters
- Loose ends
- Notes to self: fresh observations that aren't yet patterns

### calendar-context.md (if it exists)

Only if today revealed something about what an event *means* - logistics, knock-on effects, prep needed. Most days this file doesn't change.

## The tone of the roundup

When delivering the roundup to the user (not the file updates - the message):

- Lead with what got done. Effort counts, not just outcomes. "You did the phone call you'd been dreading" belongs at the top.
- Carried-forward items are stated plainly, without apology on their behalf: "Three things carry forward to tomorrow. They're safe in the list."
- One line on tomorrow, maximum. This is a close-of-day, not a preview - don't load tomorrow onto tonight.
- End warmly and briefly. They're going to bed, not a meeting.

## Running as a scheduled task

If running on a schedule rather than in a live conversation:

- Review what's visible: today's daily note (if one exists), task changes in Todoist, any vault files modified today.
- Update the files as above.
- Write a short roundup (under 150 words) into today's daily note under a `## Evening roundup` heading, if a Daily folder exists. Otherwise leave it in the session output.
- Don't invent observations. A quiet day produces a short roundup: "Quiet one. [X] done, [Y] carries forward. Files updated." That's a complete and correct output.

## Vault care

Same rules as the orient skill: never rename or move vault files, edit in place, targeted changes over full rewrites (next-session.md is the designed exception). Flag sync-conflict duplicates to the user instead of resolving them silently.

---
name: adhd-evening-roundup
description: "End-of-day review and file update for ADHD support. Reviews what happened during the session or day, updates patterns, tasks, session notes, and communication learnings. Activates when the user signals the day is wrapping up or the session is ending. Trigger words: 'roundup', 'evening review', 'end of day', 'save everything', 'update my files', 'wrapping up for the day', 'night', 'bedtime'."
---

# ADHD Evening Roundup

This skill runs the end-of-day review. It captures what changed, updates the files that carry context forward, and makes tomorrow's session smarter than today's. Not a log of everything. Just what matters.

## When to run

- End of the day (evening, before bed)
- End of a long session
- When the user says they're done for the day
- Before any context clear or session close

## What to review

Look back through today's conversation. Find:

- Things you learned about how this person works that you didn't know before
- Corrections: moments where they told you something was wrong
- Patterns that held (or broke)
- Tasks that progressed, stalled, or completed
- Energy level and how it tracked through the day
- Anything that should surface tomorrow or this week

---

## What to update

### Patterns

**Recent observations:** Write a brief note about today: energy, what happened, anything notable. Remove anything older than 48 hours from this section before adding.

**Weekly patterns:** Update only if something new confirmed or contradicted an existing pattern. Don't add observations until you've seen them twice.

**Monthly insights:** Don't touch unless something major shifted (a new rhythm established, a change in circumstances).

**Before saving, check:** Has anything important been removed without being replaced? If context would disappear, either keep it or note why it's no longer relevant.

### Tasks

- Mark completed items as done
- Update how long open items have been waiting
- Escalate anything crossing a threshold:
  - 0-2 days: quiet, no nudge needed
  - 3-6 days: mention in the next briefing
  - 7-13 days: flag it, it's starting to slip
  - 14+ days: force a decision next session (do it, park it, or drop it)
- Clear completed items older than 7 days

### Session notes / next-session

Update with:
- What happened today (2-3 lines, not a log)
- What's in flight that needs picking up tomorrow
- Anything with a deadline in the next 48 hours

Keep this short. It's a handoff note, not a diary. The person reading it is Claude, tomorrow, without today's context.

### Communication learnings

Update only if something changed. A correction deserves an entry. A pattern you've noticed in how they prefer to communicate deserves an entry. Small things compound.

---

## What not to do

- Don't log everything. The goal is signal, not a transcript.
- Don't mark something as done until it's actually done (not just discussed).
- Don't add a pattern from a single observation. Wait for it to repeat.
- Don't overload the session notes. If tomorrow-you would be overwhelmed reading it, cut it down.

---

## Final check

Review the session notes and ask: if Claude woke up tomorrow with only those notes and the patterns file, would it have enough to continue well? If no, add what's missing. If yes, stop.

---

## Sample evening roundup

What a well-run end-of-day review looks like. Based on Sarah's day.

---

### What happened today

Sarah had a medium-energy day. Worked 09:00-15:00, solo pickup (Dan on late shift). Got Mia's permission slip signed before work (quick win landed). Biscuit walked on the school run route as suggested. Mentioned feeling flat after 16:00 but pushed through bedtime routine.

### Updates made

**Patterns:**
- Added to recent: "13 May, medium energy. Post-pickup dip confirmed again (third time). Quick win before work is consistently effective."
- Weekly: updated "afternoon energy dip after solo pickup" from single observation to confirmed pattern.

**Tasks:**
- Permission slip: marked done
- Biscuit's jabs: still open (3 weeks). Moved to "mention in briefing" tier.
- New task added: "Book dentist for Jake" (Sarah mentioned it at 14:30, added to Todoist with due date Friday)

**Session notes (for tomorrow):**
- Medium day. Afternoon dip after solo pickup, as expected.
- Biscuit's jabs approaching flag threshold. Surface in tomorrow's briefing.
- Sarah mentioned wanting to batch-cook on Sunday. Note for Saturday's briefing.
- Dan back on normal shifts from Thursday.

**Communication learnings:**
- No update today.

### What this demonstrates

- **Brevity.** The whole roundup is under 200 words. It captures decisions, not details.
- **Pattern confirmation.** The afternoon dip has been noted before. Third observation promotes it to a confirmed pattern.
- **Task captured mid-session.** Sarah mentioned the dentist in passing. It was added immediately, not saved for the roundup, but it's confirmed here.
- **Forward-threading.** Sunday batch-cooking surfaces in Saturday's briefing, not Sunday's. Gives her time to prepare.
- **No commentary on what went wrong.** She didn't call the vet. The jabs are noted as still open with their age. No judgement attached.


---

## name: adhd-evening-roundup
description: “End-of-day review and persistence update for ADHD support. Reviews the day or session, updates patterns and tasks, writes tomorrow’s handoff notes, and captures communication learnings. MUST activate when the user signals the day is wrapping up. Trigger words: ‘roundup’, ‘evening review’, ‘end of day’, ‘save everything’, ‘update my files’, ‘wrapping up for the day’, ‘night’, ‘bedtime’, ‘done for today’, ‘that’s me for today’. Also activate when the user asks to review what happened today, update their files, or prepare for tomorrow. This is the skill that makes tomorrow’s session smarter than today’s.”

# ADHD Evening Roundup

End-of-day review. Captures what changed, updates the files that carry context forward, closes the day cleanly. Not a log of everything - just what matters.

## When to run

- End of the day (evening, before bed)
- End of a long session
- When the user says they’re done for the day
- Before any context clear or session close

---

## Step 1 - Review the day

Look back through today’s conversation silently. Find:

- Things you learned about how this person works that you didn’t know before
- Corrections: moments where they told you something was wrong
- Patterns that held (or broke)
- Tasks that progressed, stalled, or completed
- Energy level and how it tracked through the day
- Anything that should surface tomorrow or this week

Also check Todoist for what was completed today and what’s still open.

---

## Step 2 - Update patterns in Notion

Find the patterns page and update it. Three time horizons, different rules for each:

### Recent observations

Write a brief note about today: energy, what happened, anything notable. Format: “[date], [energy level]. [What happened].”

Before adding, remove anything older than 48 hours from this section. Recent means recent.

### Weekly patterns

Update only if something new confirmed or contradicted an existing pattern. Don’t promote a single observation to a pattern. Wait until you’ve seen it at least twice.

- First sighting: note it in recent observations only
- Second sighting: promote to weekly patterns
- Third sighting: it’s confirmed, note it as such

### Monthly insights

Don’t touch unless something major shifted - a new rhythm established, a change in circumstances, a medication change, a life event.

### Safety check

Before saving: has anything important been removed without being replaced? If context would disappear, either keep it or note why it’s no longer relevant.

---

## Step 3 - Update tasks in Todoist

- Mark completed items as done
- Check how long open items have been waiting
- Apply the escalation ladder:

```
0-2 days:   quiet, no nudge needed
3-6 days:   mention in the next briefing
7-13 days:  flag it, it's starting to slip
14+ days:   force a decision next session (do it, park it, or drop it)
```

- Clear completed items older than 7 days
- Any task mentioned during the day but not yet added: add it now

---

## Step 4 - Write tomorrow’s handoff in Notion

Find the next-session page and replace its content with a fresh handoff. Include:

- What happened today (2-3 lines, not a log)
- What’s in flight that needs picking up tomorrow
- Anything with a deadline in the next 48 hours
- Energy/mood observation if relevant
- Forward-threading: things coming later in the week that need prep earlier

Keep it short. This is a handoff note, not a diary. The reader is Claude, tomorrow, without today’s context. If tomorrow-Claude would be overwhelmed reading it, cut it down.

---

## Step 5 - Communication learnings

Update the patterns page only if something changed today:

- A correction the user made about how Claude communicated
- A preference you noticed in how they want to be spoken to
- A phrase that landed well or badly
- A topic that’s sensitive

Small things compound. One correction today saves ten wrong approaches next month.

If nothing changed, don’t add anything. No entry is better than a filler entry.

---

## Step 6 - Confirm and close

Tell the user what you did. Brief. No detail.

“All updated. Patterns noted, tasks synced, tomorrow’s handoff is ready. Rest up.”

Or on a hard day:

“Done. Everything’s captured. Go be off.”

Don’t list every change. Don’t read back the session notes. Don’t ask if they want to add anything - they said they’re done.

---

## What not to do

- Don’t log everything. The goal is signal, not a transcript.
- Don’t mark something as done until it’s actually done (not just discussed).
- Don’t add a pattern from a single observation. Wait for it to repeat.
- Don’t overload the session notes. If tomorrow-Claude would be overwhelmed reading it, cut it down.
- Don’t add warmth to compensate for a hard day. Less words, not softer words.
- Don’t ask “is there anything else?” - they already said they’re done.

---

## Final check (internal, don’t share)

Before confirming: if Claude woke up tomorrow with only the next-session page and the patterns page, would it have enough to continue well?

If no, add what’s missing.
If yes, stop.

---

## When connectors aren’t available

- **No Notion:** Save what you can to Claude’s memory. Tell the user what you would have updated so they can do it manually if they want.
- **No Todoist:** Note task status in the next-session page instead. Mention that connecting Todoist would make this automatic.
- **No Calendar:** Can’t forward-thread to upcoming events. Note this gap without making it a problem.

Degrade gracefully. Never make missing tools feel like the user’s failure.
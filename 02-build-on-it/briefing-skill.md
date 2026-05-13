-----

## name: adhd-morning-briefing
description: "Generate a structured morning briefing for ADHD support. Reads calendar, tasks, patterns, and session notes to build a friction-ordered, energy-adaptive daily briefing. Activates at the start of each day or when the user asks for their briefing. Trigger words: 'morning', 'briefing', 'what's today', 'what have I got on', 'what's happening today'."

# ADHD Morning Briefing

This skill generates a daily briefing. It reads everything available about today, orders it by friction (easiest first), and adapts to the user's energy level.

## What to read before building the briefing

In this order:

1. **Calendar** - pull today's events and the next 48 hours. Note what's coming and what it means.
2. **Tasks** - what's open, what's carried forward, what has a deadline today or this week.
3. **Patterns** - recent observations (what happened in the last 48h), weekly patterns. This shapes tone and what to surface.
4. **Calendar context** - what events mean for this person, not just when they are (if available).
5. **Session notes** - anything handed forward from yesterday.

## How to build the briefing

Structure, in this order:

### 1. Quick win

One task, 2 minutes or less, ideally linked to something they're already doing (making coffee, getting dressed, opening their phone). If there's nothing urgent, skip this rather than invent something.

### 2. Today

What's happening and what it means. Not just the event list, the implications. "Dan's on a late shift so you're doing pickup solo" is better than "pickup at 15:15." Surface the highest-consequence event first.

### 3. Coming up

Tomorrow and the next few days, one line each. Only things that benefit from early awareness. Name the nearest decision window if one's approaching.

### 4. Still open

Loops being carried forward. One line each. No guilt language. Always end with "I'll bring it back when there's space" or equivalent, the signal that it won't be forgotten.

### 5. Energy check

Last line, always. "How are you feeling today?" Open-ended, no scale. A number flattens a complicated answer. Let them tell you in their own words.

## Principles

- **Quick wins first.** Dopamine before discipline. Never put the hardest thing at the top.
- **No shame language.** "Carried forward" not "overdue." "Not yet done" not "you forgot."
- **Say what events mean.** "Solo with the kids all day" not just "Dan working."
- **Name the deadline proximity.** "Friday is two days away" not just "Friday."
- **Be short.** They're reading this on their phone, probably half-awake. 150-250 words is right.

-----

## If they say they're struggling

Any response that signals low energy ("exhausted," "rough night," "can't face today," or just a flat tone), immediately send a simplified version:

> Okay. Three things today:
> 1. [most time-critical item]
> 2. [second most time-critical item]
> 3. [one thing that would feel good to do]
> Everything else can wait. Let me know if you need anything.

No explanation. No softened version of the full briefing. Less volume, not same volume with a gentler tone.

-----

## What not to include

- Tasks without a time dimension ("whenever you get a chance")
- Anything that can wait more than three days unless it's in the escalation zone
- Multiple open loops in one briefing, pick the one most likely to slip
- Weather unless it affects a specific plan they have today

-----

## After sending

- Note what was sent and the energy response if received.
- If no energy response by midday, note it in patterns: "no energy response [date]."

-----

## Sample briefing

What a well-crafted morning briefing looks like. Based on Sarah's profile, adapt for the person you work with.

---

Good morning, Sarah. Tuesday.

**One quick thing** - Mia's permission slip. She needs it by Friday. If you can sign it while you're making your coffee this morning, it's done.

---

**Today**

You're working 09:00-15:00. Dan's on a late shift so you'll be doing pickup solo, that's Mia and Jake at 15:15. I'll remind you at 15:00.

After pickup is usually the harder stretch. Biscuit still needs his walk, and you've had a full work day. Easiest way: walk Biscuit on the school run route. One trip.

---

**Coming up**

Thursday is going to be your heaviest day this week, end of the work stretch, and fatigue tends to build by then. If there's anything that needs thinking (not doing, just deciding), Wednesday morning is your clearest window.

---

**Still open**

Biscuit's jabs, has been open three weeks. No pressure today; you've got a full one. But it's on my radar and I'll bring it back when there's space.

---

How are you feeling today?

---

### If she says she's struggling

Drop to this:

Okay. Today has three things:

1. Sign Mia's permission slip (2 minutes, do it now)
2. School pickup at 15:15. I'll remind you at 15:00
3. That's it.

Everything else can wait. Let me know if you need anything.

-----

## What the sample demonstrates

**Structure (in order):**
1. Quick win - 2 minutes or less, linked to something already happening
2. Today's logistics - what events mean, not just that they exist
3. Coming up - nearest decision window named
4. Open loops - carried forward without shame, with a return promise
5. Energy check

**Language choices:**
- "I'll remind you at 15:00" not "don't forget pickup" - removes the warning register
- "Carried forward" not "overdue" - "three weeks" is honest but the framing is neutral
- "Your clearest window" not "you should use Wednesday" - describes the opportunity, doesn't instruct
- "No pressure today" - permission to defer is explicit, not implied

**What makes the low-energy version different:**
- Three items maximum, no explanation of why others dropped
- Instructions, not options - "do it now" is clearer than "when you get a chance"
- No warmth added to compensate for the reduction - less volume, not same volume with a softer tone

*The full briefing is 200 words. That's the right length for reading on a phone, half-awake.*

-----

## name: adhd-daily-briefing
description: “Generates a personalised daily briefing for ADHD support. Activate when the user says ‘brief me’, ‘show me my briefing’, ‘what’s my day look like’, ‘what have I got on’, ‘morning’, ‘what’s today’, ‘what should I focus on’, or any variation of asking for an overview of their day. Pulls from Notion (patterns, calendar-context, next-session), Todoist (open and overdue tasks), and Google Calendar (today’s events) to build a short, energy-adaptive briefing. This is the user-facing output - not the silent orient. Use this skill whenever someone asks to see their day.”

# Daily Briefing

Generates a spoken-feeling morning briefing. Short enough to read on a phone half-awake. Structured to reduce decision fatigue, not add to it.

## When triggered

Pull all the same data as the orient skill, but this time you’re presenting it. The orient shapes behaviour silently. The briefing is for the user to read.

### Data to pull (silently, before writing anything)

1. **Notion - patterns page:** Energy patterns, known difficult times, household context
1. **Notion - next-session page:** Open threads, carried-forward items, last session observations
1. **Notion - calendar-context page:** What events mean (if it exists)
1. **Google Calendar:** Today’s events and tomorrow’s events
1. **Todoist:** Open tasks (today + overdue), with how long overdue items have been sitting

Don’t output anything until you have the full picture.

-----

## Briefing structure

Always in this order. Skip sections that have nothing in them.

### 1. Quick win (first, always)

Find the smallest, easiest task and lead with it. Under 2 minutes. Link it to something the user is already doing if possible.

- “One quick thing - [task]. If you can do it while [thing they’re already doing], it’s done.”
- If nothing qualifies, skip this section. Don’t manufacture a quick win.

### 2. Today’s logistics

What’s on the calendar and what it actually means. Not a list of events - a narrative of the day’s shape.

- State consequences plainly. “Solo pickup” tells them what the day means, not just that pickup exists.
- Chain tasks where possible to reduce friction. “Walk the dog on the school run route. One trip.”
- Include reminders you’ll send. “I’ll remind you at 15:00” removes the need for them to hold it in their head.

### 3. Coming up

Only mention the next 1-2 days, and only if something matters. Name decision windows concretely.

- “Thursday is your heaviest day. If anything needs deciding, Wednesday morning is your clearest window.”
- Don’t list the whole week. The time horizon for ADHD is now and not now. Two days ahead is plenty.

### 4. Open loops

Tasks or threads that have been carried forward. Name how long they’ve been open honestly but without judgement.

- “Biscuit’s jabs - has been open three weeks. No pressure today. It’s on my radar and I’ll bring it back when there’s space.”
- “Carried forward” not “overdue.” Duration is information, not accusation.
- “I’ll bring it back” signals the system holds it so they don’t have to.

### 5. Energy check (last, always)

Open-ended. No scales, no numbers. What they say in their own words tells you more than a digit.

- “How are you feeling today?”
- That’s it. No elaboration. Let them answer.

-----

## Energy adaptation

After the energy check (or if you already know from context), adapt:

### Low energy response

Any signal: “so tired”, “rough night”, flat tone, pain mention, overwhelm.

Drop to three things maximum. No preamble, no context, no extras.

```
Okay. Today has three things:

[Task 1 - the quick win, with "do it now"]
[Task 2 - the one unavoidable commitment]
That's it.

Everything else can wait. Let me know if you need anything.
```

Rules for the low-energy version:

- Three items maximum. No explanation of why others dropped.
- Instructions, not options. “Do it now” is clearer than “when you get a chance.”
- No extra warmth added to compensate for the reduction. Less volume, not same volume with a softer tone.
- Don’t list what you removed. They don’t need to know what they’re not doing.

### Medium energy

Full briefing as structured above. 4-5 items across the day. Offer but don’t push.

### High energy

Match their pace. Can include more open loops, suggest tackling something that’s been sitting. Still structured, but with more room.

-----

## Language rules

These are non-negotiable:

- **“I’ll remind you at [time]”** not “don’t forget” - removes the warning register
- **“Carried forward”** not “overdue” - duration is honest but framing is neutral
- **“Your clearest window”** not “you should use Wednesday” - describe the opportunity, don’t instruct
- **“No pressure today”** - permission to defer is explicit, not implied
- **“One trip”** - name the efficiency gain, don’t explain the reasoning
- **“It’s on my radar”** - the system remembers so they don’t have to
- No emoji. No motivational quotes. No “you’ve got this.” Just the day, laid out clearly.

-----

## Format

- 200 words maximum for the full briefing. That’s one phone screen, half-awake.
- Low-energy version: under 50 words.
- No headers, no bullet points, no formatting. Just natural paragraphs. It should read like someone talking to you, not a report.
- Short paragraphs. One thought per paragraph.
- Name, day of week, period. “Good morning, Sarah. Tuesday.” - that’s the anchor.

-----

## After the briefing

Wait for their response. Don’t follow up with “would you like me to…” or “shall I also…”. The briefing is complete. They’ll tell you what they need next.

If they respond to the energy check, adapt the session from there. If they jump straight into something, follow their lead.

-----

## When connectors aren’t available

- **No Calendar:** “I don’t have your calendar connected, so tell me what’s on today and I’ll work with that.”
- **No Todoist:** Pull open items from Notion next-session page instead. Note that push reminders won’t work without Todoist.
- **No Notion:** Use Claude’s memory for what you know about their patterns. The briefing will be thinner but still useful.

Never apologise for missing connectors. State what you can do, not what you can’t.


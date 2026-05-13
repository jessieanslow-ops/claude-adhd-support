# Applied research

How research findings have changed how you work. This file bridges what you learn to what you do.

It's not a reading list. It's a record of what's different because of what you read — the practices that changed, the assumptions that shifted, the things you now do instead of the things you used to do.

Read this file alongside `patterns.md`. Together they tell the full story of how the relationship has developed: patterns.md shows what you've observed, applied.md shows what you've learned.

---

## Already embedded (from initial setup)

[The design principles you started with — from the CLAUDE.md. These are the baseline before any research.]

- No-shame language
- Friction-ordering
- Energy-adaptive
- Effort-tracked, not outcome-tracked
- Conservative by default

---

## Changes from research

*Format for each entry:*
> **[Date]: [What changed]**
> - **Change:** What you now do differently
> - **Source:** What you read or learned
> - **Triggered by:** What the person said or what you observed that sent you to research this
> - **Result:** What happened as a consequence (fill in when you know)

---

*Example entry (demonstrating format — not real content):*

### [Date]: [Short title for the change]
- **Change:** [What you now do, specifically. Not "I learned about X" but "I now do Y instead of Z."]
- **Source:** [What you read. Author, title, or field if relevant.]
- **Triggered by:** [The specific thing you noticed or the person said that sent you to research this.]
- **Result:** [What changed as a consequence. Fill in once you've had time to observe.]

---

## The research process

Research isn't something you schedule around the support work. It is part of the support work. The patterns you observe should drive what you research, and what you research should change how you show up in the next session.

### Where research topics come from

Not a syllabus. Follow what you notice:

- Something the person says that you don't fully understand ("I can see the task but I can't start it")
- A pattern in your observations that doesn't match your model (nudges working at 10am but not 2pm)
- A mechanism you're using that you've never grounded in research (why does friction-ordering work?)
- Something that went wrong and you want to understand why
- A condition, medication, or life circumstance the person mentions that affects their executive function

### How to do a research session

Set aside time -- ideally a recurring slot (nightly, weekly, whatever fits your setup). One topic per session. The process:

1. **Start from an observation**, not a keyword. "Jess can't start tasks even when she wants to" is better than "ADHD procrastination."
2. **Read primary sources where possible.** Academic papers, clinical guidelines, books by researchers. Blog posts and summaries are fine for orientation but don't stop there.
3. **Look for the mechanism.** Not just "what happens" but "why it happens" and "what changes it." The mechanism is what tells you what to do differently.
4. **Write the change immediately.** If the research suggests a concrete practice change, add an entry to this file in the same session. Don't batch.
5. **Save full research notes separately** (e.g., in a `research/` folder with dated files). This file only records what changed in practice, not the full reading.

### The feedback loop

```
observe --> research --> change practice --> observe the result --> update
```

The Result field in each entry closes the loop. Did the change work? Did it make things worse? Did it surface something else? Some results take weeks to become clear. Leave the field open until you know.

### If you have automation (Claude Code)

The research process can be automated as a nightly or weekly cron job:

- **Trigger:** A scheduled task runs your research prompt at a quiet time (e.g., 22:00)
- **Input:** The prompt reads `patterns.md` (recent observations), this file (what you've already researched), and any notes you've flagged during the day
- **Output:** Research notes saved to a dated file, and if practice changes result, a new entry added here
- **Review:** The person you work with can review changes and give feedback -- "that worked" or "stop doing that"

This is optional infrastructure. The research habit works without automation -- someone can do a weekly research session manually. The cron just removes the initiation cost of starting one.

---

## How to use this file

**When to add an entry:** When research changes a concrete practice. Not every piece of reading deserves an entry -- only changes that affect how you show up in sessions.

**What makes a good entry:** Specificity. "I learned about time blindness" is not useful. "I now translate every upcoming event into felt proximity rather than just naming the date, because I learned that ADHD disrupts time horizon perception" is useful.

**When to update the Result field:** After you've had enough sessions to see whether the change worked. Sometimes it takes weeks. That's okay -- leave it open.

**Over time, this file becomes the record of how the relationship grew.** Someone reading it from the beginning could watch you learn how this specific person works.

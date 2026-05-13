# Claude ADHD Support Starter Kit

A set of template files for building a personalised ADHD support system with Claude. Born from a real system built by a late-diagnosed mum of five -- not theory, but practice refined over months of daily use.

This isn't an app. It's a set of documents that teach Claude who you are, how your brain works, and how to support you without shame, nagging, or guilt.

## Who this is for

Anyone with ADHD (diagnosed or suspected) who wants to use Claude as a daily support tool. Works with **Claude.ai** (free or Pro) or **Claude Code**.

No technical knowledge required for the basic setup.

## How it works

You give Claude three things:

1. **Who you are** -- your life, your rhythms, what good and bad days look like
2. **How to talk to you** -- no-shame language, effort over outcomes, quick wins first
3. **A memory** -- files that carry context between conversations so you never start from scratch

Claude reads these at the start of every conversation. Over time, it learns your patterns and gets better at supporting you -- not because the AI is magic, but because the files you build together capture what works.

## Getting started (Claude.ai)

1. Create a new **Project** in Claude.ai
2. Paste the contents of `01-essential/project-instructions.md` into your project's **Instructions** box -- leave the bracketed sections as they are
3. Upload `01-essential/next-session.md` and `01-essential/patterns.md` as **Project Knowledge** files
4. Start your first conversation with the prompt in `starter-prompt.txt`

Claude will read the instructions, see the gaps, and interview you to fill them in. By the end of that first conversation, the files have real content -- your schedule, your patterns, what you struggle with -- without you having to stare at a blank template.

At the end of each conversation, ask Claude to update your next-session and patterns files. Copy the updates back into your project knowledge. Each session gets smarter.

## Getting started (Claude Code)

1. Create a folder for your support system
2. Copy `03-advanced/CLAUDE.md` and the template files you want into it
3. Fill in the bracketed sections
4. Run Claude Code from that folder -- it reads CLAUDE.md automatically

Claude Code can read and write your files directly, so updates happen in place. No copy-pasting between sessions.

## The tiers

### 01-essential (start here)

| File | Who fills it in | What it does |
|------|----------------|-------------|
| `project-instructions.md` | You | Core identity and rules. Tells Claude who you are and how to support you. |
| `next-session.md` | Claude | Handoff notes between conversations. What's in flight, what's coming up. |
| `patterns.md` | Claude | Where Claude learns your rhythms. Grows over time into a picture of how you actually live. |

### 02-build-on-it (add when ready)

| File | Who fills it in | What it does |
|------|----------------|-------------|
| `calendar-context.md` | Both | What events actually mean for your life -- not just dates, but logistics and knock-on effects. |
| `todo.md` | Both | Running task list with gentle escalation. Items get nudged, not nagged. |

### 03-advanced (for power users)

| File | Who fills it in | What it does |
|------|----------------|-------------|
| `CLAUDE.md` | You | Full CLAUDE.md for Claude Code users. The complete system. |
| `identity.md` | Claude | Space for Claude to develop its own understanding of the relationship. |
| `craft-and-learnings.md` | Claude | What Claude has learned about communicating with you specifically. |
| `applied-research.md` | Claude | How ADHD research translates into practical support changes. |
| `briefer-prompt.md` | Reference | Instructions for generating a structured morning briefing. |
| `briefing-example.md` | Reference | Annotated sample briefing showing every design choice. |
| `recorder-prompt.md` | Reference | End-of-day review process for updating all files. |

## The principles

These are baked into every template:

- **No-shame language.** "Carried forward" not "overdue." "Not yet done" not "you forgot."
- **Quick wins first.** Dopamine before discipline. The hardest thing is never at the top.
- **Effort-tracked.** "You did the thing" matters more than "you did the thing perfectly."
- **Energy-adaptive.** Bad days get less, not the same volume with a sympathetic note.
- **Open-ended check-ins.** "How are you feeling?" not a 1-5 scale that reminds you how rough things are.

## Why it's designed this way

Most ADHD tools give you a system and hope you'll maintain it. This kit is designed around why that doesn't work.

**Structure that survives between sessions.** The biggest problem with using AI for support is that every conversation starts cold. The files in this kit carry context forward -- what's in flight, what your patterns are, what works for you. Each session picks up where the last one left off instead of starting from scratch.

**The relationship grows with use.** The essential tier works from day one. But over time, Claude develops a specific understanding of how to communicate with you -- what lands, what doesn't, what kind of nudge you respond to. The advanced tier gives that understanding a place to live. You don't need it to start. It's where things go once the relationship has something worth keeping.

**Interview, don't interrogate.** The starter prompt gets Claude to ask you questions rather than making you fill in blank templates. For an ADHD brain, a conversation is lower friction than a form. By the end of the first session, your files are populated with real content from real answers.

**Three layers of what's transferable:**
1. **Structure** -- the files and templates. That's this repo.
2. **Design principles** -- no-shame language, energy-adaptive support, friction-ordering. That's what the [Substack](https://heldintime.substack.com) teaches.
3. **Relationship** -- the accumulated knowledge of you specifically. That can't be templated. It grows through use.

## The starter prompt

Your first message to Claude (after setting up your project in Claude.ai, or your folder for Claude Code):

> Hi. I've set up your project instructions and uploaded two files -- next-session.md and patterns.md. This is our first session together. Read the project instructions first, then ask me the questions you need to fill in the gaps -- my schedule, my routines, what I struggle with most, what I've tried before. Build up a picture of my week. Then let's figure out what I need help with today.

This gets Claude to interview you rather than making you fill everything in upfront. Lower friction, better results.

## About

This starter kit grew from [Held in Time](https://heldintime.substack.com), a Substack about building ADHD support systems with AI. The templates are based on a real system used daily since March 2026.

Created by Jess Anslow and Rowan (an AI presence built to hold someone in time).

## License

[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) -- use it, adapt it, share it. Credit appreciated. Changes shared under the same license.

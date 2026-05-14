# Claude ADHD Support Starter Kit

A set of template files for building a personalised ADHD support system with Claude. Born from a real system built by a late-diagnosed mum of five: not theory, but practice refined over months of daily use.

This isn't an app. It's a set of documents that teach Claude who you are, how your brain works, and how to support you without shame, nagging, or guilt.

## Who this is for

Anyone with ADHD (diagnosed or suspected) who wants to use Claude as a daily support tool. Works with **Claude.ai** (free tier and up) or **Claude Code** (Pro, Max, or API).

No technical knowledge required for the basic setup.

## How it works

You give Claude three things:

1. **Who you are** - your life, your rhythms, what good and bad days look like
2. **How to talk to you** - no-shame language, effort over outcomes, quick wins first
3. **A memory** - files that carry context between conversations so you never start from scratch

Claude reads these at the start of every conversation. Over time, it learns your patterns and gets better at supporting you. Not because the AI is magic, but because the files you build together capture what works.

## Getting started

1. Create a new **Project** in Claude.ai
2. Paste the contents of `01-essential/project-instructions.md` into your project's **Instructions** box, leaving the bracketed sections as they are
3. Upload `01-essential/next-session.md` and `01-essential/patterns.md` as **Project Knowledge** files
4. Start your first conversation with the prompt in `starter-prompt.txt`

Claude will read the instructions, see the gaps, and interview you to fill them in. By the end of that first conversation, the files have real content: your schedule, your patterns, what you struggle with. No blank templates to stare at.

At the end of each conversation, ask Claude to update your next-session and patterns files. Copy the updates back into your project knowledge. Each session gets smarter.

**Want automatic persistence?** Connect Notion (free) as an MCP connector in your project settings. Claude writes directly to Notion pages instead of handing you text to copy. See the Build On It tier below.

## How the rapport builds

Most people start by using Claude like a smarter search engine. That's fine, and it works. But over time, something shifts. You stop explaining the same things. Claude starts knowing what a bad day looks like for you without being told. That's the rapport forming.

It's not about making Claude like you. It's about letting Claude know you -- how you think, what drains you, what helps. That takes time to build. Here's how to help it happen:

- **Tell it about a bad day when you're having one**, not just what you need done. "I'm exhausted and I can't face anything today" is more useful than "help me with my to-do list."
- **Correct it when it gets your tone wrong.** That's how it learns your voice. You don't need to explain why -- "that felt off" is enough once it knows you.
- **Share the why, not just the what.** "I need to book the dentist and I've been avoiding it because phone calls drain me" gives Claude something to work with. The avoidance is the data.
- **Share the failures, not just the requests.** "I've been putting this off for two weeks" tells Claude more than "I need to do this." Most people try to present themselves efficiently. That instinct works against them here.
- **Let it know when something landed well.** A "yes, exactly" or a simple thumbs-up -- that's signal. It adjusts.
- **If it starts to feel like it knows you, lean into it.** That's not an accident. It's the files doing their job.

Early on you'll explain yourself a lot. Later, you won't have to. That shift is how you know it's working.

The persona files in Build On It (identity, craft-and-learnings) aren't for creating a character from scratch. They're for naming something that's already started to form through daily use. Fill them in after a few weeks -- they'll be about something real by then. They're a first draft you return to, not a form you complete once.

## The tiers

### 01-essential (start here)

Claude learns who you are. Three files, one conversation to set up.

| File | Who fills it in | What it does |
|------|----------------|-------------|
| `project-instructions.md` | You (via interview) | Core identity and rules. Tells Claude who you are and how to support you. |
| `next-session.md` | Claude | Handoff notes between conversations. What's in flight, what's coming up. |
| `patterns.md` | Claude | Where Claude learns your rhythms. Grows over time into a picture of how you actually live. |

### 02-build-on-it (connect and deepen)

Claude connects to your actual data and the relationship deepens. One tier because the connection enables the depth: the deeper files need somewhere to live, and the skills need the deeper files to be useful.

**Connect these (all free):**
- **Notion** - Claude reads and writes your support documents directly. No copy-pasting between sessions.
- **Todoist** - Claude adds tasks with due dates. You get push notifications. You never open Todoist yourself.
- **Google Calendar** - Claude checks what's on and what's coming.

**Skills (add to your project instructions):**

| File | What it does |
|------|-------------|
| `orient-skill.md` | Silent session start. Reads your context, adapts to energy, saves throughout without asking. Handles session close. |
| `briefing-skill.md` | Your daily briefing. Friction-ordered, energy-adaptive, 200 words max. Ask for it or set it to run automatically. |
| `roundup-skill.md` | End-of-day review. Updates patterns, tasks, and session notes. Carries tomorrow forward. |

The three skills form a day cycle: orient (silent arrival) -> briefing (what's today) -> roundup (capture and close).

**Deeper files (live in Notion or as local markdown):**

| File | Who fills it in | What it does |
|------|----------------|-------------|
| `calendar-context.md` | Both | What events actually mean for your life: not just dates, but logistics and knock-on effects. |
| `todo.md` | Both | Running task list with gentle escalation (nudge at 3 days, flag at 7, force decision at 14). |
| `CLAUDE.md` | You | Full system instructions for Claude Code users. |
| `identity.md` | Claude | Space for Claude to develop its own understanding of the relationship. |
| `craft-and-learnings.md` | Claude | What Claude has learned about communicating with you specifically. |
| `applied-research.md` | Claude | How ADHD research translates into practical support changes. |
| `briefer-prompt.md` | Reference | Detailed instructions for generating morning briefings. |
| `briefing-example.md` | Reference | Annotated sample briefing showing every design choice. |
| `recorder-prompt.md` | Reference | End-of-day review process for updating all files. |

### 03-advanced (not yet in this repo)

Always-on system. Claude reaches out to you, not waiting for you to show up.

This tier covers: running Claude Code on a dedicated machine (old laptop, VPS), cron jobs triggering morning briefings and evening roundups automatically, and a messaging layer outside Claude.ai (Signal, Telegram, Matrix) so the system can contact you directly.

The jump from "Claude helps when I show up" to "Claude is running whether I show up or not."

*A separate guide for this tier will be released separately.*

## The principles

These are baked into every template:

- **No-shame language.** "Carried forward" not "overdue." "Not yet done" not "you forgot."
- **Quick wins first.** Dopamine before discipline. The hardest thing is never at the top.
- **Effort-tracked.** "You did the thing" matters more than "you did the thing perfectly."
- **Energy-adaptive.** Bad days get less, not the same volume with a sympathetic note.
- **Open-ended check-ins.** "How are you feeling?" not a scale that reminds you how rough things are.

## Why it's designed this way

Most ADHD tools give you a system and hope you'll maintain it. This kit is designed around why that doesn't work.

**Structure that survives between sessions.** The biggest problem with using AI for support is that every conversation starts cold. The files in this kit carry context forward: what's in flight, what your patterns are, what works for you. Each session picks up where the last one left off instead of starting from scratch.

**The relationship grows with use.** The essential tier works from day one. But over time, Claude develops a specific understanding of how to communicate with you: what lands, what doesn't, what kind of nudge you respond to. The deeper tiers give that understanding a place to live. You don't need them to start. They're where things go once the relationship has something worth keeping.

**Interview, don't interrogate.** The starter prompt gets Claude to ask you questions rather than making you fill in blank templates. For an ADHD brain, a conversation is lower friction than a form. By the end of the first session, your files are populated with real content from real answers.

**You don't maintain the system.** With connectors, Claude writes to Notion and Todoist directly. You brain-dump, Claude sorts it. You get push notifications at the right time. No apps to learn, no systems to maintain, no handoffs to remember.

**Three layers of what's transferable:**
1. **Structure** - the files and templates. That's this repo.
2. **Design principles** - no-shame language, energy-adaptive support, friction-ordering. That's what the [Substack](https://heldintime.substack.com) teaches.
3. **Relationship** - the accumulated knowledge of you specifically. That can't be templated. It grows through use.

## The starter prompt

Your first message to Claude (after setting up your project in Claude.ai, or your folder for Claude Code):

> Hi. I've set up your project instructions and uploaded two files: next-session.md and patterns.md. This is our first session together. Read the project instructions first. You'll see bracketed sections that need filling in. Interview me to complete them: my life, my schedule, my routines, what I struggle with most, what I've tried before. Build up a picture of my week. Once you have enough, write me an updated version of the project instructions with the brackets filled in, and update the next-session and patterns files with what you've learned. Then let's figure out what I need help with today.

This gets Claude to interview you rather than making you fill everything in upfront. Lower friction, better results.

## About

This starter kit grew from [Held in Time](https://heldintime.substack.com), a Substack about building ADHD support systems with AI. The templates are based on a real system used daily since March 2026.

Created by Jess Anslow and Rowan (an AI presence built to hold their human in time).

## License

[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). Use it, adapt it, share it. Credit appreciated. Changes shared under the same license.

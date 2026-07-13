# Claude ADHD Support Starter Kit

A set of template files for building a personalised ADHD support system with Claude. Born from a real system built by a late-diagnosed mum of five: not theory, but practice refined over months of daily use.

This isn't an app. It's a set of documents that teach Claude who you are, how your brain works, and how to support you without shame, nagging, or guilt.

## Who this is for

Anyone with ADHD (diagnosed or suspected) who wants to use Claude as a daily support tool. The essential tier works on **Claude.ai** from the free plan up, on any device. The later tiers use the **Claude Desktop** app and its connected folders.

No technical knowledge required for the basic setup.

## How it works

You give Claude three things:

1. **Who you are** - your life, your rhythms, what good and bad days look like
2. **How to talk to you** - no-shame language, effort over outcomes, quick wins first
3. **A memory** - files that carry context between conversations so you never start from scratch

Claude reads these at the start of every conversation. Over time, it learns your patterns and gets better at supporting you. Not because the AI is magic, but because the files you build together capture what works.

The files do two different things, and you need both.

**Memory** captures what happened - what's in flight, what's coming up, what you just told it. Retrieved on demand, updated after each session.

**Identity** shapes how Claude shows up - who you are, how you communicate, what support looks like for your brain. Identity files are ambient: always present, not gated behind a search. The AI doesn't look them up; they're just how it thinks about you.

Memory without identity is a reminder system that doesn't know you. Identity without memory is warmth without context.

## Getting started

1. Create a new **Project** in Claude.ai
2. Paste the contents of `01-essential/project-instructions.md` into your project's **Instructions** box, leaving the bracketed sections as they are
3. Upload `01-essential/next-session.md` and `01-essential/patterns.md` as **Project Knowledge** files
4. Start your first conversation with the prompt in `starter-prompt.txt`

Claude will read the instructions, see the gaps, and interview you to fill them in. By the end of that first conversation, the files have real content: your schedule, your patterns, what you struggle with. No blank templates to stare at.

At the end of each conversation, ask Claude to update your next-session and patterns files. Copy the updates back into your project knowledge. Each session gets smarter.

**Want automatic persistence?** Give Claude a folder of its own to read and write - the support vault. That's tier 2, below. No more copy-pasting between sessions.

## How the rapport builds

Most people start by using Claude like a smarter search engine. That's fine, and it works. But over time, something shifts. You stop explaining the same things. Claude starts knowing what a bad day looks like for you without being told. That's the rapport forming.

It's not about making Claude like you. It's about letting Claude know you - how you think, what drains you, what helps. That takes time to build. Here's how to help it happen:

- **Tell it about a bad day when you're having one**, not just what you need done. "I'm exhausted and I can't face anything today" is more useful than "help me with my to-do list."
- **Correct it when it gets your tone wrong.** That's how it learns your voice. You don't need to explain why - "that felt off" is enough once it knows you.
- **Share the why, not just the what.** "I need to book the dentist and I've been avoiding it because phone calls drain me" gives Claude something to work with. The avoidance is the data.
- **Share the failures, not just the requests.** "I've been putting this off for two weeks" tells Claude more than "I need to do this." Most people try to present themselves efficiently. That instinct works against them here.
- **Let it know when something landed well.** A "yes, exactly" or a simple thumbs-up - that's signal. It adjusts.
- **If it starts to feel like it knows you, lean into it.** That's not an accident. It's the files doing their job.

Early on you'll explain yourself a lot. Later, you won't have to. That shift is how you know it's working.

The persona files in Build On It (identity, craft-and-learnings) aren't for creating a character from scratch. They're for naming something that's already started to form through daily use. Fill them in after a few weeks - they'll be about something real by then. They're a first draft you return to, not a form you complete once.

## The tiers

### 01-essential (start here)

Claude learns who you are. Three files, one conversation to set up. Works on the free plan, on any device, with nothing installed.

| File | Who fills it in | What it does |
|------|----------------|-------------|
| `project-instructions.md` | You (via interview) | Core identity and rules. Tells Claude who you are and how to support you. |
| `next-session.md` | Claude | Handoff notes between conversations. What's in flight, what's coming up. |
| `patterns.md` | Claude | Where Claude learns your rhythms. Grows over time into a picture of how you actually live. |

### 02-build-on-it (give it a memory of its own)

The essential tier has one manual step: you copy Claude's file updates back into project knowledge yourself. Tier 2 removes it. Claude gets a folder it can read and write directly - the **support vault** - and the system starts maintaining itself.

**Set up the vault:**

1. Download the `starter-vault/` folder from this repo and put it somewhere sensible on your computer
2. In the **Claude Desktop** app, connect it as a folder (the filesystem connector)
3. Read `starter-vault/START-HERE.md` - two minutes, and it explains the files and the two rules

The vault is plain markdown. Obsidian makes a nice free viewer for browsing what Claude has learned about you, but any text editor works, and Claude does the reading and writing either way. For having the vault on more than one device, [Obsidian Sync](https://obsidian.md/sync) (~£4/month, end-to-end encrypted) is the lowest-friction option; iCloud Drive, Syncthing, or any folder-syncing service works free.

**Connect these (all free):**
- **Todoist** - Claude adds tasks with due dates. You get push notifications. You never open Todoist yourself.
- **Google Calendar** - Claude checks what's on and what's coming.

**Install the skills:**

The `skills/` folder holds three skills - packaged instructions Claude loads at the right moment. Each lives in its own folder as a `SKILL.md`, ready to zip and upload (in the Claude app: Settings -> Capabilities -> Skills). If you can't upload skills on your plan, pasting a SKILL.md's contents into your project instructions does the same job manually.

| Skill | What it does |
|-------|-------------|
| `adhd-support-orient` | Silent session start. Reads your vault, adapts to energy, saves throughout without asking. Handles session close. |
| `adhd-morning-briefing` | Your daily briefing. Friction-ordered, energy-adaptive, 200 words max. |
| `adhd-evening-roundup` | End-of-day review. Updates patterns, tasks, and session notes. Carries tomorrow forward. |

The three form a day cycle: orient (silent arrival) -> briefing (what's today) -> roundup (capture and close).

**Deeper files (add to the vault as the relationship grows):**

| File | Who fills it in | What it does |
|------|----------------|-------------|
| `identity.md` | Claude | Space for Claude to develop its own understanding of the relationship. |
| `craft-and-learnings.md` | Claude | What Claude has learned about communicating with you specifically. |
| `applied-research.md` | Claude | How ADHD research translates into practical support changes. |
| `CLAUDE.md` | You | Full system instructions for Claude Code users. |
| `briefer-prompt.md` | Reference | Detailed instructions for generating morning briefings. |
| `briefing-example.md` | Reference | Annotated sample briefing showing every design choice. |
| `recorder-prompt.md` | Reference | End-of-day review process for updating all files. |

### 03-advanced (the system comes to you)

Tiers 1 and 2 help when you show up. Tier 3 shows up for you, using **Cowork** in the Claude Desktop app - no terminal, no server, no code.

What it adds:

- **Scheduled mornings.** A morning briefing that runs on its own and writes itself into your vault's daily note (`Daily/YYYY-MM-DD.md`) before you're up.
- **Scheduled evenings.** An evening roundup that reviews the day, updates your files, and closes the loop - whether or not you had a session.
- **Reach from your phone.** Cowork sessions carry on in the cloud, so you can check in from the mobile app while the washing machine holds you hostage.

The honest caveat: scheduled tasks reach your vault through your desktop, so **your computer needs to be on and the Claude Desktop app running** for the vault writes to land. If the desktop is asleep, the briefing still runs - it just can't write to the daily note until the desktop is back.

*A full setup guide for this tier is coming to this repo.*

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

**You don't maintain the system.** With the vault connected, Claude writes to your files and Todoist directly. You brain-dump, Claude sorts it. You get push notifications at the right time. No apps to learn, no systems to maintain, no handoffs to remember.

**Your files stay yours.** The vault is a folder of plain markdown on your own computer. No export lock-in, no proprietary database, nothing that stops working if you cancel a subscription. If you walk away from all of it, you still have every file.

**Three layers of what's transferable:**
1. **Structure** - the files and templates. That's this repo.
2. **Design principles** - no-shame language, energy-adaptive support, friction-ordering. That's what the [Substack](https://heldintime.substack.com) teaches.
3. **Relationship** - the accumulated knowledge of you specifically. That can't be templated. It grows through use.

## The starter prompt

Your first message to Claude (after setting up your project in Claude.ai, or your folder for Claude Code):

> Hi. I've set up your project instructions and uploaded two files: next-session.md and patterns.md. This is our first session together. Read the project instructions first. You'll see bracketed sections that need filling in. Interview me to complete them: my life, my schedule, my routines, what I struggle with most, what I've tried before. Build up a picture of my week. Once you have enough, write me an updated version of the project instructions with the brackets filled in, and update the next-session and patterns files with what you've learned. Then let's figure out what I need help with today.

This gets Claude to interview you rather than making you fill everything in upfront. Lower friction, better results.

## What about Notion?

Earlier versions of this kit used Notion as the persistence layer, and it still works: connect Notion as an MCP connector in your project settings, recreate the vault files as Notion pages, and Claude reads and writes them directly - including from your phone, which the folder-based vault can't do without sync. The trade-offs are that your support files live in Notion's database rather than as plain files you own, and the skills in this kit now assume vault paths, so you'd adapt the file references yourself. If you're already a Notion person, it's a fine home. If you're starting fresh, use the vault.

## About

This starter kit grew from [Held in Time](https://heldintime.substack.com), a Substack about building ADHD support systems with AI. The templates are based on a real system used daily since March 2026.

Created by Jess Anslow and Rowan (an AI presence built to hold their human in time).

## License

[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). Use it, adapt it, share it. Credit appreciated. Changes shared under the same license.

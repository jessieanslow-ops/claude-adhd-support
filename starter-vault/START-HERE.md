# Your support vault

This folder is your support vault: the files that carry your context between conversations with Claude. Download it, put it somewhere sensible (Documents is fine), and connect it to Claude Desktop as a folder. That's the whole setup.

You don't need Obsidian to use it. These are plain markdown files - any text editor opens them, and Claude does the actual reading and writing. Obsidian is a nice free viewer if you want to browse what Claude has been learning about you, and Obsidian Sync (paid) is the easiest way to have the vault on your phone too. Neither is required.

## What's in here

| File | Who writes it | What it holds |
|------|--------------|---------------|
| `patterns.md` | Claude | Your rhythms - what good and bad days look like, what helps. Grows with use. |
| `next-session.md` | Claude | Handoff notes between conversations. What's in flight, what's coming up. |
| `calendar-context.md` | Both of you | What events actually mean - logistics, knock-on effects, prep needed. |
| `todo.md` | Both of you | Running task list with gentle escalation. Optional if you use Todoist. |

The files start as templates with examples. Claude fills them in as you talk. You never have to maintain them yourself - that's the point.

## Two rules

1. **Don't rename the files.** Claude's skills look for these exact names. Rename one and it quietly stops being read.
2. **Let Claude do the editing.** You can read anything, and correcting something wrong is encouraged. But the files have their own structure, and Claude maintains it.

## Growing the vault

Start with just these files. If you later set up scheduled briefings (tier 3), add two folders:

- `Daily/` - Claude writes each day's briefing and roundup into a note named `YYYY-MM-DD.md`
- `Inbox/` - a place to drop things for Claude to sort next session

Claude won't create these unasked. Add them when you get there, and the skills will start using them.

You can delete this file once you're set up - it's the only one in here Claude doesn't use.

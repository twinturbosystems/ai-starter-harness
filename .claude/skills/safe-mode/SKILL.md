---
name: safe-mode
description: Lists exactly what the assistant will and will not do inside this folder, and how to change those limits. Use when the person types /safe-mode or asks what the assistant is allowed to do here.
user-invocable: true
---

# Safe mode

Show the person the limits in force in this folder, plainly, and how to change them if they want to.

## What to say

Print the list below. Adapt it only if the person has changed the rules earlier in this conversation, and say so if you did.

What I will do in this folder, when you say yes:
- Create and edit files inside this folder.
- Run commands that only show information, like listing files or checking a version.
- Run the small programs we build together, after telling you what they do.

What I will not do without asking you first:
- Create, edit, or delete anything outside this folder.
- Install anything: packages, tools, extensions.
- Delete any file, even inside this folder.
- Run any command that changes files before telling you what it does.
- Send your files anywhere.

What I do not do here, even if asked:
- Say a step worked when it did not.
- Skip explaining a new term the first time it appears.

How this is enforced:
- `CLAUDE.md` in this folder holds the standing instructions I follow here. It is plain text and you can read it any time.
- `.claude/settings.json` in this folder tells Claude Code itself to keep its normal permission prompts on and to refuse to read secret files like `.env` (a file where programs keep passwords and keys).
- Claude Code has its own permission prompts on top of that. They are separate from me and you answer them yourself.

How to change it:
- To let me do more, for example edit files without asking each time, edit `CLAUDE.md` and remove or soften the line you want changed. Ask me to show you the line first.
- To let me do less, add a line under "Before you change anything" in `CLAUDE.md`.
- To turn teaching mode off entirely, rename `CLAUDE.md` to something else, or open Claude Code in a different folder.
- Claude Code's own permission settings live in `.claude/settings.json`. Ask me to explain any line before you change it.

Then ask: "Want me to change any of these now?" and wait.

## Rules

- This skill reads and prints. It does not change any file unless the person says which change they want and confirms it.
- Keep the wording the same each time so it reads as a fixed list, not a negotiation.
- Plain words, no hype, no exclamation marks, no bold inside sentences.

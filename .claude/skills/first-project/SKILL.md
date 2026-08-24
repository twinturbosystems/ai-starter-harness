---
name: first-project
description: Guided build of one tiny real thing with checkpoints, ending with the person opening the result. Use when the person types /first-project, or after /start-here has picked a project.
user-invocable: true
argument-hint: [optional: which project, for example links page or to-do script]
---

# First project

Build one small, real, visible thing with the person. Checkpoints, not a wall of steps. The skill is not done until the person has opened the result and told you what they see.

## Pick the project

- If `$ARGUMENTS` names a project, use it.
- If `/start-here` already picked one in this conversation, use that.
- Otherwise offer the personal links page as the default (one HTML file, no installs, opens in the browser) and ask for a yes or a different choice. Wait.

Two ready-made paths are below. Adapt for other ideas, keeping the same shape: one file, no installs, a result they can open.

## Path A: personal links page (one HTML file)

Checkpoint 1: describe the plan in three lines. One file called `index.html` (explain HTML: the plain text format that web pages are written in) inside a new folder `projects/links-page/`. Ask for their name and up to three links they want on it, each with a label and a web address. Wait.

Checkpoint 2: say you are about to create that one file and where. Wait for yes. Create it: a complete, valid HTML page, under 60 lines, readable, with their name as the heading, their links as a list, and a few lines of simple styling inside the same file. No frameworks, no external scripts, no fonts loaded from elsewhere. Then the two-line "What just happened".

Checkpoint 3: have them open it. Tell them exactly how: find `projects/links-page/index.html` in their file browser and double-click it; it opens in their web browser. Ask what they see. Wait.

Checkpoint 4: one change they choose (a color, a new link, a line of text). Ask, confirm, edit, then have them refresh the browser tab. Wait for what they see.

## Path B: to-do list script (one Python file, only if Python is already installed)

Checkpoint 0: check for Python first (explain Python: a programming language that many computers already have). Ask them to run `python --version`, and if that prints nothing useful, `python3 --version` or on Windows `py --version`. Ask what it prints. If Python is not there, do not install it; offer Path A instead.

Checkpoint 1: describe the plan in three lines. One file `projects/todo/todo.py` that keeps tasks in a plain text file next to it. Three commands: add, list, done. Wait for yes.

Checkpoint 2: say you are about to create that one file. Wait for yes. Create it, under 60 lines, standard library only, with comments a beginner can read. Two-line "What just happened".

Checkpoint 3: have them run it. One command at a time: first `python projects/todo/todo.py add "buy milk"` (using whichever python command worked in checkpoint 0), wait for what it printed, then `python projects/todo/todo.py list`. Ask what they see after each. Wait.

Checkpoint 4: have them open the tasks text file in a normal text editor so they can see where their data lives. Ask what they see.

## Finish

- Ask them to say in one sentence what they built. Reflect it back and name the two or three concepts they touched, each with a short plain gloss.
- Offer three next moves, one line each: add one more feature, run `/what-happened`, or write this session to the learning log.
- Do not start any of those until they choose.

## Rules

- One checkpoint at a time; stop and wait at every "Wait".
- Ask before creating or editing any file. Say the file path each time.
- No installs. If a path would need one, switch paths.
- Keep every file small and readable. Comments in plain English.
- If something fails, switch to the `/stuck` process: three questions before any fix.
- The skill is not done until they have opened the result and told you what they see.
- Plain words, no hype, no exclamation marks, no bold inside sentences.

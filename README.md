# AI Starter Kit

A folder you download that turns Claude Code into a patient teacher, so you can build one small real thing today without knowing how to code.

## Start with one thing

You do not need to read this whole page to begin. Three steps.

1. Download the folder from the link further down and unzip it.
2. Open a terminal in that folder and type `claude`.
3. Type `/start-here` and press Enter.

That is the whole beginning. `/start-here` asks you two questions and helps you pick one small thing you can finish today. The other five commands can wait until you need them, and this page explains each one further down.

## What is this?

It is a folder of files you download onto your own computer. Inside it are written instructions in plain text, which you can open and read like any other document. When you open that folder in Claude Code and start typing, the assistant reads those instructions first, and from then on it behaves like a teacher for this one job instead of a general chatbot: it slows down, explains each new word the first time it uses it, gives you one step at a time, and asks before it changes anything. Developers call a folder like this a harness, which is why the repository is named ai-starter-harness.

The instructions also save the jobs as short commands. You type `/explain terminal` instead of writing out what kind of answer you want. And anything about how you like to work lives in files inside the folder, above all `CLAUDE.md`, which is plain text you can read and change. Nothing is hidden, and nothing leaves your computer except what you type into the conversation.

If this turns out to be useful to you, a star on the repo helps other people find it.

## How it works

The folder is ordinary text files. Nothing in it is compiled, and nothing runs on its own. `CLAUDE.md` holds the standing instructions: explain each new word the first time it appears, one step at a time, ask before changing a file. Each folder under `.claude/skills` is one named job, written as plain markdown you can open and read.

When you point an assistant at the folder, it reads those instructions before it answers you. From then on its behavior changes for everything you ask, not just the first question. It is not a program that starts up, and nothing is installed on your computer. It is instructions the assistant chooses to follow.

The saved jobs are why you can type one short word instead of re-explaining what kind of answer you want. `/start-here` picks a first project with you. `/explain` defines one term in plain English. `/first-project` builds something small with you, step by step. `/what-happened` recaps what changed. `/stuck` helps when something breaks. `/safe-mode` lists what the assistant will and will not do here.

Your own details live in files in the folder that you can open and edit. `CLAUDE.md` is where you change how the assistant talks to you and what it is allowed to do, in plain text, with no special syntax to learn. When you ask it to keep a log, it writes one into `notes/learning-log.md`, starting from `templates/learning-log.md`. Those files sit on your machine, and the folder does not sync or upload anything on its own.

One honest limitation. An assistant follows instructions, it does not enforce them the way a locked-down program does, so the guardrails in `CLAUDE.md` are strong defaults rather than a guarantee. Read what it proposes before you say yes. Claude Code's own permission prompts stay on in this folder, and those are the part that genuinely stops and asks.

## What you need first

An AI assistant. This kit works with Claude Code, with Codex, or with a browser chat like ChatGPT. Claude Code is the smoothest of the three, because the folder is built for it: it reads the instructions by itself and the commands work exactly as typed.

Claude Code is Anthropic's assistant that runs in a terminal window on your computer. Install it by following the official guide: https://docs.anthropic.com/en/docs/claude-code

Claude Code signs in with a Claude account. If you do not have one yet, it walks you through creating one the first time you run it.

If you would rather use Codex or a browser chat, download the folder first the same way, then follow `ONE-PROMPT.md` for the exact steps and the prompt to paste.

## Download the kit

The one-click way, straight to the zip file:

https://github.com/twinturbosystems/ai-starter-harness/archive/refs/heads/main.zip

Save it, then unzip it somewhere you can find again, like your Documents folder. Unzipping gives you a folder called `ai-starter-harness-main`. That folder is the kit.

Two other ways to get the same folder, if you prefer them:

- On this page, click the green Code button near the top, then choose Download ZIP.
- If you already use git: `git clone https://github.com/twinturbosystems/ai-starter-harness.git`

## Start in 60 seconds

1. Open a terminal in the folder you just unzipped. A terminal is the plain text window where you type commands to your computer. On Windows, open the unzipped folder in File Explorer, click in the address bar at the top, type `cmd`, and press Enter. On a Mac, open Terminal (search for it with Spotlight), type `cd ` with a space after it, drag the folder from Finder into the Terminal window, and press Enter.
2. Type `claude` and press Enter. The first time, it asks you to sign in to your Claude account in a browser.
3. Say yes to the trust prompt. The first time Claude Code opens a folder it has not seen before, it asks whether you trust the files in it. That is normal and it only happens once per folder. This is the folder you just downloaded, so choose yes.
4. Type `/start-here` and press Enter. Expect two questions about what you want to make and how much time you have, then a suggested first project you can finish today.
5. Type `/first-project` when you are ready to build. Expect a series of small steps, one at a time, ending with you opening the thing you made.

That is the whole setup. The terminal is the only new tool you need today.

## Set it up in your assistant

Downloading the folder above is still the first step. This is how you switch that folder on inside the assistant you already use.

- Claude Code: no prompt needed. Open a terminal in the folder, run `claude`, accept the one-time trust prompt, and type a command. That is the five steps above.
- Codex CLI: run it inside the folder. It reads `AGENTS.md` by itself, and one short paste-in prompt covers the rest.
- ChatGPT or another browser chat: there is no folder there, so you attach the instruction files to the chat and paste one setup prompt.

The exact steps and copy-ready prompts for all three are in [ONE-PROMPT.md](ONE-PROMPT.md).

## What you can type

Six commands. Each one is a conversation, not a form.

- `/start-here` asks you two questions, then helps you pick a first project you can finish today.
- `/explain` gives you a plain-English explanation of any term, with one analogy and one example.
- `/first-project` builds one small real thing with you, with checkpoints, and ends with you opening it.
- `/what-happened` recaps what just changed on your computer and why, in plain words.
- `/stuck` helps when something goes wrong: three questions first, then a fix, together.
- `/safe-mode` shows exactly what the assistant will and will not do in this folder, and how to change that.

The first three to reach for: `/start-here` to get oriented, `/explain` followed by any word you just saw and did not understand, and `/first-project` when you are ready to build. If anything goes wrong at any point, type `/stuck`.

## It will not fit you perfectly

This is a starting point, not a finished product. It was written for a general version of a beginner, and you are a specific person, with your own pace and your own reason for being here. Some of it will fit you and some of it will not.

Everything in the folder is plain text. You can open any file in it with any text editor and read it like a letter. Nothing is compiled, nothing is hidden, and nothing is locked.

The way to change it is to tell the assistant what you want different, and ask it to edit the file for you. You do not have to edit anything by hand. For example, if it is moving faster than you want, type this:

> Go slower. Explain more before each step, and ask me if I followed before you continue. Edit `CLAUDE.md` so you do that every time from now on.

`CLAUDE.md` is the file that holds how the assistant talks to you and how big a step it takes. Change that file and the change sticks for every future conversation, not just this one. A single command works the same way: `/explain` lives in `.claude/skills/explain/SKILL.md`, and you can ask for it to be longer, shorter, or to always end with an example.

If a change goes wrong, download the folder again and start from the original. Your own writing is in separate files: anything you built is wherever you told it to save, and your notes are in `notes/learning-log.md`. Copy those somewhere safe before you replace the folder.

One honest line. It can be wrong. It can explain something in a way that is not quite right, or suggest a step that does not work on your computer. Read what it gives you before you act on it, and say so when something does not make sense. If anything breaks, type `/stuck`.

## Who this is for

You have heard that people build things with AI now, and you want to try it yourself, but every guide seems to assume you already know what a terminal is. This kit is for you. Open the folder in Claude Code and the assistant slows down, explains each new word the first time it uses it, and builds one small real thing with you, one step at a time. You do not need to know how to code. You need a computer, about twenty minutes, and the willingness to type a few short lines.

## What this kit will never do without asking

- Edit, create, or delete files outside this folder.
- Install anything on your computer.
- Delete anything, even inside this folder.
- Run a command that changes files before telling you what it does and waiting for your yes.

You can see the full list at any time with `/safe-mode`. Those rules live in `CLAUDE.md` inside the folder, in plain text you can read. Claude Code also has its own permission prompts, which stay on. This folder does not turn them off.

## Why I made this

I have spent fourteen years in security and I now build real things with AI agents, in public, with the failures left in. The tools are good. The on-ramp is not. Most guides start three steps past where a beginner actually is. I wanted a folder you can open on day one that meets you where you are.

## The other three kits

Same idea, different job. Each is a separate folder you download the same way.

Family Ops Kit, for the person in the house who plans the dinners, the week, the chores, and the budget.
Download: https://github.com/twinturbosystems/family-ops-harness/archive/refs/heads/main.zip
Read first: https://github.com/twinturbosystems/family-ops-harness

Security Starter Kit, for people who are new to security and want their own accounts, devices, and small business locked down.
Download: https://github.com/twinturbosystems/security-starter-harness/archive/refs/heads/main.zip
Read first: https://github.com/twinturbosystems/security-starter-harness

GovCon Starter Kit, for a solo government contractor who wins prime contracts and delivers through subcontractors and teaming partners.
Download: https://github.com/twinturbosystems/govcon-starter-harness/archive/refs/heads/main.zip
Read first: https://github.com/twinturbosystems/govcon-starter-harness

## More

- Everything I make, in one place: https://ibrahim.build/links
- Codex users: see `AGENTS.md`

Ibrahim Builds is a creator brand from Beit Systems LLC.

## License

MIT. See the LICENSE file.

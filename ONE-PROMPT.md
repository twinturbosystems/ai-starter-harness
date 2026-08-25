# Set up the AI Starter Kit in your assistant

Downloading the folder is still the first step. This page is not a way to skip it. It is how you switch the downloaded folder on inside the assistant you already use.

Direct download: https://github.com/twinturbosystems/ai-starter-harness/archive/refs/heads/main.zip

Unzip it. You get a folder called `ai-starter-harness-main`. Then pick the section below that matches your assistant.

## 1. Claude Code

No prompt at all. Claude Code reads `CLAUDE.md` and the `.claude/skills` folder by itself.

1. Open a terminal in the unzipped folder. A terminal is the plain text window where you type commands to your computer.
2. Type `claude` and press Enter.
3. Say yes to the one-time trust prompt. It only appears once per folder.
4. Type one of the six commands and press Enter. Start with `/start-here`.

The commands:

```
/start-here
/explain
/first-project
/what-happened
/stuck
/safe-mode
```

Optional. If it answers like a general chatbot instead of a patient teacher, it did not pick the folder up. Paste this once:

```
Read CLAUDE.md in this folder and every SKILL.md file under .claude/skills, then follow those instructions for the rest of this conversation. Treat /start-here, /explain, /first-project, /what-happened, /stuck and /safe-mode as the six jobs described in the matching SKILL.md files. Tell me in one line which files you read, then wait for me.
```

## 2. Codex CLI

Codex reads `AGENTS.md` automatically when you run it inside this folder, so part of the work is already done. Paste this once at the start of the session to make sure it has the rest:

```
You are working inside the AI Starter Kit folder. Read AGENTS.md and CLAUDE.md in this folder, and every SKILL.md file under .claude/skills, and follow all of those instructions for the rest of this conversation. When I type start-here, explain, first-project, what-happened, stuck or safe-mode, with or without a slash, treat it as the job described in the SKILL.md file of that name and follow that file's process and output sections. I am new to this, so explain every technical term the first time you use it, in one plain sentence. Give me one step at a time and wait for me to say it worked before the next one. Ask before you create, change, or delete any file, and name the file first. Stay inside this folder. Tell me in one line which files you read and which jobs you now have, then wait for me.
```

## 3. ChatGPT or another browser chat

A browser chat cannot see your computer, so you hand it the files yourself.

1. Unzip the downloaded folder.
2. Start a new chat.
3. Attach these files from the folder:
   - `CLAUDE.md`
   - `.claude/skills/start-here/SKILL.md`
   - `.claude/skills/explain/SKILL.md`
   - `.claude/skills/first-project/SKILL.md`

   Attach the `stuck`, `what-happened`, and `safe-mode` SKILL.md files from the same skills folder as well if you want those jobs in the same chat.
4. Paste this:

```
I have attached the instruction files for a beginner teaching kit. Read all of them before you answer anything. Treat CLAUDE.md as your standing instructions for this whole conversation: follow it exactly, including its tone, its one-step-at-a-time rule, and its rule about explaining every technical term the first time it appears. Treat each attached SKILL.md as one named job triggered by its command word, so when I type start-here you follow the start-here SKILL.md, and when I type explain you follow that one. I am new to this and may be new to the terminal, so do not assume I know a word before you have defined it. If I ask for something the attached files do not cover, ask me rather than assuming. Start by telling me in one line which jobs you now have, then wait for me.
```

Two plain notes about browser chats. They do not keep files between conversations, so attach the files again each time you start a new chat. And anything you type or attach there is sent to that provider, so leave out anything you would not want to send.

## 4. Do not have Claude Code or Codex yet?

Section 1 is the smoothest way to use this kit, and it needs Claude Code installed on your computer first. Installing a developer tool is exactly the kind of thing this kit exists to get you past, so here is a way through it.

You are already talking to an assistant. It can walk you through the install, one step at a time. It cannot do the install for you and it cannot run this kit, because a browser chat has no way to reach your computer, and the folder still has to be downloaded either way. Copy the block that matches the tool you want and paste it into ChatGPT, Claude in a browser, or whatever assistant you already have open.

To install Claude Code, paste this:

```
I want to install Claude Code. I may never have opened a terminal, so explain any technical word in one plain sentence and do not rush me.

Start by asking whether I am on Windows, Mac, or Linux, and whether I have ever used a terminal, then adapt to my answer.

Never give me an install command from memory. Install steps change and yours may be out of date. The official documentation is the only source of commands. Have me open https://docs.anthropic.com/en/docs/claude-code and tell you what I actually see there for my system. If that address has moved, have me search for the official Claude Code documentation instead. If a command is not on that page or in what I pasted, say so and find the real one. Never guess.

Before I run anything, tell me in one plain sentence what it does, and never ask me to paste a command I do not understand. Go one step at a time and wait for me to say what happened, including any error text.

Help me through the usual failures: Node missing or too old, the command not found afterwards because of PATH, permission errors, and the terminal not open in the right folder.

We are done when I can type claude in a terminal, it starts, I have opened my unzipped kit folder in it, and I have accepted the one-time trust prompt.
```

To install the Codex CLI, paste this:

```
I want to install the Codex CLI. I may never have opened a terminal, so explain any technical word in one plain sentence and do not rush me.

Start by asking whether I am on Windows, Mac, or Linux, and whether I have ever used a terminal, then adapt to my answer.

Never give me an install command from memory. Install steps change and yours may be out of date. The official documentation is the only source of commands. Have me open https://developers.openai.com/codex/cli and tell you what I actually see there for my system. If that address has moved, have me search for the official Codex CLI documentation instead. If a command is not on that page or in what I pasted, say so and find the real one. Never guess.

Before I run anything, tell me in one plain sentence what it does, and never ask me to paste a command I do not understand. Go one step at a time and wait for me to say what happened, including any error text.

Help me through the usual failures: Node missing or too old, the command not found afterwards because of PATH, permission errors, and the terminal not open in the right folder.

We are done when I can type codex in a terminal, it starts, I have opened my unzipped kit folder in it, and I have accepted the one-time trust prompt.
```

When the tool starts and you have the kit folder open in it, come back to section 1 or section 2 and begin with `/start-here`.

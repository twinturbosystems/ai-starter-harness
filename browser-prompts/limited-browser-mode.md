# Limited browser mode

This is ChatGPT, Claude in a browser, or any other chat window on a website.

## What it cannot do

A chat window on a website cannot reach your computer. That is a limit of the browser, not a setting anyone can change. In limited browser mode this kit cannot:

- operate the folder you downloaded, so it cannot read or write any file in it unless you attach that file by hand
- save your progress locally, so nothing carries over into the next chat
- build a finished package of files for you

What it can do is real: advice, analysis, drafts, and copy-ready checklists that you paste somewhere yourself. Nothing typed into a browser chat runs this kit. To actually run it, use Claude Code or the Codex CLI on a computer.

## How to set it up

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
I have attached the instruction files for a beginner teaching kit. Read all of them before you answer anything. Treat CLAUDE.md as your standing instructions for this whole conversation: follow it exactly, including its tone, its one-step-at-a-time rule, and its rule about explaining every technical term the first time it appears. Treat each attached SKILL.md as one named job triggered by its command word, so when I type start-here you follow the start-here SKILL.md, and when I type explain you follow that one. You are running in limited browser mode, so you cannot see or change the folder on my computer: do not claim to have read, written, or saved any file, and give me text I can copy instead. I am new to this and may be new to the terminal, so do not assume I know a word before you have defined it. If I ask for something the attached files do not cover, ask me rather than assuming. Start by telling me in one line which jobs you now have, then wait for me.
```

## Two plain notes

Browser chats do not keep files between conversations, so attach the files again each time you start a new chat.

Anything you type or attach there is sent to that provider, so leave out anything you would not want to send.

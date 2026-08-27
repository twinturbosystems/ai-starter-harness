# Set up the AI Starter Kit in your assistant

Downloading the folder is still the first step. This page is not a way to skip it. It is how you switch the downloaded folder on inside the assistant you already use.

Direct download: https://github.com/twinturbosystems/ai-starter-harness/archive/refs/heads/main.zip

Unzip it. You get a folder called `ai-starter-harness-main`.

The shortest path, if you have Claude Code or the Codex CLI on your computer: open a terminal in that folder, start the assistant, and type `Start the kit`. Nothing on this page is needed for that.

The prompts themselves now live in the [browser-prompts](browser-prompts/) folder, in plain view rather than inside the hidden `.claude` directory. This page points at them so there is one copy of each rather than two.

## 1. Claude Code

No prompt at all. Claude Code reads `CLAUDE.md` and the `.claude/skills` folder by itself. Open a terminal in the folder, type `claude`, confirm that any trust prompt names the folder you downloaded, then type `Start the kit`. Read later permission requests before deciding.

If it answers like a general chatbot instead of a patient teacher, the nudge prompt is in [browser-prompts/claude-code.md](browser-prompts/claude-code.md).

## 2. Codex CLI

Codex reads `AGENTS.md` automatically when you run it inside this folder. Paste the prompt in [browser-prompts/codex-cli.md](browser-prompts/codex-cli.md) once at the start of the session, then type `Start the kit`.

## 3. Limited browser mode

This is ChatGPT, Claude in a browser, or any other chat window on a website. It cannot operate the folder you downloaded, it cannot save your progress locally, and it cannot build final packages of files. It can give you advice, analysis, drafts, and copy-ready checklists. Nothing typed into a browser chat runs this kit.

Attach the single visible file [browser-prompts/browser-kit.md](browser-prompts/browser-kit.md). The short prompt to paste is in [browser-prompts/limited-browser-mode.md](browser-prompts/limited-browser-mode.md).

## 4. Do not have Claude Code or Codex yet?

An assistant you already have open can walk you through the install, one step at a time. The two install prompts are in [browser-prompts/install-the-assistant.md](browser-prompts/install-the-assistant.md).

## If something goes wrong

`docs/STUCK.md` has one next action for each of the common stumbles, including the command not being found and the assistant not being able to see the folder.

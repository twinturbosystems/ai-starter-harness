# Claude Code

You should not need a prompt at all. Claude Code reads `CLAUDE.md` and the `.claude/skills` folder by itself.

1. Open a terminal in the unzipped folder. A terminal is the plain text window where you type commands to your computer.
2. Type `claude` and press Enter.
3. If a trust prompt appears, check that it names the folder you downloaded, then approve that folder. Read later permission requests before deciding.
4. Type `Start the kit` and press Enter.

The commands, once you are going:

```
Start the kit
/start-here
/explain
/first-project
/what-happened
/stuck
/safe-mode
```

If it answers like a general chatbot instead of a patient teacher, it did not pick the folder up. Paste this once:

```
Read CLAUDE.md in this folder and every SKILL.md file under .claude/skills, then follow those instructions for the rest of this conversation. Treat /start, /start-here, /explain, /first-project, /what-happened, /stuck and /safe-mode as the jobs described in the matching SKILL.md files, and treat the words "Start the kit" as /start. Tell me in one line which files you read, then wait for me.
```

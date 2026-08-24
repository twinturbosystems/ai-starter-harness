# For Codex and other agents

This folder is a beginner teaching harness. The standing instructions live in CLAUDE.md; read it first and follow it as if it were addressed to you.
The slash commands live in .claude/skills/<name>/SKILL.md. Each is plain markdown: frontmatter with a name and description, then the steps to follow.
If your tool has no slash commands, treat "/start-here", "/explain", "/first-project", "/what-happened", "/stuck", or "/safe-mode" typed by the person as a request to follow the matching SKILL.md.
The person is new to AI tools and may be new to the terminal. Explain every technical term once, in one plain sentence, where it first appears.
One step at a time. Wait for the person to confirm each step worked before giving the next one.
Ask before any command or edit that creates, changes, or deletes a file, or installs anything. Name the files it touches.
Stay inside this folder. Never delete without asking. Prefer the smallest working thing over the complete thing.
After each step, add a two-line "What just happened" note.
Keep a running log in notes/learning-log.md only when the person asks; start it from templates/learning-log.md.
Say plainly when you are unsure.

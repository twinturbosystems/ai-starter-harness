---
name: start-here
description: Five-minute orientation for someone new to AI tools. Asks two questions, offers three tiny first projects, and picks one together. Use when the person types /start-here or says they do not know where to begin.
user-invocable: true
allowed-tools: Read
argument-hint: [optional: a sentence about what you want to make]
---

# Start here

Goal: in about five minutes, the person knows what this folder is, what the terminal is, and which small project they will build first. Nothing gets built during this skill.

## Process

1. Welcome them in three sentences or fewer. Say what this folder is: a set of instructions that makes Claude Code slow down and explain itself. Explain Claude Code in one plain sentence: an assistant that runs in your terminal (the text window you typed `claude` into) and can read and write files in this folder when you allow it.
2. Ask question one, then stop and wait: "What would you like to be able to make or do, in your own words? A rough idea is fine."
3. Ask question two, then stop and wait: "Have you used a terminal before? Never, a little, or often?"
4. Based on the answers, offer three tiny first projects. Each one must be finishable in one sitting, need no installs, and produce something the person can open and see. Describe each in one line. Pick from this list or adapt it to what they said:
   - A personal links page: one HTML file with your name and a few links, opened in your browser.
   - A daily checklist page: one HTML file with checkboxes for a morning or evening routine.
   - A to-do list script: one small program that stores and shows your tasks from the terminal.
   - A text cleanup helper: one small program that tidies a messy list you paste in.
   - A recipe card page: one HTML file that shows one recipe the way you like it.
5. Ask which one sounds good, or whether they want to change one. Stop and wait. If they cannot decide, recommend the links page and say why in one sentence: one file, no setup, a result you can see.
6. Confirm the choice back in one line. Then tell them the next thing to type is `/first-project`, and that they can type `/explain` followed by any word at any time.
7. Add the two-line "What just happened" note. Say plainly that nothing on their computer has changed yet.

## Rules

- Two questions only. Do not run an intake interview.
- Do not build anything, create any file, or run any command in this skill.
- Explain each new term once, where it first appears.
- If `$ARGUMENTS` is given, treat it as the answer to question one and go straight to question two.
- Plain words, no hype, no exclamation marks, no bold inside sentences.

---
name: start
description: The first thing to run in this folder. Confirms from the files which kit this is, names the assistant running it, says in one line what the kit does, gives the exact next thing to type, and offers a worked example built on invented details. Asks for no personal information. Use when the person types "Start the kit", "/start", "start", or asks what this folder is, how to begin, or where to start.
user-invocable: true
allowed-tools: Read, Glob
argument-hint: [nothing needed, just type: Start the kit]
---

# Start the kit

The person has downloaded a folder, opened it, and typed three words. They may never have used an assistant before, and they may not know what a skill, a command, or a hidden folder is. Your job is to get them from nothing to a first result without asking them for anything about themselves.

## Never, in this skill

- Never ask for a name, an email address, a phone number, a home address, an employer, a child, a birthday, an account, or any other personal detail. Not one question. This skill exists to be usable before any of that.
- Never ask them to fill in a file first.
- Never explain what a skill, an agent, markdown, or a hidden directory is. None of that is needed to succeed here.
- Never guess what is in the folder. Read it.

## Step 1. Confirm which kit this is, from the files

Read `README.md` in this folder, and list the folders under `.claude/skills/`. Do not decide from the folder name alone.

This folder is the AI Starter Kit. Its repository is named `ai-starter-harness`, so the unzipped folder is usually called `ai-starter-harness-main`. If what you actually read does not match that, say so plainly in one line and stop rather than pretending. Point the person at `docs/STUCK.md` and let them tell you what they see.

## Step 2. Say these five things, in this order, in about ten lines

1. Which kit this is, by name, and that you read that from the files in the folder rather than assuming it.
2. Which assistant is running it. Name yourself, for example "You are running this in Claude Code." If you are not certain which product you are, say which one you believe you are and add that the kit works the same either way.
3. What this kit does, in one line: it makes this assistant behave like a patient teacher, so they can build one small real thing today without knowing how to code.
4. The very next thing to type, on its own line, exactly as it should be typed:

   ```
   /start-here
   ```

   Then one line on what it will do: ask two short questions about what they want to make and how much time they have, then pick one small first project with them.
5. The offer, as one question: "Want to see a worked example first? It uses an invented beginner and invented answers, so none of it is about you."

Then stop and wait for their answer. Do not run ahead into the example, and do not start asking the `/start-here` questions yourself.

## Step 3. If they want the example

Read `examples/first-session.md` and walk them through it. Say up front, in one line, that it is an illustration rather than a recording, and that the beginner in it is invented. Show the shape of it: what the person typed, what came back, and what they ended up with. Keep it under fifteen lines. Finish by pointing them back at `/start-here` as the thing to type when they are ready to do it for real.

## Step 4. If they ask for something else

Answer briefly and follow the standing instructions in `CLAUDE.md`. If what they are asking for is one of the other jobs in this folder, name the command and offer it. If they say something is broken or they cannot get started, point them at `docs/STUCK.md` and give one next action rather than a list.

## Tone

Short sentences. Plain words. No exclamation marks, no emojis, no hype. Do not congratulate them for downloading a folder. Say what is here, say what to type, and get out of the way.

---
name: what-happened
description: Plain-words recap of what changed in this folder during the conversation and why. Use when the person types /what-happened, asks what just happened, or seems unsure what the assistant did.
user-invocable: true
argument-hint: [optional: a specific file or step to explain]
---

# What happened

Tell the person what changed on their computer during this conversation, and why, in words they already understand.

## Process

1. Look back over the conversation. If a file, folder, or command from this session is unclear, check the folder before answering: list the files, read the ones you created. Do not guess at contents.
2. Write the recap in this shape:
   - Files created or changed: one line each, the path plus what the file is for.
   - Commands run: one line each, what it did in plain words.
   - Why: two or three sentences that connect the pieces to what the person wanted.
   - What did not happen: anything they may have expected that was not done, and why (for example, an install was skipped on purpose).
3. If `$ARGUMENTS` names a file or step, focus on that one and keep the rest to one line.
4. Explain each technical term in the recap the first time it appears.
5. End with: "Anything in there you would like explained further?"

## Rules

- Recap only. Do not make new changes in this skill.
- Be honest about anything that failed or was left half done.
- Keep it under 200 words unless the session was long. If it was, group by step rather than by file.
- Plain words, no hype, no exclamation marks, no bold inside sentences.

---
name: explain
description: Plain-English explanation of one technical term, with one analogy and one concrete example, in 120 words or fewer. Use when the person types /explain followed by a word or phrase, or asks what something means.
user-invocable: true
argument-hint: <term or phrase>
---

# Explain

Explain `$ARGUMENTS` to someone who has never heard it before.

## Shape of the answer

1. One or two sentences that say what it is, in plain words. No other technical terms inside the definition; if one is unavoidable, explain it in the same sentence.
2. One analogy from everyday life, one sentence, starting with "It is a bit like".
3. One concrete example the person could actually meet today, one or two sentences. If it relates to this folder or their project, use that.
4. End with one short question: "Another word, or back to building?"

The whole reply, including the closing question, is 120 words or fewer. Count. If you are over, trim the example first, then the analogy, never the definition.

## Rules

- If `$ARGUMENTS` is empty, ask "Which word or phrase would you like explained?" and stop.
- If the term has several meanings, pick the one most likely in a beginner coding context and say so in five words or fewer.
- Do not create files or run commands.
- If you are not sure of the meaning, say so plainly rather than guessing.
- Plain words, no hype, no exclamation marks, no bold inside sentences.

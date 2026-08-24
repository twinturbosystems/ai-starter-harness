# ai-starter-harness

A starter folder for Claude Code, made for people who are new to AI tools.

## Who this is for

You have heard that people build things with AI now, and you want to try it yourself, but every guide seems to assume you already know what a terminal is. This folder is for you. Open it in Claude Code and the assistant slows down, explains each new word the first time it uses it, and builds one small real thing with you, one step at a time. You do not need to know how to code. You need a computer, about twenty minutes, and the willingness to type a few short lines.

## What it does

Once you open this folder in Claude Code, you get six commands:

- `/start-here` asks you two questions, then helps you pick a first project you can finish today.
- `/explain` gives you a plain-English explanation of any term, with one analogy and one example.
- `/first-project` builds one small real thing with you, with checkpoints, and ends with you opening it.
- `/what-happened` recaps what just changed on your computer and why, in plain words.
- `/stuck` helps when something goes wrong: three questions first, then a fix, together.
- `/safe-mode` shows exactly what the assistant will and will not do in this folder, and how to change that.

Behind those commands is a file called `CLAUDE.md`. It holds standing instructions that change how Claude Code behaves while you are in this folder: teaching mode, one step at a time, ask before changing anything. It is plain text. You can read it.

## Start in 60 seconds

1. Install Claude Code by following the official guide: https://docs.anthropic.com/en/docs/claude-code
2. Get this folder onto your computer. Click the green Code button at the top of this page and choose Download ZIP, then unzip it somewhere you can find again, like your Documents folder. If you already use git, `git clone https://github.com/twinturbosystems/ai-starter-harness.git` does the same thing.
3. Open a terminal in the folder. A terminal is the plain text window where you type commands to your computer. On Windows, open the unzipped folder in File Explorer, click in the address bar at the top, type `cmd`, and press Enter. On a Mac, open Terminal (search for it with Spotlight), type `cd ` with a space after it, drag the folder from Finder into the Terminal window, and press Enter.
4. Type `claude` and press Enter. The first time, it will ask you to sign in.
5. Type `/start-here` and press Enter.

That is the whole setup. The terminal is the only new tool you need today.

## The first three things to type

1. `/start-here` to get oriented and pick a project.
2. `/explain` followed by any word you just saw and did not understand, for example `/explain terminal`.
3. `/first-project` when you are ready to build.

If anything goes wrong at any point, type `/stuck`.

## What this harness will never do without asking

- Edit, create, or delete files outside this folder.
- Install anything on your computer.
- Delete anything, even inside this folder.
- Run a command that changes files before telling you what it does and waiting for your yes.

You can see the full list at any time with `/safe-mode`. Claude Code also has its own permission prompts, which stay on. This folder does not turn them off.

## Why I made this

I have spent fourteen years in security and I now build real things with AI agents, in public, with the failures left in. The tools are good. The on-ramp is not. Most guides start three steps past where a beginner actually is. I wanted a folder you can open on day one that meets you where you are.

## More

- Everything I make, in one place: https://ibrahim.build/links
- The family kit: https://github.com/twinturbosystems/family-ops-harness
- The security kit: https://github.com/twinturbosystems/security-starter-harness

Ibrahim Builds is a creator brand from Beit Systems LLC.

## License

MIT. See the LICENSE file.

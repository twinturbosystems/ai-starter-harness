# Example: what a first session can look like

This is an illustration, not a recording. The lines below show the shape of a first session so you know what to expect. Your session will differ. Nothing here is a promise about how long anything takes or how it turns out.

Text after "You:" is what the person types. Text after "Assistant:" is the kind of reply this folder's instructions produce.

---

You: /start-here

Assistant: Welcome. This folder is a set of instructions that makes Claude Code slow down and explain itself as we go. Claude Code is an assistant that runs in your terminal (the text window you typed `claude` into) and can read and write files in this folder when you allow it.

First question: what would you like to be able to make or do, in your own words? A rough idea is fine.

You: I want a simple page with my name and links to my stuff, like a link in bio thing

Assistant: Good, that is a real project and a small one. Second question: have you used a terminal before? Never, a little, or often?

You: never, this is my first time

Assistant: Then we go one step at a time, and I will explain each new word the first time it comes up. Here are three projects that fit what you said. All three need nothing installed and give you something to open and look at.

1. A personal links page: one HTML file with your name and a few links, opened in your browser.
2. A daily checklist page: one HTML file with checkboxes for a routine.
3. A to-do list script: one small program you run from the terminal.

The first one is what you described. Want to go with it, or change something?

You: the first one

Assistant: Personal links page it is. When you are ready to build, type /first-project. At any point, type /explain followed by a word you did not understand, for example /explain HTML.

What just happened: we picked one small project with a visible result. Nothing on your computer has changed yet.

---

You: /explain HTML

Assistant: HTML is the plain text format that web pages are written in. A browser reads an HTML file and turns the text into what you see on screen: headings, links, images.

It is a bit like a recipe card: the card is only words and structure, and the cook, your browser, turns it into the dish.

Concrete example: the links page we are about to build will be one file named index.html. Open it in a text editor and you see words and tags. Open it in a browser and you see your page.

Another word, or back to building?

---

You: /first-project

Assistant: Here is the plan, three lines. One file called index.html in a new folder projects/links-page/. It will have your name as the heading and your links as a list. A few lines of styling inside the same file so it looks tidy.

Before I create anything, I need two things from you: the name you want at the top, and up to three links, each with a label and a web address.

You: Sam Rivera. Links: my Instagram instagram.com/example, my shop example.com/shop, my email sam@example.com

Assistant: Got it. I am about to create one file: projects/links-page/index.html. It touches only that one new file. Is that a yes?

You: yes

Assistant: (creates the file, then continues)

Done. What just happened: I created projects/links-page/index.html, a single web page with your name and three links. Nothing else on your computer changed.

Next step, and then I will wait: open the folder projects/links-page in your file browser and double-click index.html. It should open in your web browser. Tell me what you see.

You: it opened, I see my name in big letters and the three links under it

Assistant: That is the page working as intended. Want to change one thing now? A color, the order, a fourth link?

---

That is the shape of it. The session continues with one small change, then a recap through /what-happened, and if the person asks for it, an entry in notes/learning-log.md.

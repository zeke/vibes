# 🔮 Vibe Coding Workshop

Vibe coding is a new practice in software development where humans chat with AI language models that generate code. The human provides instructions using natural language (English, Spanish, Chinese, etc.) and the model generates code (JavaScript, Python, CSS, HTML, etc) to satisfy those requirements. It's an iterative process where human and machine work together to build and improve an app, website, game,tool, or document through a long-running conversational dialogue.

To vibe code is to "give in to the vibes", disregarding the specific implementation details of the code you're generating, and instead improving your project through natural language prompts.

The term was [coined by Andrej Karpathy](https://x.com/karpathy/status/1886192184808149383) in early 2025.

In this workshop, you'll **learn how to vibe code using Cursor and p5.js**. If you don't know what those things are, don't worry. We'll cover that!

## Prerequisites

You will need:

- A computer
- An internet connection
- An open mind

You'll also need to install the following software:

- [Cursor](https://www.cursor.com/) - Code editor with AI superpowers (Free to start / Paid features for advanced use)
- [GitHub Desktop](https://github.com/apps/desktop) - Free and open-source app for working with Git and GitHub.

You can optionally create a [GitHub](https://github.com/) account if you want to store your code in the cloud, publish it, and share it with others.

## What is p5.js?

p5.js is a friendly tool for learning to code and make art. It is a free and open-source JavaScript library built by an inclusive, nurturing community. p5.js welcomes artists, designers, beginners, educators, and anyone else!

p5.js is a port of the popular [Processing](https://processing.org/) project, but written in JavaScript (instead of Java) so it works in web browsers.

p5.js has been around for a long time and it's well documented, so the large language models of the world have lots of context about p5.js in their training data. That makes it a great tool for vibe coding, as AI models can write working code for p5.js apps without much help.

Check out the [p5.js website](https://p5js.org/examples/) for examples of what you can do with it.

## What is Cursor?

Cursor is a code editor with AI superpowers.

Cursor is built on top of VS Code, the popular open-source code editor from Microsoft. VS Code is free and open-source, and is used by millions of developers around the world. Cursor is basically the same thing as VS Code, but with some extra features for writing code with AI assistance.

Cursor is also a venture-backed startup that's raised 1 billion dollars and is valued at 10 billion dollars.

## Cursor Commands

Cursor has [lots of keyboard shortcuts](https://docs.cursor.com/configuration/kbd), but there are a few that are particularly useful:

- <kbd>cmd + shift + p</kbd> (Mac) / <kbd>ctrl + shift + p</kbd> (Windows/Linux) - Open the Command Palette. The meta-keyboard shortcut ... kinda like Spotlight on Mac. Type stuff and run it.

And these are the AI-powered commands:

- <kbd>cmd + k</kbd> (Mac) / <kbd>ctrl + k</kbd> (Windows/Linux) - Edit at the current line or block of selected code
- <kbd>cmd + l</kbd> (Mac) / <kbd>ctrl + l</kbd> (Windows/Linux) - Edit the current file
- <kbd>cmd + i</kbd> (Mac) / <kbd>ctrl + i</kbd> (Windows/Linux) - Edit the whole project

Mnemonics for your convenience:

- **k** is for kitty (small) 😻
- **l** is for lion (large cat) 🦁
- **i** is for infinity (whole project) 🌎

## Step 1: Set up a new project

Open GitHub Desktop.

1. Click on **File > New Repository...**
1. In the dialog, set the **Name** to `vibes` and choose a location for your project folder.
1. (Optional) Add a description if you like.
1. Leave **Initialize this repository with a README** unchecked (we'll generate it later).
1. Click **Create Repository**.

You now have a new, empty Git repository called `vibes` on your computer.

In Cursor, click **File > Open Folder...** and select the `vibes` folder you just created.

## Step 2: Commence vibing

Notice the pane on the right side of the screen that says "New Chat". This is the chat interface where you have a conversation with the AI "agent". (If you don't see this pane, type <kbd>cmd + i</kbd> (Mac) / <kbd>ctrl + i</kbd> (Windows/Linux) to open it)

Now type an instruction like this:

> **Create an index.html with a simple p5.js setup using CDN-hosted libraries.**

Cursor will take a minute to think before generating some code. When it's done, you should see a new file called `index.html` in your project directory. It should look something like this:

![cursor-agent-mode](./images/cursor-agent.png)

Let's break down what just happened:

- We gave it an instruction about a specific file to create
- We mentioned the popular p5.js library
- We asked for CDN-hosted libraries. This means our code can refer to a script that's hosted on a CDN (Content Delivery Network) like [unpkg](https://unpkg.com/) or [jsDelivr](https://www.jsdelivr.com/), so we don't have to bother downloading and configure it in our project.

## Step 3: Open your project in a browser

Let's see what it looks like in a browser.

Find your project folder in your computer's file explorer/finder and double-click `index.html` to open it in your default browser.

## Step 4: Save your progress

You have something that works. Yay!

Your project is already a Git repository, thanks to GitHub Desktop.

To save your progress:

1. Open GitHub Desktop.
1. You should see your `vibes` repository listed. If not, use **File > Add Local Repository...** and select your `vibes` folder.
1. Any new or changed files (like `index.html`) will appear in the **Changes** tab.
1. Enter a summary for your commit (e.g., "Add index.html").
1. Click **Commit to main**.
1. (Optional) Click **Publish repository** to push it to GitHub.com if you want a remote backup.

## Step 5: Continue vibing

Now that you have a working p5.js project, you can start to vibe.

Here are some prompts you can try to take your project to the next level:

> Generate a tutorial page about Perlin noise with multiple p5 sketches, explaining what it is and how to use it.

---

> Create a visualizer for mic input that maps frequencies to colorful dancing shapes.

---

> Create a motion detection system that uses the webcam to replace pixels in the image with ascii characters.

---

> Make an interactive particle system where particles are attracted to the mouse and leave colorful trails.

---

> Create a generative art piece using recursive patterns and the noise() function for organic movement.

---

> Build a physics simulation with bouncing balls that interact with each other using vectors.

---

> Make a flocking simulation inspired by Craig Reynolds' Boids algorithm to simulate bird-like movement.

---

> Create an interactive soundscape where clicking creates ripples that generate tones based on their size and speed.

---

> Build a cellular automaton like Conway's Game of Life with custom rules and colorful cell states.

---

> Generate a fractal tree that responds to wind simulation using noise and transforms.

---

> Create a three-dimensional structure that you can navigate through using the keyboard or mouse. Take advantage of P5 "orbit controls".


## Step 6: Generate a README!

Once you've got your project into a state that you're happy with, you can generate a README.md file to document your project.

Type this into the chat:

> **Generate a README.md file for this project. Keep it short and sweet.**

## Tips

- **Use Git to save your progress**. Whenever you make a change that you like, commit it to your repository. That way you can always restore you work if you mess something up.

- **Don't ask leading questions!** The AI will tend to agree with you. For example, instead of asking a question like "Do the red dots represent nodes in the graph?", try something like "What do the red dots represent?"

- **Use URLs to give the AI specific reference material**. You can paste in a URL to a website to give the AI specific reference material for use when generating code.

- **Start over by making a new file!** If you want to start over, just make a new file. The AI will usually be able to figure out what you want to do based on the context of the project.

- **Use the Command Palette to open the project in Cursor**. You can open the project in Cursor by typing <kbd>cmd + i</kbd> (Mac) / <kbd>ctrl + i</kbd> (Windows/Linux) in the terminal.

## Examples

- [Vibe coding an iOS app](https://x.com/karpathy/status/1903671737780498883)
- [Vibe coding menuGen](https://karpathy.bearblog.dev/vibe-coding-menugen/) - a web app that converts text-based restaurant menus into visual menus

## Alternative tools

Cursor is currently one of the most popular tools among professional developers, but there are lots of other tools out there for vibe coding. Here are some popular ones:

| Tool                         | Core Use Case                          | Ideal For                          |
|-----------------------------|----------------------------------------|------------------------------------|
| [GitHub Copilot](https://github.com/features/copilot)              | In-editor suggestions                  | Everyday coding                    |
| [v0](https://v0.dev/)                          | Front‑end UI generation                | UX designers, React devs           |
| [Val Town](https://val.town/)                   | TypeScript cloud functions             | Backend prototyping                |
| [Lovable](https://lovable.dev/)                     | Full‑stack app creation via prompts    | Non‑tech builders, prototyping     |
| [Replit](https://replit.com/)                      | Collaborative, multi‑language coding   | Students, generalists              |
| [Windsurf](https://windsurf.com/)                    | Agentic code IDE + preview             | Power developers, teams            |
| [Claude Code](https://www.anthropic.com/claude-code)                 | Debugging, refactoring, Git work       | Senior devs, long coding sessions  |
| [LM Studio](https://lmstudio.ai/)                   | Local LLM experimentation & code       | LLM enthusiasts, developers        |
| [Bolt](https://bolt.new/)                        | UI prototyping                         | Front‑end designers                |
| [Superwhisper / Composer](https://example.com/)     | Voice/prompt-driven builds             | Experimental use                   |
| [Aider](https://aider.ai/)                       | Context-specific code output           | Developers needing fine control    |


# Vibe Coding Workshop

Hello! Let's do some vibe coding!

## What is vibe coding?

The term "vibe coding" was coined by Andrej Karpathy in early 2025:

> There's a new kind of coding I call "vibe coding", where you fully give in to the vibes, embrace exponentials, and forget that the code even exists. It's possible because the LLMs [...] are getting too good. Also I just talk to Composer with SuperWhisper so I barely even touch the keyboard. I ask for the dumbest things like "decrease the padding on the sidebar by half" because I'm too lazy to find it. I "Accept All" always, I don't read the diffs anymore. When I get error messages I just copy paste them in with no comment, usually that fixes it. The code grows beyond my usual comprehension, I'd have to really read through it for a while. Sometimes the LLMs can't fix a bug so I just work around it or ask for random changes until it goes away. It's not too bad for throwaway weekend projects, but still quite amusing. I'm building a project or webapp, but it's not really coding - I just see stuff, say stuff, run stuff, and copy paste stuff, and it mostly works.

Examples:

- [Vibe coding an iOS app](https://x.com/karpathy/status/1903671737780498883)

## What is Cursor?

Cursor is a code editor with AI superpowers.

Cursor is built on top of VS Code, the popular open-source code editor from Microsoft. VS Code is free and open-source, and is used by millions of developers around the world. Cursor is basically the same things as VS Code, but with some extra features for writing code with AI assistance.

Cursor is also a venture-capital backed startup that's raise 1 billion dollars and is valued at 10 billion dollars.

## Prerequisites

You will need:

- A computer
- An internet connection
- An open mind

## Step 0: Install software

In this workshop we will use the following software:

- [Cursor](https://www.cursor.com/) - Code editor with AI superpowers (Free to start / Paid features for advanced use)
    1. Sign up or login or "Skip and continue"
    1. You can optionally import your existing VS Code settings (or skip and continue)
    1. Choose a theme (or skip it!)
    1. Key bindings (or skip it!)
    1.  "Open from terminal" -- Yes. You want this.

- [GitHub Desktop](https://github.com/apps/desktop) - Free and open-source software for easily working with Git and GitHub.

Optional:

- [GitHub](https://github.com/) account (optional) - A place to store, publish, and collaborate on your code. (Free to start / Paid features for advanced use)


## Cursor Commands

Cursor has [lots of keyboard shortcuts](https://docs.cursor.com/configuration/kbd), but there are a few that are particularly useful:

- <kbd>cmd + shift + p</kbd> (Mac) / <kbd>ctrl + shift + p</kbd> (Windows/Linux) - Open the Command Palette. The meta-keyboard shortcut ... kinda like Spotlight on Mac. Type stuff and run it.

And these are the AI-powered commands:

- <kbd>cmd + k</kbd> (Mac) / <kbd>ctrl + k</kbd> (Windows/Linux) - Edit at the current line or block of selected code
- <kbd>cmd + l</kbd> (Mac) / <kbd>ctrl + l</kbd> (Windows/Linux) - Edit the current file
- <kbd>cmd + i</kbd> (Mac) / <kbd>ctrl + i</kbd> (Windows/Linux) - Edit the whole project

Mmnemonics for your convenience:

- **k** is for kitty (small)
- **l** is for lion (large cat)
- **i** is for infinity (whole project)

## Step 1: Set up a new project

Open Cursor.

Cursor has a built-in terminal for running commands on your computer.

We'll use that to create a new project.

Start by opening a new terminal in Cursor.

Press <kbd>cmd + shift + p</kbd> (Mac) or <kbd>ctrl + shift + p</kbd> (Windows/Linux) to open the Command Palette 

Type "terminal" and select "Terminal: Create New Terminal".

A terminal pane should open at the bottom of the screen.

Now you issue commands to the terminal.

Create a new folder called `vibes` and change into it:

```
mkdir vibes
cd vibes
```

You now have an empty folder called `vibes`.

Open the sidebar by pressing <kbd>cmd + b</kbd> (Mac) or <kbd>ctrl + b</kbd> (Windows/Linux).

If you are not already in the `vibes` folder, click the "Open Folder" button and navigate to your `vibes` folder.

## Step 2: Dive in

In cursor, type <kbd>cmd + i</kbd> to open Agent mode. You should see a new panel on the right side of the screen that says "New Chat"

Type an instruction like this:

> Create an index.html with a simple p5.js setup using CDN-hosted libraries.

Cursor will take a minute to think, consulting an AI oracle, before generating some code. When it's done, you should see a new file called `index.html` in your project directory. It should look something like this:

![cursor-agent-mode](./images/cursor-agent.png)

## Step 3: Open your project in a browser

In Cursor, type <kbd>cmd + l</kbd> to open the file explorer.

Click on `index.html` to open it in a new tab.

## Step 4: Sprinkle in some React

## Step 5: Add tailwind for styles

## Step 6: 

## Step 10: Use URLs

Paste in a URL to a website and see what happens!

## Dangers and limitations of vibe coding

- Vibe code is not always correct
- Vibe code is not always safe
- Vibe code is not always efficient
- Vibe code is not always easy to understand
- Complex systems are harder to code with AI

## Alternative tools

We won't be covering them in this workshop, but there are many great tools out there for vibe coding. Here are some popular ones:

- Val Town
- Lovable
- v0
- Replit
- Windsurf
- Claude Code


Extras

- System prompt in cursor
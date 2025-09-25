# Version Control with Git

## What is Git?

Git is a version control system that tracks changes to your files over time. Think of it as a sophisticated "undo" system that remembers every version of your project. You can:
- Save snapshots of your work (called "commits")
- Go back to any previous version
- See what changed between versions
- Work on different features simultaneously without breaking things

## What is GitHub?

GitHub is a website that hosts Git repositories online. It's like Google Drive but specifically designed for code. GitHub lets you:
- Back up your code online
- Share projects with others
- Collaborate with teammates
- Showcase your portfolio
- Contribute to open-source projects

## What is GitHub Desktop?

GitHub Desktop is a visual app that makes Git easier to use. Instead of typing commands in a terminal, you can click buttons to:
- Save changes
- View your project history
- Sync with GitHub
- Switch between different versions

## Why use version control?

Version control helps you:
- **Recover from mistakes** - Accidentally deleted something? Get it back from a previous commit
- **Experiment safely** - Try new ideas without fear of breaking working code
- **Track your progress** - See how your project evolved over time
- **Collaborate** - Work with others without stepping on each other's toes
- **Build a portfolio** - Show potential employers your coding journey

## Installation

### Git (command line)
- **Mac**: Already installed! Open Terminal to use it
- **Windows**: Download from [git-scm.com](https://git-scm.com/)
- **Linux**: Run `sudo apt-get install git` (Ubuntu/Debian) or equivalent

### GitHub Desktop
Download from [desktop.github.com](https://desktop.github.com/)

### GitHub account
Sign up free at [github.com](https://github.com/)

## Basic usage

### Using Git from terminal

```bash
# Start tracking a project
git init

# Save your current work
git add .
git commit -m "describe what you changed"

# View history
git log

# Go back to a previous version
git checkout [commit-id]
```

### Using GitHub Desktop

1. **Open GitHub Desktop**
2. **Add your project**: File > Add Local Repository > Select your folder
3. **Save changes**:
   - Changed files appear in the left panel
   - Write a summary of your changes
   - Click "Commit to main"
4. **Upload to GitHub**: Click "Publish repository" (first time) or "Push origin" (subsequent times)

### Connecting to GitHub

After creating a GitHub account:
1. In GitHub Desktop: Sign in with your GitHub account
2. For terminal: Run `git config --global user.email "your-email@example.com"`

## Common workflow

1. Make changes to your files
2. Save a snapshot (commit) when something works
3. Continue coding
4. If you mess up, restore from a previous commit
5. Optionally push to GitHub for backup

## Learn more

- [GitHub's Git tutorial](https://try.github.io/)
- [Interactive Git branching tutorial](https://learngitbranching.js.org/)
- [GitHub Desktop documentation](https://docs.github.com/desktop)
# GitHub 101 — Quick Reference & Article Index

This file helps Claude quickly answer GitHub questions by pointing to the right section of `github-101.md`. For detailed explanations, read the full article.

## Article Map

| Section | Line | What it covers |
|---------|------|----------------|
| **GitHub in Plain Language** | 58 | What Git and GitHub are, why they matter for non-engineers, how collaboration works |
| **Meet the Practice Repo** | 112 | Introduction to the acme-ops practice repo used throughout the article |
| **Part 1: Setup & Installation** | 132 | GitHub account, installing Git, configuring Git, SSH keys, GitHub CLI, GitHub MCP |
| **Part 2: GitHub Repositories 101** | 282 | What repos are, repo structure on GitHub, organizing repos, public vs private, cloning, forking |
| **Part 3: The Daily GitHub Workflow** | 505 | The 6-step workflow (branch → edit → commit → push → PR → merge), Google Drive comparisons, deep dive on each step |
| **When Things Go Wrong** | 1025 | Common Git errors and how to fix them |
| **.gitignore** | 1099 | What files to exclude from Git (API keys, node_modules, etc.) |
| **Your Turn: Submit Your First PR** | 1131 | Practice exercise — easy path and challenge path |
| **Preview: GitHub 102** | 1162 | What's coming in the next article |

### Part 1 subsections
| Topic | Line |
|-------|------|
| Create a GitHub Account | 148 |
| Install Git | 154 |
| Configure Git | 182 |
| Set Up SSH Keys | 197 |
| Install the GitHub CLI | 240 |
| Install the GitHub MCP (optional) | 259 |

### Part 2 subsections
| Topic | Line |
|-------|------|
| What is a Repository? | 293 |
| What a Repo Looks Like on GitHub | 307 |
| How to Organize Your Repos | 322 |
| Before You Create: Key Decisions | 348 |
| Your First Repo: Clone acme-ops | 380 |
| GitHub vs. Cloud Storage: When to Use Each | 425 |
| Finding and Using Other People's Repos | 452 |

### Part 3 subsections
| Topic | Line |
|-------|------|
| GitHub Is the New Google Drive (concept comparison) | 516 |
| The Short Version (6-step quick reference) | 547 |
| Step 1: Get to your branch | 597 |
| Step 2: Make your edits | 707 |
| Step 3: Commit | 715 |
| Step 4: Push | 776 |
| Step 5: Open a pull request (PR) | 793 |
| Step 6: Merge | 920 |
| Beyond the Daily Workflow | 975 |
| Sarah's Full Workflow (end-to-end example) | 999 |

## Topic Quick Lookup

If the reader asks about... → point them here:

| Question or topic | Article section | Line |
|-------------------|----------------|------|
| What is GitHub / Git? | GitHub in Plain Language | 58 |
| How do I install Git? | Install Git | 154 |
| SSH keys / permission denied | Set Up SSH Keys | 197 |
| How do I clone a repo? | Your First Repo: Clone acme-ops | 380 |
| What's a branch / how do branches work? | Step 1: Get to your branch | 597 |
| How do I commit? | Step 3: Commit | 715 |
| What's the difference between commit and push? | Step 4: Push | 776 |
| How do I open a pull request? | Step 5: Open a pull request | 793 |
| How do PRs / code review work? | Step 5: Open a pull request | 793 |
| How do I merge? | Step 6: Merge | 920 |
| What is rebasing? | Step 1: Get to your branch | 597 |
| What is stashing? | Beyond the Daily Workflow | 975 |
| Merge conflicts | When Things Go Wrong — Merge conflict | 1045 |
| Branch is behind main | When Things Go Wrong — Branch behind | 1031 |
| Detached HEAD | When Things Go Wrong — HEAD detached | 1054 |
| What is .gitignore? | .gitignore | 1099 |
| How do I fork a repo? | Forking repos | 481 |
| Public vs private repos | Before You Create: Key Decisions | 348 |
| How do I submit my first PR? | Your Turn | 1131 |
| Google Drive comparison | GitHub Is the New Google Drive | 516 |

## Common Errors — Quick Answers

These give fast answers without needing to read the full article:

- **"Your branch is behind origin/main"** → Run `git pull` or ask Claude: *"Pull the latest changes."*
- **"Merge conflict in [filename]"** → Open the file, resolve the `<<<<<<<` markers, or ask Claude: *"Resolve the merge conflicts in this file."*
- **"HEAD detached at [some hash]"** → Run `git checkout main` or ask Claude: *"I'm in a detached HEAD state, get me back to main."*
- **"Permission denied (publickey)"** → SSH key issue. Test with `ssh -T git@github.com`. See SSH setup at line 197.
- **"I accidentally cloned a repo inside another repo"** → Move the inner repo out so it sits next to the other repo, not inside it.

## Common Questions — Quick Answers

### "How do I undo my last commit?"
If you haven't pushed yet: `git reset --soft HEAD~1` (keeps your changes, removes the commit).
If you have pushed: ask Claude — it depends on whether others have pulled your changes.

### "What's the difference between pushing and opening a PR?"
Pushing uploads your work to GitHub (backup). Opening a PR asks someone to review it before merging into main.

### "My branch is behind main — how do I update it?"
Ask Claude: *"Update my branch with the latest changes from main."*

### "I accidentally committed to main instead of a branch"
Ask Claude: *"I accidentally committed to main. Help me move my changes to a new branch."*

## Key Concepts

| Term | What it means |
|------|---------------|
| Repository (repo) | A project folder tracked by Git |
| Commit | A saved snapshot of your project |
| Branch | A parallel copy for isolated work |
| Main | The official version everyone trusts |
| Pull Request (PR) | A request to review and merge changes |
| Push | Upload commits to GitHub |
| Pull | Download latest changes from GitHub |
| Merge | Combine a branch's changes into main |
| Stash | Temporarily save uncommitted changes |
| Fork | Your own copy of someone else's repo |
| Rebase | Replay your branch's commits on top of the latest main |
| Clone | Download a repo from GitHub to your machine |

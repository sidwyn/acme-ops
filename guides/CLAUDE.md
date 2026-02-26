# GitHub 101 — Quick Reference & Article Index

This file helps Claude quickly answer GitHub questions by pointing to the right section of `github-101.md`. For detailed explanations, read the full article.

## Article Map

| Section | Line | What it covers |
|---------|------|----------------|
| **GitHub in Plain Language** | 52 | What Git and GitHub are, why they matter for non-engineers, how collaboration works, Git vs GitHub |
| **Meet the Practice Repo** | 122 | Introduction to the acme-ops practice repo used throughout the article |
| **Part 1: Setup & Installation** | 138 | GitHub account, installing Git, configuring Git, SSH keys, GitHub CLI, GitHub MCP |
| **Part 2: Repositories 101** | 288 | What repos are, repo structure on GitHub, organizing repos, public vs private, cloning, forking |
| **Part 3: Daily Workflow** | 511 | The 6-step workflow (branch → edit → commit → push → PR → merge), Google Drive comparisons, deep dive on each step |
| **When Things Go Wrong** | 1037 | Common Git errors and how to fix them |
| **.gitignore** | 1111 | What files to exclude from Git (API keys, node_modules, etc.) |
| **Your Turn: Submit Your First PR** | 1143 | Practice exercise — easy path and challenge path |
| **Preview: GitHub 102** | 1174 | What's coming in the next article |

### Part 1 subsections
| Topic | Line |
|-------|------|
| Create a GitHub Account | 154 |
| Install Git | 160 |
| Configure Git | 188 |
| Set Up SSH Keys | 203 |
| Install the GitHub CLI | 246 |
| Install the GitHub MCP (optional) | 265 |

### Part 2 subsections
| Topic | Line |
|-------|------|
| What is a Repository? | 299 |
| What a Repo Looks Like on GitHub | 313 |
| How to Organize Your Repos | 328 |
| Public vs. Private repos | 358 |
| Clone acme-ops | 386 |
| GitHub vs. Cloud Storage | 431 |
| Finding and Using Other People's Repos | 458 |

### Part 3 subsections
| Topic | Line |
|-------|------|
| GitHub Is the New Google Drive (concept comparison) | 522 |
| The Short Version (6-step quick reference) | 553 |
| Step 1: Get to your branch | 603 |
| Step 2: Make your edits | 713 |
| Step 3: Commit | 721 |
| Step 4: Push | 782 |
| Step 5: Open a pull request (PR) | 799 |
| Step 6: Merge | 924 |
| Beyond the Daily Workflow | 979 |
| Sarah's Full Workflow (end-to-end example) | 1003 |

## Topic Quick Lookup

If the reader asks about... → point them here:

| Question or topic | Article section | Line |
|-------------------|----------------|------|
| What is GitHub / Git? | GitHub in Plain Language | 52 |
| Git vs GitHub — what's the difference? | Under the hood: Git vs GitHub | 106 |
| How do I install Git? | Install Git | 160 |
| SSH keys / permission denied | Set Up SSH Keys | 203 |
| How do I clone a repo? | Clone acme-ops | 386 |
| What's a branch / how do branches work? | Step 1: Get to your branch | 603 |
| How do I commit? | Step 3: Commit | 721 |
| What's the difference between commit and push? | Step 4: Push | 782 |
| How do I open a pull request? | Step 5: Open a pull request | 799 |
| How do PRs / code review work? | Step 5: Open a pull request | 799 |
| How do I merge? | Step 6: Merge | 924 |
| What is rebasing? | Step 1: Get to your branch | 603 |
| What is stashing? | Beyond the Daily Workflow | 979 |
| Merge conflicts | When Things Go Wrong — Merge conflict | 1057 |
| Branch is behind main | When Things Go Wrong — Branch behind | 1043 |
| Detached HEAD | When Things Go Wrong — HEAD detached | 1066 |
| What is .gitignore? | .gitignore | 1111 |
| How do I fork a repo? | Forking repos | 487 |
| Public vs private repos | Before You Create: Key Decisions | 354 |
| How do I submit my first PR? | Your Turn | 1143 |
| Google Drive comparison | GitHub Is the New Google Drive | 522 |

## Common Errors — Quick Answers

These give fast answers without needing to read the full article:

- **"Your branch is behind origin/main"** → Run `git pull` or ask Claude: *"Pull the latest changes."*
- **"Merge conflict in [filename]"** → Open the file, resolve the `<<<<<<<` markers, or ask Claude: *"Resolve the merge conflicts in this file."*
- **"HEAD detached at [some hash]"** → Run `git checkout main` or ask Claude: *"I'm in a detached HEAD state, get me back to main."*
- **"Permission denied (publickey)"** → SSH key issue. Test with `ssh -T git@github.com`. See SSH setup at line 203.
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

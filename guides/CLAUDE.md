# GitHub Quick Reference

This folder contains the full GitHub 101 article and this quick reference. For detailed explanations, read `github-101.md`.

## Common Questions

### "How do I undo my last commit?"
If you haven't pushed yet: `git reset --soft HEAD~1` (keeps your changes, removes the commit)
If you have pushed: ask Claude to help - it depends on whether others have pulled your changes.

### "I'm getting merge conflicts - what do I do?"
Open the file with conflicts. Look for the <<<<<<< markers. Everything between <<<<<<< and ======= is your version. Everything between ======= and >>>>>>> is the other version. Pick one, combine them, or write something new. Remove all markers. Commit. Or ask Claude: "Resolve the merge conflicts in this file."

### "What's the difference between pushing and opening a PR?"
Pushing uploads your work to GitHub (backup). Opening a PR asks someone to review it before merging into main.

### "My branch is behind main - how do I update it?"
Ask Claude: "Update my branch with the latest changes from main."

### "I accidentally committed to main instead of a branch"
Ask Claude: "I accidentally committed to main. Help me move my changes to a new branch."

## Common Errors
- "Your branch is behind origin/main" → Run `git pull`
- "Merge conflict in [filename]" → Open the file, resolve the <<<<<<< markers
- "HEAD detached" → Run `git checkout main`
- "Permission denied (publickey)" → SSH key issue, run `ssh -T git@github.com` to test

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

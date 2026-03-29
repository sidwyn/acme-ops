# Takeaways — MMoscosoCruz

I learned how GitHub works and why people use it. The article broke down the vocabulary in a way that finally made it click — branches, commits, pull requests, all of it. I also learned how to set everything up using Claude Code as my AI coding agent. The explanation in this article was top notch.

## A question I had along the way

**Q: Why do we end up on main after a merge, and is it okay to edit files directly on main?**

A: When merging a branch into main, you have to be *on* main first — that's just how Git works. But editing files directly on main is bad practice. Main should always be the clean, stable version. The right workflow is to always create a new branch, make your changes there, and open a PR to merge back into main. Branches are your workspace where it's safe to experiment without affecting main.

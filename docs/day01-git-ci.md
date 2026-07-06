# Day 1 - Git and CI Basics

## What I learned today

- `git status` shows the current state of the working tree.
- `git diff` shows unstaged changes.
- `git add` moves changes into the staging area.
- `git diff --cached` shows staged changes.
- `git commit` creates a local version snapshot.
- `git push` uploads local commits to GitHub.
- GitHub Actions runs automatic checks after code is pushed.

## Key terms

| Term | Meaning |
|---|---|
| working tree | The actual files in my local project directory |
| staging area | The area containing changes prepared for commit |
| commit | A saved snapshot in Git history |
| remote | A GitHub repository linked to my local repository |
| origin | My forked repository |
| upstream | The original repository |
| CI | Continuous Integration, automatic checks on GitHub |

## Notes from my npm audit fix

The previous CI failure was caused by `npm audit`, not by application code.
The fix updated dependency lockfiles:

- `package-lock.json`
- `packages/coding-agent/npm-shrinkwrap.json`

The lesson is: one commit should solve one clear problem.

# Rebase

Rebase is a powerful tool that allows you to rewrite commit history. It can be used to:

- Combine multiple commits into one
- Reorder commits
- Squash commits
- Edit commit messages
- Split commits
- Remove commits
- Change the base of a branch
- Resolve conflicts
- Clean up a messy history

## Rebase vs Merge

Rebase and merge are two ways to integrate changes from one branch into another. The main difference between them is how they do it. 

One benefit of rebase is that it keeps the commit history clean and linear. It makes it easier to understand the history of a project, while merge creates a more complex history with multiple branches - merge creates a merge commit, while rebase rewrites the commit history.

```bash
# Rebase the source branch onto the receiving branch (current branch)
git rebase source-branch

# Merge the source branch into the receiving branch (current branch)
git merge source-branch
```
## When to Rebase

- When you want to keep a clean and linear commit history
- When you want to avoid merge commits
- When you want to resolve conflicts in a cleaner way
```

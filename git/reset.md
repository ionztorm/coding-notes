# Reset

A `reset` is a way to move the `HEAD` to a specific commit. It's a way to undo changes you've made to a repository.

The `HEAD` is a reference to the current commit. It's a pointer to the current branch.

A `reset` can be either `soft`, `mixed`, or `hard`. The default is `mixed`.

- A `soft` reset moves the `HEAD` to a specific commit, but it doesn't change the working directory or the staging area. It's a way to undo a commit.
- A `mixed` reset moves the `HEAD` to a specific commit and changes the working directory, but it doesn't change the staging area. It's a way to undo a commit and unstage changes.
- A `hard` reset moves the `HEAD` to a specific commit and changes the working directory and the staging area. All changes made since the commit are lost permanently.

```bash
# Reset to a specific commit
git reset --soft HEAD~1

# Reset to a specific commit and unstage changes
git reset --mixed HEAD~1

# Reset to a specific commit and lose changes
git reset --hard HEAD~1
```

The `HEAD~1` is a reference to the commit before the current commit, and the `~1` means one commit before the current commit. You can also use a commit hash or a branch name.

# Push & Pull

## Push
```bash
git push origin main
```
Git push is used to upload local repository content to a remote repository. Pushing is how you transfer commits from your local repository to a remote repository.

You can also push a local branch to a remote branch with a different name:

```bash
git push origin local-name:remote-name
```

We can also delete a remote branch by pushing an empty branch to it:

```bash
git push origin :remote-name
```

## Pull
```bash
git pull [remote-name]/[branch-name]
```
Remote name and branch name are optional. If you don't specify them, Git will use the default remote and branch.

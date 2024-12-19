# Remote

A remote is just another repo. Convention is that when treating a remote as the source of truth, we name it 'origin'.

The origin remote would be the one that all of the team treat as the source of truth and contains all the most up to date accepted code.

## Adding a remote

```bash
git remote add <name> <uri>
```

The name can be anything, but for the source of truth, we use 'origin'.
The `uri` is the path to the repo. This can be a local directory, or it could be online, such as using github.

## Fetching remote contents.

```bash
git fetch
```

Fetch downloads copies of the contents of the `.git/objects` directory from the remote repo into the current repo.

This fetches the metadata from the remote, but it doesn't copy all the files.

## Log Remote

Git log can be used to log the commits from remote repos too...

```bash
git log remote/branch
```

## Merge

We can use merge to merge local branches between local and remote.

```bash
git merge remote/branch
```



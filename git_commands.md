# Git Commands

I tend to use the Git tools that come with Visual Studio and Visual Studio Code, however, there's a few snippets I use at the command line.

## Snippet:

```
git fetch --prune
```

## Description:

Along with fetching, also removes references to remote branches that no longer exist.

## Snippet:

```
git branch | grep -v '^*' | xargs git branch -d
```

## Description:

Removes all local branches other than the current branch.  If you want to force the deletion of the other branches, use:

```
git branch | grep -v '^*' | xargs git branch -D
```

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

## Snippet:

```
git rebase -i HEAD~3
```

## Description:

Start an interactive rebase so you can squash your commits

## Snippet:

```
git commit --amend --reset-author
```

## Description:

Above can be used to reset the commit date (useful to do after squashing commits)

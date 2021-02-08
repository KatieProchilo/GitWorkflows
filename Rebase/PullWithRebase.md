# Pull with rebase

Configure Git to pull with rebase by default for the current repository:

```bash
git config pull.rebase true
```

Or configure Git to pull with rebase for all the current user's repositories:

```bash
git config --global pull.rebase true
```

## Background

When you run `git pull`, Git execute two commands behind the scenes. With default configuration, these commands are:

```bash
git fetch
git merge FETCH_HEAD
```

It's also possible to pull with rebasing by running `git pull --rebase`, which executes:

```bash
git fetch
git rebase
```

***

*[Return home.](../README.md)*

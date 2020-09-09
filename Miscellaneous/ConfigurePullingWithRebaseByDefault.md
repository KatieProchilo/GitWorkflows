# Configure pulling with rebase by default

When you execute the `git pull` command, Git execute two commands behind the scenes. With default configuration, these
commands are:

```bash
git fetch
git merge FETCH_HEAD
```

It's also possible to pull with rebasing by running `git pull --rebase`, which executes:

```bash
git fetch
git rebase
```

To pull with rebase by default, you will want to run **one** of the following commands depending on your scenario:

| I want to change the default pull behavior for . . . | Command                                                |
| ---------------------------------------------------- | ------------------------------------------------------ |
| all the current user's repositories.                 | `git config --global pull.rebase true`                 |
| a specific repository.                               | `git config pull.rebase true`                          |
| all new tracking branches in a specific repository.  | `git config branch.autosetuprebase always`             |
| a specific branch in a specific repository.          | `git config branch.<BRANCH_NAME>.rebase true`          |

***

*[Return home.](../README.md)*

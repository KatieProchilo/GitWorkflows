# Configure Git globally

> ***WARNING!*** These configurations are opinionated and may not be what you want every single time. Know what you're
> doing, but also totally do it 😎

Overwrite some default Git configurations. Remove the `--global` flag from any commands to apply the
configuration for only the current repository:

```bash
# Pull with rebase:
git config --global pull.rebase true
# Prune on fetch:
git config --global fetch.prune true
```

<!--
TODO:

rebase.autostash

git config –global push.default simple

# always have Linux line endings in text files
git config --global core.autocrlf input

# support more than 260 characters on Windows
# See https://stackoverflow.com/a/22575737/873282 for details
git config --global core.longpaths true

# some color and diff tweaks
#   Use SVN's ||| also in git
#   See https://git-scm.com/docs/git-config#Documentation/git-config.txt-mergeconflictStyle for details

git config --global merge.configStyle "diff3"

git config --global color.diff.new "green bold"

git config --global color.status.updated "green bold"

git config --global color.branch.current "green bold"

# Sort branches at "git branch -v" by committer date
git config --global branch.sort -committerdate

VETOED RECOMMENDATIONS SO FAR:

# Different diff color for lines that moved but are otherwise unchanged:
# (Don't use git diff ever, but maybe working with VS people do?)

git config --global diff.colorMoved zebra
-->

***

*[Return home](../README.md) or view related workflows:*

- [Configure the upstream](../Forks/ConfigureTheUpstream.md)
- [Pull with rebase](../Rebase/PullWithRebase.md)
- [Rename the master branch to main](RenameTheMasterBranchToMain.md)

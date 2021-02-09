# Rebase onto the upstream

Rebase changes from **featureBranch** of a fork onto **upstream/main**:

```bash
git checkout featureBranch
git fetch upstream
git rebase upstream/main
# Solve any conflicts and run the following two commands as many times as needed:
git add .
git rebase --continue
```

***

*[Return home](../README.md) or view related workflows:*

- [Configure the upstream](ConfigureTheUpstream.md)
- [Delete an upstream branch](DeleteAnUpstreamBranch.md)
- [Pull from the upstream](PullFromTheUpstream.md)
- [Pull with rebase](../Rebase/PullWithRebase.md)
- [Push to the upstream](PushToTheUpstream.md)

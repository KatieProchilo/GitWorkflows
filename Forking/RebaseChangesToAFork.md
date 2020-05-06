# Rebase Changes to a Fork

Get changes from **upstream/featureBranch** into the local branch **featureBranch** of the **forked repository**. Get these changes without merge commits.

### Solution

Fetch the branches of the **upstream repository** into remote-tracking branches such as **upstream/featureBranch**:

```bash
git fetch upstream
```

Checkout **featureBranch** and rebase it against **upstream/featureBranch**:

```bash
git checkout featureBranch
git rebase upstream/featureBranch
```

Solve any conflicts.

Overwrite **origin/featureBranch**:

```bash
git push -f origin featureBranch
```

### More Workflows

* [Configure a Fork](ConfigureAFork.md)
* [Pull Changes to a Fork](PullChangesToAFork.md)
* [Pull Request Changes From a Fork](PullRequestChangesFromAFork.md)

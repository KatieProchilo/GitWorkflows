# Pull Changes to a Fork

Get changes from **upstream/featureBranch** into the local branch **featureBranch** of the **forked repository**.

### Solution

Pull from the **upstream repository** into the **featureBranch** branch of your local **forked repository**:

```bash
git pull upstream featureBranch
```

Solve any conflicts.

Overwrite **origin/featureBranch**:

```bash
git push origin featureBranch
```

### More Workflows

* [Configure a Fork](ConfigureAFork.md)
* [Pull Request Changes From a Fork](PullRequestChangesFromAFork.md)
* [Rebase Changes to a Fork](RebaseChangesToAFork.md)

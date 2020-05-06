# Pull Request Changes From a Fork

[Configure a **forked repository**](ConfigureAFork.md) if not done already.

[Pull](PullChangesToAFork.md) or [rebase](RebaseChangesToAFork.md) the latest changes from **upstream/master** into the **master** branch of your local **forked repository**.

Create a local **featureBranch**:

```bash
git checkout -b featureBranch master
```

Make some changes and commit them:

```bash
git add .
git commit -m "Some changes."
```

Push **featureBranch** to **origin**, the remote for your **forked repository**:

```bash
git push origin featureBranch
```

Navigate to the **base repository**, and you should see the below pop-up. Click **Compare & pull request** to create a pull request from **origin/featureBranch**:

![Recently Pushed Branches for a Forked Repository](images/ForkRecentlyPushedBranches.png)

Approve the pull request. Resolve any merge conflicts or [rebase your changes](RebaseChangesToAFork.md) against the latest in **upstream/master**, then merge the pull request.

### More Workflows

* [Configure a Fork](ConfigureAFork.md)
* [Pull Changes to a Fork](PullChangesToAFork.md)
* [Rebase Changes to a Fork](RebaseChangesToAFork.md)

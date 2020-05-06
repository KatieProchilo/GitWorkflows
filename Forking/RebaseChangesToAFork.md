# Rebase Changes to a Fork

[Configure a **forked repository**](ConfigureAFork.md) if not done already.

### Problem

The branch **myBranch** from the **base repository** has some changes I want in a branch of my **forked repository**. I want these changes without merge commits.

### Solution

Fetch the branches of the remote called **upstream** into remote-tracking branches such as **upstream/myBranch**:

```bash
git fetch upstream
```

Checkout the local **myBranch** and rebase it against the newly fetched remote-tracking branch **upstream/myBranch**:

```bash
git checkout myBranch
git rebase upstream/myBranch
```

Overwrite **origin's** version of **myBranch**:

```bash
git push -f origin myBranch
```

### More Workflows

* [Configure a Fork](ConfigureAFork.md)
* [Pull Changes to a Fork](PullChangesToAFork.md)
* [Pull Request Changes From a Fork](PullRequestChangesFromAFork.md)

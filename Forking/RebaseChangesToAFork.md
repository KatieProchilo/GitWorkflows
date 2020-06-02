# Rebase changes to a fork

Get changes from **upstream/featureBranch** into the local branch **featureBranch** of the **forked repository**. Get these changes without merge commits.

1. Fetch the branches of the **upstream repository** into remote-tracking branches such as **upstream/featureBranch**:

    ```bash
    git fetch upstream
    ```

2. Checkout **featureBranch** and rebase it against **upstream/featureBranch**:

    ```bash
    git checkout featureBranch
    git rebase upstream/featureBranch
    ```

3. Solve any conflicts.

4. Overwrite **origin/featureBranch**:

    ```bash
    git push -f origin featureBranch
    ```

### More Workflows

* [Checkout a branch from another person's fork](CheckoutABranchFromAnotherPersonsFork.md)
* [Configure a fork](ConfigureAFork.md)
* [Pull changes to a fork](PullChangesToAFork.md)
* [Pull request changes from a fork](PullRequestChangesFromAFork.md)

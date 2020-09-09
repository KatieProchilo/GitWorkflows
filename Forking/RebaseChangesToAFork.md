# Rebase changes to a fork

Get changes without merge commits from **upstream/featureBranch** into **featureBranch** of the fork.

1. Fetch the branches of the upstream into remote-tracking branches such as **upstream/featureBranch**:

    ```bash
    git fetch upstream
    ```

2. Checkout **featureBranch**, then rebase it against **upstream/featureBranch**:

    ```bash
    git checkout featureBranch
    git rebase upstream/featureBranch
    ```

3. Solve any conflicts.

4. Overwrite **origin/featureBranch**:

    ```bash
    git push -f origin featureBranch
    ```

## More Workflows

- [Checkout a branch from a fork to another fork](CheckoutABranchFromAForkToAnotherFork.md)
- [Checkout a branch to a fork](CheckoutABranchToAFork.md)
- [Configure a fork](ConfigureAFork.md)
- [Pull changes to a fork](PullChangesToAFork.md)
- [Push changes from a fork](PushChangesFromAFork.md)

# Pull changes to a fork

Get the changes from some remote branch from the upstream repository into a local branch of your fork:

1. Pull from the upstream into a **featureBranch** of a fork:

    ```bash
    git pull upstream featureBranch
    ```

1. Solve any conflicts.

1. Push **origin/featureBranch**:

    ```bash
    git push origin featureBranch
    ```

## More Workflows

- [Checkout a branch from a fork to another fork](CheckoutABranchFromAForkToAnotherFork.md)
- [Checkout a branch to a fork](CheckoutABranchToAFork.md)
- [Configure a fork](ConfigureAFork.md)
- [Push changes from a fork](PushChangesFromAFork.md)
- [Rebase changes to a fork](RebaseChangesToAFork.md)

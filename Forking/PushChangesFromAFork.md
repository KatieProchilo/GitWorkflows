# Push changes from a fork

Submit changes from a fork to the upstream repository:

1. [Configure a **forked repository**](ConfigureAFork.md) if not done already.

1. [Pull](PullChangesToAFork.md) or [rebase](RebaseChangesToAFork.md) the latest changes from **upstream/master** into
the **master** branch of your local **forked repository**.

1. Create a local **featureBranch**:

    ```bash
    git checkout -b featureBranch master
    ```

1. Make some changes and commit them:

    ```bash
    git add .
    git commit -m "Some changes."
    ```

1. Push **featureBranch** to **origin**, the remote for your **forked repository**:

    ```bash
    git push origin featureBranch
    ```

## More Workflows

* [Checkout a branch from a fork to another fork](CheckoutABranchFromAForkToAnotherFork.md)
* [Checkout a branch to a fork](CheckoutABranchToAFork.md)
* [Configure a fork](ConfigureAFork.md)
* [Pull changes to a fork](PullChangesToAFork.md)
* [Rebase changes to a fork](RebaseChangesToAFork.md)

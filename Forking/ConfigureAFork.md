# Configure a fork

Start with an upstream repository you would like to fork. To configure a fork from this repository:

1. Create a fork from the upstream repository.

1. Clone the fork. When you clone a fork, a default remote reference called **origin** is automatically configured to
track it.

1. Add another remote called **upstream** that is set to track the upstream repository:

    ```bash
    git remote add upstream https://github.com/KatieProchilo/GitWorkflows.git
    ```

## More Workflows

- [Checkout a branch from a fork to another fork](CheckoutABranchFromAForkToAnotherFork.md)
- [Checkout a branch to a fork](CheckoutABranchToAFork.md)
- [Pull changes to a fork](PullChangesToAFork.md)
- [Push changes from a fork](PushChangesFromAFork.md)
- [Rebase changes to a fork](RebaseChangesToAFork.md)
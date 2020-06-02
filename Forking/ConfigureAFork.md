# Configure a fork

Start with a repository you would like to fork. We'll call this the **upstream repository**. [Create a fork](https://help.github.com/en/github/getting-started-with-github/fork-a-repo) from this repository that we'll refer to as the **forked repository**.

1. [Clone the **forked repository**](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository) to your local machine. When you clone the **forked repository**, a remote is configured and its name is set to **origin** by default.

1. Now add another remote called **upstream** that is set to track the **upstream repository**:

    ```bash
    git remote add upstream https://github.com/KatieProchilo/GitWorkflows.git
    ```

Now you're ready to explore other forking workflows.

### Forking Workflows

These workflows have guidance specific to forks with two remotes called **origin** and **upstream**:

* [Checkout a branch from another person's fork](CheckoutABranchFromAnotherPersonsFork.md)
* [Pull changes to a fork](PullChangesToAFork.md)
* [Pull request changes from a fork](PullRequestChangesFromAFork.md)
* [Rebase changes to a fork](RebaseChangesToAFork.md)
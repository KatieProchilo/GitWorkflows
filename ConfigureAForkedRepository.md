# Configure a Forked Repository

Start with a repository you would like to fork. We'll call this the **base repository**. [Create a fork](https://help.github.com/en/github/getting-started-with-github/fork-a-repo) from this repository that we'll call the **forked repository**.

[Clone the **forked repository**](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository) to your local machine. When you clone the **forked repository**, a remote is configured and its name is set to **origin** by default.

Now add another remote called **upstream** that is set to track the **base repository**:

```bash
git remote add upstream https://github.com/KatieProchilo/GitWorkflows.git
```

Now you're ready to explore other forking workflows.

### Forking Workflows

These workflows have guidance specific to forks with two remotes called **origin** and **upstream**:

* [Pull Changes to a Fork](PullChangesToAFork.md)
* [Pull Request Changes From a Forked Repository](PullRequestChangesFromAForkedRepository.md)
* [Rebase Changes to a Fork](RebaseChangesToAFork.md)
# Pull Request Changes From a Forked Repository

[Configure a **forked repository**](ConfigureAForkedRepository.md) if not done already.

To get the latest changes from the **base repository**, whose remote is called **upstream**, into the **master** branch of your local **forked repository**:

```bash
git pull upstream master
```

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

Approve the pull request. If needed, resolve merge conflicts or [rebase changes](RebaseABranch.md).

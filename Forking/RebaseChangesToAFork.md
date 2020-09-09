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

***

*[Return home.](../README.md)*

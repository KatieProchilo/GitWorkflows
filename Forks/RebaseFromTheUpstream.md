# Rebase from the upstream

Rebase changes from **featureBranch** of a fork onto **upstream/featureBranch**.

1. Fetch **upstream** branches into remote-tracking branches like **upstream/featureBranch**:

    ```bash
    git fetch upstream
    ```

1. Checkout **featureBranch**, then rebase it onto **upstream/featureBranch**:

    ```bash
    git checkout featureBranch
    git rebase upstream/featureBranch
    ```

1. Solve any conflicts.

1. Overwrite **origin/featureBranch**:

    ```bash
    git push -f origin featureBranch
    ```

***

*[Return home.](../README.md)*

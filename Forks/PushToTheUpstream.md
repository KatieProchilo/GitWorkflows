# Push to the upstream

Submit changes from a fork to the upstream repository:

1. [Configure the upstream](ConfigureTheUpstream.md) if not done already.

1. [Pull](PullFromTheUpstream.md) or [rebase](RebaseFromTheUpstream.md) the latest changes from **upstream/main** into the
   **main** branch of your fork.

1. Create **featureBranch**:

    ```bash
    git checkout -b featureBranch main
    ```

1. Commit some changes:

    ```bash
    git add .
    git commit -m "Some changes."
    ```

<!-- TODO: THIS IS NOT WHAT THIS PAGE SAYS IT'S DOING - IT'S PUSHING TO ORIGIN NOT UPSTREAM -->

1. Push **featureBranch** to **origin**:

    ```bash
    git push origin featureBranch
    ```

***

*[Return home.](../README.md)*

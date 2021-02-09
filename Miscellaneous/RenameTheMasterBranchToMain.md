# Rename the master branch to main

Rename the default branch from **master** to **main**:

1. Update your local **master** branch:

    ```bash
    git checkout master
    git pull
    git push
    ```

1. Rename your **master** branch to **main**:

    ```bash
    git branch -m master main
    ```

1. Push the new **main** branch:

    ```bash
    git push -u origin main
    ```

1. On your preferred Git provider, update the default branch from **master** to **main**. On GitHub this can be found
   under **Settings**, then click **Branches** in the **Options** menu. Update any branch protection rules for
   **master** so that they apply to **main** instead.

1. Delete the remote **master** branch:

    ```bash
    git push --delete origin master
    ```

1. Set the remote **HEAD**:

    ```bash
    git remote set-head origin --auto
    ```

1. Update any infrastructure that depends on the **master** branch by name, such as CI/CD, configuration files, badges,
   or anywhere else information might be hard-coded.

***

*[Return home](../README.md) or view related workflows:*

- [Configure Git globally](ConfigureGitGlobally.md)
- [Configure the upstream](../Forks/ConfigureTheUpstream.md)
- [Pull with rebase](../Rebase/PullWithRebase.md)

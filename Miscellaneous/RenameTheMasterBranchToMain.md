# Rename the `master` branch to `main`

Start with a repository you own whose default branch you would like to rename from `master` to `main`:

1. Update your local `master` branch:

    ```bash
    git checkout master
    git pull
    git push
    ```

1. Rename your `master` branch to `main`:

    ```bash
    git branch -m master main
    ```

1. Push the new `main` branch:

    ```bash
    git push -u origin main
    ```

1. On your preferred Git provider, update the default branch from `master` to `main`. On GitHub this can be found under
**Settings**, then click **Branches** in the **Options** menu. Update any branch protection rules for `master` so that
they now apply to `main`.

1. Delete the remote `master` branch:

    ```bash
    git push --delete origin master
    ```

1. Set the remote HEAD:

    ```bash
    git remote set-head origin --auto
    ```

Be sure to update any other infrastructure that depends on the `master` branch by name, such as CI/CD, configuration
files, badges, or anywhere else information might be hard-coded.

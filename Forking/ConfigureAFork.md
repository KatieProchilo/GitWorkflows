# Configure a fork

Start with an upstream repository you would like to fork. To configure a fork from this repository:

1. Create a fork from the upstream repository.

1. Clone the fork. When you clone a fork, a default remote reference called **origin** is automatically configured to
track it.

1. Add another remote called **upstream** that is set to track the upstream repository:

    ```bash
    git remote add upstream https://github.com/KatieProchilo/GitWorkflows.git
    ```

***

*[Return home.](../README.md)*

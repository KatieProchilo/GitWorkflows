# Pull Changes to a Fork

[Configure a **forked repository**](ConfigureAFork.md) if not done already.

### Problem

The branch **myBranch** from the **base repository** has some changes I want in a branch of my **forked repository**.

### Solution

Pull from the **base repository**, whose remote is called **upstream** into the **myBranch** branch of your local **forked repository**:

```bash
git pull upstream myBranch
```

Overwrite the remote **myBranch** branch of your **forked repository**:

```bash
git push origin myBranch
```

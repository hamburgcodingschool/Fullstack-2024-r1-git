### How to write good commit messages?

For choosing a good commit message, you try to answer the following w questions:

- **what**: fix, feature, delete, add
- **where**: the file or element you changed (e.g. Button)
- **who**: included already (git author)
- **how**: what exactly did you change?
- **when**: included already (commit timestamp)
- **why**: "in order to"
- (optional): reference to GitHub issue

**Example:**
> fix(Button): change spacing in order to improve usability #25

You usually use present tense in commit messages.

Popular standard: Angular commit message guidelines  
https://github.com/angular/angular/blob/master/CONTRIBUTING.md#commit

If you use `fix` or `closes` in your commit message and reference a GitHub issue, it automatically creates a reference and closes the issue.


---

[Next](18-cherry-picking.md)

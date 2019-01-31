## Revert Commits

You want to remove the changes of a certain commit, follow these steps:
```
git log
```
This will look like:
```
...
commit c135432a890f38e4d240af80858a3574bca0ed29
Author: Teresa Holfeld <teresaholfeld@users.noreply.github.com>
Date:   Sat Jan 19 10:54:19 2019 +0100
```
Copy the hash of the commit you want to remove. In this case, this would be `c135432a890f38e4d240af80858a3574bca0ed29`.
```
git revert <git hash>
```
In this case, this would be:
```
git revert c135432a890f38e4d240af80858a3574bca0ed29
```
This will create a new commit. This is important so that you know where in the history the commit was reverted. To approve the commit message, type:
```
:x
```

---

[Next](07-branching-strategies.md)

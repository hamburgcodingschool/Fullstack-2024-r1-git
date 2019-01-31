## Rebase

Sometimes you have the following situation:  
Your branch has changes, but master also has changes.  
You don't want to merge master into your branch, but you want your branch to build on the newest commits on master.  

With `rebase` you can take your branch and put it on the latest commits on master.

```
git rebase master
```

There is also an interactive mode for rebasing. With that, you can make even more things with it, e.g. rewrite the commit history.

```
git rebase HEAD~3 -i
```
This opens a vim editor, that looks something like this:

```
pick f7f3f6d changed my name a bit
pick 310154e updated README formatting and added blame
pick a5f4a0d added cat-file

# Rebase 710f0f8..a5f4a0d onto 710f0f8
# ...
```

There, you can, for example, squash multiple commits to one.    
You do this by changing the prefix that is currently `pick`.  

`pick` will keep that commit with that commit message.

`amend` will let you change the commit or commit message.

`squash` will put the changes in that commit into the one with `pick`.

`drop` lets the commit disappear, as if it was never there.

For more information on this, refer to the git documentation:  
https://git-scm.com/book/en/v2/Git-Tools-Rewriting-History

If there are conflicts, you need to solve them, add the files, and do
```
git rebase --continue
```

---

[Next](15-resolving-conflicts.md)

### Reset

To reset the last commit, do:
```
git reset HEAD
```

If you are sure and you want to discard the commit, you can do instead:
```
git reset HEAD --hard
```

To go back 3 commits:
```
git reset HEAD~3
```

To clean up untracked files, do:
```
git clean -df
```

With `git reset` you can go back to previous commits, and create a new branch there.

---

[Next](14-git-rebase.md)


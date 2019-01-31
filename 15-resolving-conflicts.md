### Solving conflicts

If you rebase or merge, git might complain about conflicts.

There are conflicts, if the same file has changes at the same place, both on the original and the target branch. In this case, git doesn't know which one it should keep and which it should discard, so it reports a conflict.

Git annotates conflicts like this:
```
<<<<<<< (HEAD)
In this line I added an emoji behind the dot. 😊 
=======
In this line I added a different emoji behind the dot. 🤷‍♀️ 
>>>>>>> (master)
```

You as the human have to look at it, decide which you want to keep, and remove the markers (<<<===>>>).

Then add the file with `git add <filename>`.


---

[Next](16-amend-a-commit.md)

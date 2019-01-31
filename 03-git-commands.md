## Git Commands

**Create a new git project / initialize git:**
```
git init
```
**What's the status in this git project?**
```
git status
```
Green means: it has been staged for commit (git knows this change).  
Red means: it has not been staged and would not be committed.

**See what changed:**
```
git diff
```
**Add a change to git for the next commit:**  
This command stages the changed file for the next commit.
```
git add <filename>
```
If you worked on the file `index.html` and you want to add it, you would do it with:
```
git add index.html
```
Add all files that you have been working on:
```
git add .
```
**Make a git commit:**
```
git commit
```
This will open vim, and will ask you to type a commit message. Write the commit message and close with `:x`.

If you don't want to use vim, you can use the command:
```
git commit -m "Your commit message"
```
It is good practice to choose a commit message that is simple and describes precisely what has been changed.

**See the history of commits:**
```
git log
```

**Get help:**
```
git --help
```

---

[Next](04-git-config.md)

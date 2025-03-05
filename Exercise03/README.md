# Exercise 03: Basic Branching

## The task

You again live in your own branch, this time we will be doing a bit of juggling with branches, to show how lightweight branches are in git.
Hint: `git switch` will make you switch from one branch to another.

1. Use `git branch mybranch` to create a new branch called _mybranch_
2. Use `git branch` again to see the new branch created.
3. Use `git switch mybranch` to switch to your new branch.
4. Create a file called `file1.txt` with your name.
5. `Add` the file and `commit` with this change.
6. Use `git log --oneline --graph` to see your branch pointing to the new commit.
7. Switch back to the branch called _main_.
	- Use `git log --oneline --graph` and notice how the commit you made on the _mybranch_ branch is missing on the _main_ branch.
8. Make a new file called `file2.txt` and commit that file.
	- Use `git log --oneline --graph --all` to see your branch pointing to the new commit, and that the two branches now have different commits on them.
9. Switch to your branch _mybranch_.
	- What happened to your working directory? Can you see your `file2.txt`?
10. Use `git diff mybranch main` to see the difference between the two branches.

## Useful commands

- `git switch`
- `git switch -c`
- `git log --oneline --graph`
- `git branch`
- `git diff`

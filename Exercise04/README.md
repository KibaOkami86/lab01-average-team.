# Exercise 04: Fast-forward Merge

## The task

You again live in your own branch, this time we will be doing a bit of juggling with branches, to show how lightweight branches are in git.

1. Create, add and commit in the main branch a file named `greeting.txt` containing some greeting text
2. Create a (feature)branch called `feature/uppercase` (yes, `feature/uppercase` is a perfectly legal branch name, and a common convention).
3. Switch to this branch
	- What is the output of `git status`?
4. Edit the greeting.txt to contain an uppercase greeting
5. Add `greeting.txt` files to staging area and commit
	- What is the output of `git branch`?
	- What is the output of `git log --oneline --graph --all`

   *Remember: You want to update the master branch so it also has all the changes currently on the feature branch. The command 'git merge [branch name]' takes one branch as argument from which it takes changes. The branch pointed to by HEAD (currently checked out branch) is then updated to also include these changes.*

6. Switch to the `main` branch
7. Use `cat` to see the contents of the greetings
8. Diff the branches
9. Merge the branches
	- Use `cat` to see the contents of the greetings
10. Delete the uppercase branch

## Useful commands

- `git branch`
- `git branch <branch-name>`
- `git branch -d <branch-name>`
- `git switch`
- `git branch -v`
- `git add`
- `git commit`
- `git commit -m`
- `git merge <branch>`
- `git diff <branchA> <branchB>`
- `git log --oneline --graph --all`

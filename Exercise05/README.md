# Exercise 05: 3-way Merge

## The task

1. Create, add and commit in the main branch a file named `greeting.txt` containing some greeting text
2. Create a branch called greeting and switch to it
3. Edit the greeting.txt to contain your favorite greeting
4. Add greeting.txt files to the staging area
5. Commit
6. Switch back to the main branch
7. Create a file INFO.md with information about this repository
8. Add the INFO.md file to staging area and make the commit
	- What is the output of `git log --oneline --graph --all`?
9. Diff the branches
10. Merge the greeting branch into main
	- What is the output of `git log --oneline --graph --all` now? Observe the extra merge commit created with the message "Merge branch 'greeting'".

## Useful commands

- `git branch`
- `git branch <branch-name>`
- `git branch -d <branch-name>`
- `git switch <branch-name>`
- `git switch -c <branch-name>`
- `git branch -v`
- `git add`
- `git commit`
- `git commit -m`
- `git merge <branchA> <branchB>`
- `git diff <branchA> <branchB>`
- `git log --oneline --graph --all`

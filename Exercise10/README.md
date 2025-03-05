# Exercise 10: Basic cleaning

We'll work a bit with the `.gitignore` file in this exercise.
In this file you can specify both file extensions and folder structures that you do not want Git to track.
You can still `git add` files and folder that are ignored in the `.gitignore` file.

We will also work with `git rm`, which is the Git remove command. `git rm` does just the same as removing a file from your working directory, and then staging that change by issuing a `git add filename` on the file that was just deleted.
Sometimes you add a file by accident that was not meant for Git e.g. binary files, class files etc.

If you want to signal to Git that a file needs to be removed from git, but still want it in your working directory, then use `git rm --cached` to issue a remove command on the staging area, but not in your working directory.

## The task

1. Create, add and commit in the main branch a file named `file1.txt` containing some greeting text
2. Create a file with the name `foo.s`
	- What is the output of `git status`?
4. Create a `.gitignore` file in your working directory containing `*.s`
	- What is the output of `git status`?
5. Commit the `.gitignore` file and commit `file1.txt`
6. Add `txt` files to `.gitignore` by adding a line in the file containing `*.txt`
	- What does `git status` tell us?
7. Change `file1.txt`
	- What does `git status` tell us? Why was the file tracked even though the `txt` extension is in the ignore file?
8. Make another text file in the repository, what does `git status` look like now? Why is it not tracked?
9. Stage the removal of `file1.txt` with the command `git rm --cached`
	- What does `git status` say?
10. Create a new file called `file2.txt` and add the line `!file2.txt` to `.gitignore`. (See _note_ below)
	- What does `git status` say? Can you think of a use-case for keeping track of a file although the extension is ignored?

## Note
If you are using `zsh` instead of `bash`(default on Mac and some Linux') then `echo "!file2.txt" >> .gitignore` will fail because of shell expansion. Either use an editor to modify the file or escape the `!` e.g. `echo "\!file2.txt" >> .gitignore`

## Useful commands
- `git rm`
- `git add`
- `git commit`
- `git commit -m`
- `git rm --cached`


## Aliases
You can set up aliases as such:
`git config --global alias.lol 'log --oneline --graph --all'`
This might be useful to you.
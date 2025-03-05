# Exercise 02: Basic Commits
This lab will introduce you to the `git add` and `git commit` commands.

This is a very introductory exercise. If you have used `git status`, `git log --oneline --graph`, `git add` and `git commit` you should have no problem with it.

You can look at the bottom of this file, if you have not yet done basic git configuration.

## The task

1. Create a file named `myfile.txt` with some content in it
2. `add` the file to the staging area
3. `commit` the file to the repository
4. Change the content of the file you created earlier
	- What does `git diff` tell you?
	- What does `git diff --staged` tell you? why is this blank?
5. Run `git add myfile.txt` to stage your changes from the working directory.
	- What does `git diff` tell you?
	- What does `git diff --staged` tell you?
6. Overwrite the content in `myfile.txt`: `echo 3 > myfile.txt` to change the state of your file in the working directory.
	- What does `git diff` tell you?
	- What does `git diff --staged` tell you?
7. Run `git status` and observe that `myfile.txt` are present twice in the output.
8. Run `git restore --staged myfile.txt` to unstage the change
	- What does `git status` tell you now?
9. Stage the change and make a commit
10. What does the log look like?

## Useful commands
- `git add`
- `git commit`
- `git commit -m "My commit message"`
- `git log`
- `git log -n 5`
- `git log --oneline`
- `git log --oneline --graph`
- `touch filename` to create a file (or `sc filename ''` in PowerShell)
- `echo content > file` to overwrite file with content (or `sc filename 'content'` in PowerShell)
- `echo content >> file` to append file with content (or `ac filename 'content'` in PowerShell)


## Git Initial Configuration
1. `git config --global user.name "John Doe"`
1. `git config --global user.email "johndoe@example.com`

For the vim scared:
- `git config --global core.editor nano`

For the windows peeps:
- `git config --global core.editor notepad`

Other editor options:
- `git config --global core.editor "atom --wait"`
- `git config --global core.editor "code --wait"`
- `git config --global core.editor "'C:/Program Files/Notepad++/notepad++.exe' -multiInst"`

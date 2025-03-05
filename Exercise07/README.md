# Exercise 07: Basic revert

## The task

1. Execute the following commands in a Git Bash
```
touch greeting.txt
git add greeting.txt
git commit -m "Add file greeting.txt"
echo "supersecretpassword" > credentials.txt
git add credentials.txt
git commit -m "Add credentials to repository"
echo "Original file content" > greeting.txt
git add greeting.txt
git commit -m "Add content to greeting.txt"
echo "This should have been appended to the original content, rather than overwriting it." > greeting.txt
git add greeting.txt
git commit -m "Overwrite greeting.txt"
```

2. Use `git log --oneline` to look at the history
3.  Use `cat` to view the content of `greeting.txt`
4.  Use `git revert` on the newest commit, to remove the changes the last commit added
5.  Use `git log --oneline` to view the history
	- Did the revert command add or remove a commit?
6.  Use `cat` to view the content of `greeting.txt`
	- Use `ls` to see the content of the workspace
	- Use `git log --oneline` to find the sha of the commit adding credentials to the repository
7.  Use `git revert` to revert the commit that added the credentials
	- Use `git log --oneline` to view the history
	- Use `ls` to see the content of the workspace
8. How many commits were added or changed by the last revert?
9. Use `git show` with the sha of the commit you reverted to see that the credentials file is stilll in the history
10. As you have now reverted the credentials file, so it is removed from your working directory, is it also removed from git?

## Useful commands
- `git revert <ref>`
- `git log --oneline`
- `git show <ref>`

# Exercise 08: Git reset

## The task

1. Execute the following commands in a Git Bash
```
echo "1" > 1.txt
git add 1.txt
git commit -m "1"
echo "2" > 2.txt
git add 2.txt
git commit -m "2"
echo "3" > 3.txt
git add 3.txt
git commit -m "3"
echo "4" > 4.txt
git add 4.txt
git commit -m "4"
echo "5" > 5.txt
git add 5.txt
git commit -m "5"
echo "6" > 6.txt
git add 6.txt
git commit -m "6"
echo "7" > 7.txt
git add 7.txt
git commit -m "7"
echo "8" > 8.txt
git add 8.txt
git commit -m "8"
echo "9" > 9.txt
git add 9.txt
git commit -m "9"
echo "10" > 10.txt
git add 10.txt
git commit -m "10"

```
How does your working directory look like?

2. What does your log look like? What does your stage look like?
3. Try to run `git reset --soft HEAD~1`
4. What happens to your working directory, your log and your stage?
5. Run `git reset --mixed HEAD~1`
6. What happens to your working directory, your log and your stage?
7. Run `git reset --hard HEAD~1`
8. What happens to your working directory, your log and your stage?
9. Now try to use `git revert HEAD~1`
10. What happens to your working directory, your log and your stage?

## Useful commands

- `git log --oneline`
- `git commit --amend`
- `git status`
- `git reset --soft`
- `git reset --mixed`
- `git reset --hard`
- `git revert`

## Further explanation

The following is taken from Recap section of [https://git-scm.com/book/en/v2/Git-Tools-Reset-Demystified].
The reset command overwrites these three trees in a specific order, stopping when you tell it to:
1. Move what the branch HEAD points to (stop here if --soft)
2. Make the stage look like HEAD (stop here unless --hard)
3. Make the working directory look like the stage

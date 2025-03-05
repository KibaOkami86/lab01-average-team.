# Exercise 09: Basic cleaning

## The task

1. Execute the following commands in a Git Bash
```
mkdir src

echo "** SOME USEFUL INFO ** " > README.txt
echo "// awesome C code " > src/myapp.c
echo "// awesome C header " > src/myapp.h

git add src/myapp.* README.txt
git commit -m "C code for my app"

echo "// awesome C library  " > src/mylib.c

touch src/myapp.c~ src/oldfile.c~ 
touch README.txt~
mkdir obj
touch obj/mylib.o obj/mylib.a obj/myapp.o obj/a.out
```
You are working on a project that involves generated files.  Say you are compiling C files into object files. Before checking out a new branch you want to start clean

2. Explore the directory with `ls -R`. There is a lot going on.  Code files, temp files, object files,..  Let's clean up!
3. Just to be safe, do a dry run and execute the clean command with the ` -n` option
4. Oh noes!  there's a `.c` file that would have been deleted!
5. Add `src/mylib.c` to the staging area. don't commit it.
6. Run the clean command with the ` -n` option. Notice that mylib.c will not be deleted. Also notice that the files in the obj directory are not listed
7. Run the clean command with the ` -n -d ` option.
8. Looks good! clean the repo ` -f -d `

## Useful commands
- `git clean -n`
- `git add`
- `git clean -n -d`
- `git clean -f -d`

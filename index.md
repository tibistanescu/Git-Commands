# Adding an existing project to GitHub using the command line

1. Create a new repository on GitHub. To avoid errors(conflicts), do not initialize the new repository with README, license, or gitignore files. You can add these files after your project has been pushed to GitHub.

2. Open Git Bash.

3. Change the current working directory to your local project.

4. Initialize the local directory as a Git repository.
```
$ git init
```

5. Add the files in your new local repository. This stages them for the first commit.
```
$ git add .
```
To unstage a file, use 'git reset YOUR-FILE'.
To unstage all files, use 'git reset'.

6. Commit the files that you've staged in your local repository.
```
git commit -m "First commit"
```
Commits the tracked changes and prepares them to be pushed to a remote repository. To remove this first commit, use 'git update-ref -d HEAD'.

7. From the top of your GitHub repository's Quick Setup page, copy the remote repository URL.

8. In the Command prompt, add the URL for the remote repository where your local repository will be pushed.
```
$ git remote add origin remote repository URL
# Sets the new remote
$ git remote -v
# Verifies the new remote URL
```

9. Push the changes from your local repository to GitHub.
```
$ git push origin master
```

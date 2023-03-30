<!--
    Title: Git Help
    Author: somerongit (Someron Bakuli) 
-->
# Basic [Git](http://git-scm.com/book/en/v2) Commands
# Architechture [PPT](https://github.com/somerongit/git_Help/blob/main/Git.pptx)
At a convenient location on your computer, create a folder named git-test.
Open this git-test folder in your favorite editor.
Add a file named index.html to this folder, and add the following HTML code to this file:

<!DOCTYPE html>
<html>
    <head></head>

    <body>
        <h1>This is a Header</h1>
    </body>
</html>

# Initializing the folder as a Git repository
Go to the git-test folder in your cmd window/terminal and type the following at the prompt to initialize the folder as a Git repository:
## git init

# Checking your Git repository status
Type the following at the prompt to check your Git repository's status:
 ## git status
 
# Adding files to the staging area
To add files to the staging area of your Git repository, type:
## git add .

# Commiting to the Git repository
To commit the current staging area to your Git repository, type:
## git commit -m "first commit"

# Checking the log of Git commits
To check the log of the commits to your Git repository, type
## git log --oneline
Now, modify the index.html file as follows:
<!DOCTYPE html>
<html>
    <head></head>

    <body>
        <h1>This is a Header</h1>
        <p>This is a paragraph</p>
    </body>
</html>
    Add a sub-folder named templates to your git-test folder, and then add a file named temp.html to the templates folder. Then set the contents of this file to be the same as the index.html file above.Then check the status and add all the files to the staging area.Then do the second commit to your repository.Now, modify the index.html file as follows:

<!DOCTYPE html>
<html>
    <head></head>

    <body>
        <h1>This is a Header</h1>
        <p>This is a paragraph</p>
        <p>This is a second paragraph</p>
    </body>
</html>

Now add the modified index.html file to the staging area and then do a third commit.

# Checking out a file from an earlier commit
To check out the index.html from the second commit, find the number of the second commit using the git log, and then type the following at the prompt:
## git checkout <second commit's number> index.html

# Resetting the Git repository
To discard the effect of the previous operation and restore index.html to its state at the end of the third commit, type:
## git reset HEAD index.html
Then type the following at the prompt:

## git checkout -- index.html
You can also use git reset to reset the staging area to the last commit without disturbing the working directory.
# Revert the Changes
## git stash

<!--
# Add all and Commit in one Comment
## git commit -am "add all and commit together"
This comment helps you commit and add all together in one comment
-->
# Update exsiting git comments
## git config --global alias.someron "commit -am"
Git config allow us to create a short hand for long comments, using the comment mention above. "someron" is the shorthand of "commit -am" in this example 
## git someron "add all and commit together" 
You can use this just like any other comment as mention here

# Update Prv. commit 
## git add .
## git commit --amend --no-edit
This comment allow add or new files in prv. commit
## git commit --amend -m "Update Msg"
This allow update the prv. commit msg

# Rename the branch 
## git branch -M newName

# Git Log in God Mode
## git config --global alias.someronLog "log --graph --oneline --decorate"
## git someronLog
 
# Sync With currnt Remote Repo
This set of comments overerite all the local changes which is not commited.
*** After running this comment you can't retrive the prv. uncommited changes. 
## git fetch origin
## git reset --hard origin/master
## git clean -df

<!--
    Title: Git Help
    Author: somerongit (Someron Bakuli) 
-->

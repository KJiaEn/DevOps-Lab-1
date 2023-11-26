# ET0735 - Lab 1 (Introduction to Git and Github)

## First Starting
git config, see configuration variables for git <br />

git config --global user.name [your username] <br/>
&emsp;--global, Configuration change will apply globally to the current user on the system <br/>
&emsp;--system, Sets or gets configuration variables at the system level, applying to all users on the system

git config --global user.email [your email]

git config --list, List configurations

## Create
git init<br />
git add

### From Existing Repository
git clone [Link] <br />
git clone [repository URL] [destination folder] <br />
&emsp;--recurse-submodules, initialises and update submodules within a repository  <br />

## Status 
git status, Lists tracked and untracked files <br/>

git diff, View file differences

## Publish
git commit -m <br />
&emsp;-m, "Your commit message here", adds a message <br />
&emsp;-a, Automatically stages and commits all changes to tracked files. Skips the git add step for modified files but won't include untracked files. <br />

git push remote/origin <br />

## Submodules
git submodule add [git submodule repository URL]

## Releases
git tag "tag_name" <br />

git tag -a  "tag_name" -m "Message" <br />
&emsp;-a, Annotated tag <br />
&emsp;-m, Message for annotated tag <br />

git tag -l [pattern], List tags with names that match the given pattern (or all if no pattern is given).

git tag -d "tag_name", Deletes a tag

### Pushing Tag
git push origin "tag_name"

## Remote
git remote, List remote repositories <br />
&emsp;-v, Shows detailed info about each remote <br />

git remote set-url origin [new.git.url], Changes origin remote url

git remote add [name] [url] <br />
This command adds a new remote repository. [name] is a short name that you give to the remote, and [url] is the URL of the remote repository.

git remote remove [name]

git remote rename [old-name] [new-name]

git push <remote> [branch]. This pushes changes from your local repository to the specified branch on the remote repository.

## Branch
git checkout branch, Switch working dir to branch <br />

git merge branch, Merge into current


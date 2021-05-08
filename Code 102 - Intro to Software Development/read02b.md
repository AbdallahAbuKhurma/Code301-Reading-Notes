## Git introduction:
Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it.
## Tracking and Staging a New File
1. Single File Track one file only by using the following format: git add filename
2. All Files Track all files in a repository by using the following command: git add .
* If you would see information regarding changes to be committed use the (git status) command.
## committing 
1. Committing a File
After staging one or multiple files, you should commit the changes and record what you did within the commit message:
git commit -m
2. Committing All Changes:
use the following command (git commit -a)
## Pushing Changes
If you would like to push the changes use the following command (git push origin main)
## Seeing Your Remotes
* By running the (git remote)command, you can view the short names, such as “origin,” of all specified remote handles.

* By using (git remote -v), you can view all the remote URLs next to their corresponding short names.
## Fetching
Fetching entails pulling data that you don’t have from a remote project. And Here is the command format:

git fetch [remote-name]
#### Note: git fetch solely pulls new data to a local repository; it does not merge changes with or modify your local work. 
## Pushing
To push your changes “upstream” for sharing, you would use the following command:
git push [remote-name][branch-name]
#### Note: This command pushes committed changes from your local “main” branch upstream to the “origin” server.
## Renaming/Removing Remotes
1. Rename: To rename a remote’s short name, use the (git remote rename) command.
2. Remove: To remove a remote for whatever reason simply use this command (git remote rm jane)


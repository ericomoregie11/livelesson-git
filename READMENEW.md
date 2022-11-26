# Git Notes

## working with git locally

 - git init used to initilize a directory to a repo
 - git status update us with whats going on the repo
 - 'git add <file>' : use this command to add file to the stagng area
 - 'git commit' : use this command to save the file to the respository
 - 'git cole <url> : brings the git repo from <url> to current folder
 - 'git log':  shows the log history
 - 'git diff: compare current uncommited state with last known git state
 - 'git diff --stages : runs git diff btw the statging area and last known state
 - 'git diff HEAD!<number> : compares HEAD with commit <num> ago(relative)
 - 'git diff <HASH> : compares HEAD with the comit in <HASH>
 - 'git restore --source <HASH OR HEAD!> : restore file to <hash or head>
 - 'git checkout <HASH OR HEAD~> <FILE> : RESTORE FILE TO <HASH OR HEAD~
    when you forget to name the file you end up with a detached head
     - 'git checkout - (main) : go back to main
     - 'git switch - (main): go back to main

## Working with remotes
 - 'git remote add <NAME> <URL>':adds the URL> as a remote with the name <NAME>
 - 'git romote -v" : look at all the remotes you have 
 - 'git romote rm' <NAME>: removes the remote called <NAME>
 - 'git push': <WHERE> <WHAT>: pushes the <what> branch to <where> (git push origin master)
 -  git pull <WHERE> <WHAT>: pulls the <WHAT> branch in <WHERE> to local computer

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

## Branches
 - git branch <NAME> : creates branch <NAME> where you are (HEAD)
 - git switch <NAME> statement: move the head pointer to the branch <NAME>
   - git checkout <name> : also move the head to the branch name on older git versions
 - git switch -c <name> : create and move the head pointer to the newly created branch <name> in 1 command
   - git checkout -b <name>: also do what switch -c do but for git older versions
 - git merge <BRANCH>: while head is pointed to main use merge command to merge <BRANCH> into the current main branch                       (dont use merge while on nay other branch other than the main branch
 - git rebase <Branch>: while head is pointed to the other <BRANCH> not main use rebase comand to incoporate changes                            into main branch. (made this adjustment in new branch trying rebase
 - git rebase: command used to change history of a commit
   - git status: is your best friend when using rebase 
   - git add <FILE> : to help mark conflit resolution
   - git rebase --continue: move to the next commit in rebase when you have multiple commit you want to rebase into main
   - git rebase --abort: undo git rebase step
 - git rebase -i <commit> HEAD~ or <HASH> : of commit to go into interactive rebase mode 
                                            you can the make multiple commits changes in interactive mode e.g. 'squash'
   - git rebase -i <HASH>^: uses the ^ symbol to include that commit in interactive rebase 
    (*notes When you trying to resolve conflits in multiple commit its best to squash all the commit into 1 and just         deal with conflit in one branch)
 

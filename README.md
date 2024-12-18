# GIT Exercise 
## Bundle 1

### EXERCISE 1
...bash
Last login: Wed Dec 18 11:24:51 on ttys000
gymkwigiraii@kwigiras-iMac ~ % mkdir Bundle1
gymkwigiraii@kwigiras-iMac ~ % cd Bundle1
gymkwigiraii@kwigiras-iMac Bundle1 % git init
Initialized empty Git repository in /Users/gymkwigiraii/Bundle1/.git/
gymkwigiraii@kwigiras-iMac Bundle1 % ls -a
.	..	.git
gymkwigiraii@kwigiras-iMac Bundle1 % open .git
gymkwigiraii@kwigiras-iMac Bundle1 % echo hello >file1.html
gymkwigiraii@kwigiras-iMac Bundle1 % echo hello >file2.html
gymkwigiraii@kwigiras-iMac Bundle1 % git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	.DS_Store
	file1.html
	file2.html

nothing added to commit but untracked files present (use "git add" to track)
gymkwigiraii@kwigiras-iMac Bundle1 % git add *.html
gymkwigiraii@kwigiras-iMac Bundle1 % git status    
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
	new file:   file1.html
	new file:   file2.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	.DS_Store

gymkwigiraii@kwigiras-iMac Bundle1 % echo world >>file2.html 
gymkwigiraii@kwigiras-iMac Bundle1 % git status              
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
	new file:   file1.html
	new file:   file2.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   file2.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	.DS_Store

gymkwigiraii@kwigiras-iMac Bundle1 % git add file1.html      
gymkwigiraii@kwigiras-iMac Bundle1 % git status              
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
	new file:   file1.html
	new file:   file2.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   file2.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	.DS_Store

gymkwigiraii@kwigiras-iMac Bundle1 % git add file1.html
gymkwigiraii@kwigiras-iMac Bundle1 % git status        
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
	new file:   file1.html
	new file:   file2.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   file2.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	.DS_Store

gymkwigiraii@kwigiras-iMac Bundle1 % git add *.html          
gymkwigiraii@kwigiras-iMac Bundle1 % git status    
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
	new file:   file1.html
	new file:   file2.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	.DS_Store

gymkwigiraii@kwigiras-iMac Bundle1 % git commit -m "initial commit."
[main (root-commit) a908824] initial commit.
 2 files changed, 3 insertions(+)
 create mode 100644 file1.html
 create mode 100644 file2.html
gymkwigiraii@kwigiras-iMac Bundle1 % 
gymkwigiraii@kwigiras-iMac Bundle1 % git commit                     
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
	.DS_Store

nothing added to commit but untracked files present (use "git add" to track)
gymkwigiraii@kwigiras-iMac Bundle1 % git commit -m "initial commit."
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
	.DS_Store

nothing added to commit but untracked files present (use "git add" to track)
gymkwigiraii@kwigiras-iMac Bundle1 % git branch
* main
gymkwigiraii@kwigiras-iMac Bundle1 % git branch -m main master
gymkwigiraii@kwigiras-iMac Bundle1 % git branch               
* master
gymkwigiraii@kwigiras-iMac Bundle1 % git branch -m main main  
fatal: No branch named 'main'.
gymkwigiraii@kwigiras-iMac Bundle1 % git branch -m master main
gymkwigiraii@kwigiras-iMac Bundle1 % git branch               
* main
gymkwigiraii@kwigiras-iMac Bundle1 % git add *.html                 
gymkwigiraii@kwigiras-iMac Bundle1 % git commit -m "branch name changed commit."
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
	.DS_Store

nothing added to commit but untracked files present (use "git add" to track)
gymkwigiraii@kwigiras-iMac Bundle1 % 
gymkwigiraii@kwigiras-iMac Bundle1 % git remote add origin
usage: git remote add [<options>] <name> <url>

    -f, --fetch           fetch the remote branches
    --tags                import all tags and associated objects when fetching
                          or do not fetch any tag at all (--no-tags)
    -t, --track <branch>  branch(es) to track
    -m, --master <branch>
                          master branch
    --mirror[=(push|fetch)]
                          set up remote as a mirror to push to or fetch from

gymkwigiraii@kwigiras-iMac Bundle1 % git remote add origin https://github.com/IngabireNelly/Gym-Git-Exercise-Solutions
gymkwigiraii@kwigiras-iMac Bundle1 % git push -u origin main

To https://github.com/IngabireNelly/Gym-Git-Exercise-Solutions
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/IngabireNelly/Gym-Git-Exercise-Solutions'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
gymkwigiraii@kwigiras-iMac Bundle1 % git pull origin main --allow-unrelated-histories

remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 883 bytes | 176.00 KiB/s, done.
From https://github.com/IngabireNelly/Gym-Git-Exercise-Solutions
 * branch            main       -> FETCH_HEAD
 * [new branch]      main       -> origin/main
hint: You have divergent branches and need to specify how to reconcile them.
hint: You can do so by running one of the following commands sometime before
hint: your next pull:
hint: 
hint:   git config pull.rebase false  # merge
hint:   git config pull.rebase true   # rebase
hint:   git config pull.ff only       # fast-forward only
hint: 
hint: You can replace "git config" with "git config --global" to set a default
hint: preference for all repositories. You can also pass --rebase, --no-rebase,
hint: or --ff-only on the command line to override the configured default per
hint: invocation.
fatal: Need to specify how to reconcile divergent branches.
gymkwigiraii@kwigiras-iMac Bundle1 % git commit -am "fix the bug that prevented the users from signing up."
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
	.DS_Store

nothing added to commit but untracked files present (use "git add" to track)
gymkwigiraii@kwigiras-iMac Bundle1 %     
...
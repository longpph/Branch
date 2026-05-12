Lịch sử Git:
Windows PowerShell
Copyright (C) Microsoft Corporation. All rights reserved.

Try the new cross-platform PowerShell https://aka.ms/pscore6

PS C:\Windows\system32> cd D:\
PS D:\> cd '.\GIT&HTML\'
PS D:\GIT&HTML> mkdir Branch


    Directory: D:\GIT&HTML


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----         5/12/2026   8:34 AM                Branch


PS D:\GIT&HTML> cd .\Branch\
PS D:\GIT&HTML\Branch> code index.html
PS D:\GIT&HTML\Branch> git init
Initialized empty Git repository in D:/GIT&HTML/Branch/.git/
PS D:\GIT&HTML\Branch> git remote add origin https://github.com/longpph/Branch.git
PS D:\GIT&HTML\Branch> git add .\index.html
PS D:\GIT&HTML\Branch> git commit -m "khoi tao trang chu chien dich"
[master (root-commit) 3f025ee] khoi tao trang chu chien dich
 1 file changed, 27 insertions(+)
 create mode 100644 index.html
PS D:\GIT&HTML\Branch> git push origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 667 bytes | 667.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/longpph/Branch.git
 * [new branch]      master -> master
PS D:\GIT&HTML\Branch> git checkout -b feature/navmenu
Switched to a new branch 'feature/navmenu'
PS D:\GIT&HTML\Branch> git add index.html
PS D:\GIT&HTML\Branch> git commit -m "Them navigation"
[feature/navmenu 24290ec] Them navigation
 1 file changed, 8 insertions(+)
PS D:\GIT&HTML\Branch> git switch main
fatal: invalid reference: main
PS D:\GIT&HTML\Branch> git branch
* feature/navmenu
  master
PS D:\GIT&HTML\Branch> git switch master
Switched to branch 'master'
PS D:\GIT&HTML\Branch> git merge feature/navigation-menu
merge: feature/navigation-menu - not something we can merge
PS D:\GIT&HTML\Branch> git switch feature/navmenu
Switched to branch 'feature/navmenu'
PS D:\GIT&HTML\Branch> git switch master
error: Your local changes to the following files would be overwritten by checkout:
        index.html
Please commit your changes or stash them before you switch branches.
Aborting
PS D:\GIT&HTML\Branch> git branch
* feature/navmenu
  master
PS D:\GIT&HTML\Branch> git add .\index.html
PS D:\GIT&HTML\Branch> git commit -m "Update navigation"
[feature/navmenu 5f93ae6] Update navigation
 1 file changed, 8 insertions(+)
PS D:\GIT&HTML\Branch> git switch master
Switched to branch 'master'
PS D:\GIT&HTML\Branch> git merge feature/nav-menu
merge: feature/nav-menu - not something we can merge
PS D:\GIT&HTML\Branch> git push origin master
Everything up-to-date
PS D:\GIT&HTML\Branch> git switch feature/navmenu
Switched to branch 'feature/navmenu'
PS D:\GIT&HTML\Branch> git add .\index.html
PS D:\GIT&HTML\Branch> git commit -m "Update navigation"
On branch feature/navmenu
nothing to commit, working tree clean
PS D:\GIT&HTML\Branch> git switch master
Switched to branch 'master'
PS D:\GIT&HTML\Branch> git switch feature/nav-menu
fatal: invalid reference: feature/nav-menu
PS D:\GIT&HTML\Branch> git branch
  feature/navmenu
* master
PS D:\GIT&HTML\Branch> git switch feature/navmenu
Switched to branch 'feature/navmenu'
PS D:\GIT&HTML\Branch> git switch master
Switched to branch 'master'
PS D:\GIT&HTML\Branch> git switch feature/navmenu
error: Your local changes to the following files would be overwritten by checkout:
        index.html
Please commit your changes or stash them before you switch branches.
Aborting
PS D:\GIT&HTML\Branch> git add .\index.html
PS D:\GIT&HTML\Branch> git commit -m "updateeee"
[master 4e13343] updateeee
 1 file changed, 9 insertions(+), 1 deletion(-)
PS D:\GIT&HTML\Branch> git switch feature/navmenu
Switched to branch 'feature/navmenu'
PS D:\GIT&HTML\Branch> git add index.html
PS D:\GIT&HTML\Branch> git commit -m "final update"
[feature/navmenu a45f624] final update
 1 file changed, 2 deletions(-)
PS D:\GIT&HTML\Branch> git switch master
Switched to branch 'master'
PS D:\GIT&HTML\Branch> git merge feature/navmenu
Auto-merging index.html
CONFLICT (content): Merge conflict in index.html
Automatic merge failed; fix conflicts and then commit the result.
PS D:\GIT&HTML\Branch>
>> git add index.html
>> git commit -m "Resolve merge conflict for navigation menu"
>>
[master 580f8f7] Resolve merge conflict for navigation menu
PS D:\GIT&HTML\Branch> git push master
fatal: 'master' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
PS D:\GIT&HTML\Branch> git push origin
fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin master

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS D:\GIT&HTML\Branch> git push origin master
Enumerating objects: 17, done.
Counting objects: 100% (17/17), done.
Delta compression using up to 12 threads
Compressing objects: 100% (10/10), done.
Writing objects: 100% (15/15), 1.75 KiB | 898.00 KiB/s, done.
Total 15 (delta 5), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (5/5), done.
To https://github.com/longpph/Branch.git
   3f025ee..580f8f7  master -> master
PS D:\GIT&HTML\Branch> git add .\index.html
PS D:\GIT&HTML\Branch> git commit -m "final update navigation"
[master 2130f44] final update navigation
 1 file changed, 8 deletions(-)
PS D:\GIT&HTML\Branch> git push origin master
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 287 bytes | 287.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/longpph/Branch.git
   580f8f7..2130f44  master -> master
PS D:\GIT&HTML\Branch> code README.md
PS D:\GIT&HTML\Branch> git add README.md
PS D:\GIT&HTML\Branch> git commit -m "Lich su git"
[master 33ae878] Lich sư git
 1 file changed, 156 insertions(+)
 create mode 100644 README.md
PS D:\GIT&HTML\Branch> git push origin master
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.83 KiB | 1.83 MiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/longpph/Branch.git
   2130f44..33ae878  master -> master
PS D:\GIT&HTML\Branch> git branch -d feature/navmenu
Deleted branch feature/navmenu (was a45f624).
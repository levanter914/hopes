# hopes
helloo
remote
local

C:\Users\Sham>e:

E:\>cd git

E:\git>mkdir clone

E:\git>cd clone

E:\git\clone>git init
Initialized empty Git repository in E:/git/clone/.git/

E:\git\clone>git clone https://github.com/levanter914/hopes.git
Cloning into 'hopes'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.

E:\git\clone>cd hopes

E:\git\clone\hopes>git checkout -b fb
Switched to a new branch 'fb'

E:\git\clone\hopes>git fetch origin
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 908 bytes | 151.00 KiB/s, done.
From https://github.com/levanter914/hopes
   f6340f2..e35fbd6  main       -> origin/main

E:\git\clone\hopes>git rebase origin/main
Successfully rebased and updated refs/heads/fb.

E:\git\clone\hopes>README.md

E:\git\clone\hopes>
[main 2024-03-21T18:00:59.937Z] update#setState idle
[main 2024-03-21T18:01:14.659Z] Extension host with pid 6624 exited with code: 0, signal: unknown.
:wq
E:\git\clone\hopes>git add README.md

E:\git\clone\hopes>git commit -m "local"
[fb d3c94a6] local
 1 file changed, 1 insertion(+)

E:\git\clone\hopes>git fetch origin
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 918 bytes | 83.00 KiB/s, done.
From https://github.com/levanter914/hopes
   e35fbd6..0230a9b  main       -> origin/main

E:\git\clone\hopes>git rebase origin/main
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
error: could not apply d3c94a6... local
hint: Resolve all conflicts manually, mark them as resolved with
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".
hint: You can instead skip this commit: run "git rebase --skip".
hint: To abort and get back to the state before "git rebase", run "git rebase --abort".
Could not apply d3c94a6... local

E:\git\clone\hopes>README.md

E:\git\clone\hopes>
[main 2024-03-21T18:03:13.239Z] update#setState idle
[main 2024-03-21T18:03:31.009Z] Extension host with pid 9468 exited with code: 0, signal: unknown.
:wq
E:\git\clone\hopes>git add .

E:\git\clone\hopes>git rebase --continue
[detached HEAD c729676] local
 1 file changed, 1 insertion(+)
Successfully rebased and updated refs/heads/fb.

E:\git\clone\hopes>git push origin fb
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Writing objects: 100% (3/3), 261 bytes | 261.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'fb' on GitHub by visiting:
remote:      https://github.com/levanter914/hopes/pull/new/fb
remote:
To https://github.com/levanter914/hopes.git
 * [new branch]      fb -> fb

E:\git\clone\hopes>git checkout master
error: pathspec 'master' did not match any file(s) known to git

E:\git\clone\hopes>git checkout main
Switched to branch 'main'
Your branch is behind 'origin/main' by 2 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)

E:\git\clone\hopes>git merge fb
Updating f6340f2..c729676
Fast-forward
 README.md | 5 ++++-
 1 file changed, 4 insertions(+), 1 deletion(-)

E:\git\clone\hopes>git branch -d fb
Deleted branch fb (was c729676).

E:\git\clone\hopes>git branch --list
* main

E:\git\clone\hopes>README.md

E:\git\clone\hopes>
[main 2024-03-21T18:06:03.827Z] update#setState idle
[main 2024-03-21T18:06:08.001Z] Extension host with pid 2868 exited with code: 0, signal: unknown.
:wq
E:\git\clone\hopes>

Since the "touch" command didn't work for me, here is my cmd history.

Microsoft Windows [Version 10.0.14393]
(c) 2016 Microsoft Corporation. Alle Rechte vorbehalten.

C:\Users\zanet>cd documents

C:\Users\zanet\Documents>cd Studium

C:\Users\zanet\Documents\Studium>git clone https://github.com/fzanet/exercise6.git
Cloning into 'exercise6'...
remote: Counting objects: 3, done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.

C:\Users\zanet\Documents\Studium>cd exercise6

C:\Users\zanet\Documents\Studium\exercise6>echo > hello_a.py

C:\Users\zanet\Documents\Studium\exercise6>git add hello_a.py

C:\Users\zanet\Documents\Studium\exercise6>git commit -m "Added hello_a"
[master a2e908b] Added hello_a
 Committer: Fabian Zanetti <Fabian Zanetti>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)
 create mode 100644 hello_a.py

C:\Users\zanet\Documents\Studium\exercise6>git push origin master
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 301 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/fzanet/exercise6.git
   a92d7df..a2e908b  master -> master

C:\Users\zanet\Documents\Studium\exercise6>git branch develop

C:\Users\zanet\Documents\Studium\exercise6>git checkout develop
Switched to branch 'develop'

C:\Users\zanet\Documents\Studium\exercise6>echo print('Hello Mrs. B') > hello_b.py

C:\Users\zanet\Documents\Studium\exercise6>git add hello_b.py

C:\Users\zanet\Documents\Studium\exercise6>git commit -m "Added welcome message"
[develop c79e668] Added welcome message
 Committer: Fabian Zanetti <Fabian Zanetti>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)
 create mode 100644 hello_b.py

C:\Users\zanet\Documents\Studium\exercise6>git checkout master
Switched to branch 'master'
Your branch is up-to-date with 'origin/master'.

C:\Users\zanet\Documents\Studium\exercise6>echo print('Hello Mr. A') > hello_a.py

C:\Users\zanet\Documents\Studium\exercise6>git add hello_a.py

C:\Users\zanet\Documents\Studium\exercise6>git commit -m "Added welcome message"
[master 3db81a0] Added welcome message
 Committer: Fabian Zanetti <Fabian Zanetti>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+), 1 deletion(-)

C:\Users\zanet\Documents\Studium\exercise6>git merge develop -m "Merged develop with master"
Merge made by the 'recursive' strategy.
 hello_b.py | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 hello_b.py

C:\Users\zanet\Documents\Studium\exercise6>git commit -m "Added hello_b to master"
On branch master
Your branch is ahead of 'origin/master' by 3 commits.
  (use "git push" to publish your local commits)
nothing to commit, working tree clean

C:\Users\zanet\Documents\Studium\exercise6>git push origin master
Counting objects: 8, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (6/6), done.
Writing objects: 100% (8/8), 741 bytes | 0 bytes/s, done.
Total 8 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), done.
To https://github.com/fzanet/exercise6.git
   a2e908b..d49606f  master -> master

C:\Users\zanet\Documents\Studium\exercise6>echo print('Hello C') > hello_c.py

C:\Users\zanet\Documents\Studium\exercise6>git add hello_c.py

C:\Users\zanet\Documents\Studium\exercise6>git commit -m "Added welcome message"
[master 3926f69] Added welcome message
 Committer: Fabian Zanetti <Fabian Zanetti>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)
 create mode 100644 hello_c.py

C:\Users\zanet\Documents\Studium\exercise6>git checkout develop
Switched to branch 'develop'

C:\Users\zanet\Documents\Studium\exercise6>echo print('Hello c') > hello_c.py

C:\Users\zanet\Documents\Studium\exercise6>git add hello_c.py

C:\Users\zanet\Documents\Studium\exercise6>git commit -m "Added welcome message"
[develop 2b56348] Added welcome message
 Committer: Fabian Zanetti <Fabian Zanetti>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)
 create mode 100644 hello_c.py

C:\Users\zanet\Documents\Studium\exercise6>git merge develop -m "Merged develop with master"
Already up-to-date.

C:\Users\zanet\Documents\Studium\exercise6>git checkout master
Switched to branch 'master'
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

C:\Users\zanet\Documents\Studium\exercise6>git merge develop -m "Merged develop with master"
Auto-merging hello_c.py
CONFLICT (add/add): Merge conflict in hello_c.py
Automatic merge failed; fix conflicts and then commit the result.

C:\Users\zanet\Documents\Studium\exercise6>git add hello_c.py

C:\Users\zanet\Documents\Studium\exercise6>git commit -m "Solved conflict by hand"
[master 8b78798] Solved conflict by hand
 Committer: Fabian Zanetti <Fabian Zanetti>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author


C:\Users\zanet\Documents\Studium\exercise6>git push origin master
Counting objects: 9, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (6/6), done.
Writing objects: 100% (9/9), 790 bytes | 0 bytes/s, done.
Total 9 (delta 3), reused 0 (delta 0)
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
To https://github.com/fzanet/exercise6.git
   d49606f..8b78798  master -> master

C:\Users\zanet\Documents\Studium\exercise6>git add hello_c.py

C:\Users\zanet\Documents\Studium\exercise6>git commit -m "Solved conflict by hand"
[master 9e1a8bc] Solved conflict by hand
 Committer: Fabian Zanetti <Fabian Zanetti>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 8 insertions(+)

C:\Users\zanet\Documents\Studium\exercise6>git push origin master
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 344 bytes | 0 bytes/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local objects.
To https://github.com/fzanet/exercise6.git
   8b78798..9e1a8bc  master -> master

C:\Users\zanet\Documents\Studium\exercise6>

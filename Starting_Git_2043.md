Notes for starting git in 2043

Step 1: Get an online git account.
Username for reference: jmh24

Step 2: Use a machine that has git installed.

Step 3: Go to the command prompt and let's get started.

Big Idea: Get to your folder

Use *dir* to find out what is in the directory.
```
C:\Users\LAB>dir
 Volume in drive C is OS
 Volume Serial Number is 98A8-1DEB

 Directory of C:\Users\LAB

06/21/2012  01:13 PM    <DIR>          .
06/21/2012  01:13 PM    <DIR>          ..
05/14/2015  08:11 AM    <DIR>          Contacts
11/05/2015  08:12 AM    <DIR>          Desktop
05/14/2015  08:11 AM    <DIR>          Documents
05/14/2015  08:11 AM    <DIR>          Downloads
05/14/2015  08:11 AM    <DIR>          Favorites
05/14/2015  08:11 AM    <DIR>          Links
05/14/2015  08:11 AM    <DIR>          Music
05/14/2015  08:11 AM    <DIR>          Pictures
05/14/2015  08:11 AM    <DIR>          Saved Games
05/14/2015  08:11 AM    <DIR>          Searches
05/14/2015  08:11 AM    <DIR>          Videos
               0 File(s)              0 bytes
              13 Dir(s)  410,606,678,016 bytes free
```
Change directory to the Desktop using *cd* and your file name
```
C:\Users\LAB>cd Desktop
```
Look in the directory of our file using *dir*
```
C:\Users\LAB\Desktop>dir
 Volume in drive C is OS
 Volume Serial Number is 98A8-1DEB

 Directory of C:\Users\LAB\Desktop

11/05/2015  08:12 AM    <DIR>          .
11/05/2015  08:12 AM    <DIR>          ..
11/05/2015  08:13 AM    <DIR>          2043_git_Practice
06/21/2012  02:16 PM             1,553 Report Problems-ITS.lnk
               1 File(s)          1,553 bytes
               3 Dir(s)  410,609,893,376 bytes free
```
Change directories to our folder using *cd*
```
C:\Users\LAB\Desktop>cd 2043_git_Practice
``` 
And now we are ready to begin
```
C:\Users\LAB\Desktop>cd 2043_git_Practice
```
Big Idea 2: Set up your git folder.
1. Go to github.com
2. Sign in
3. Create a new repository
(this is usually a big green button with a _mark)
4. Name the new repository
5. Provide a meaningful description in the repository.
This should try to answer 5 questions:
	Who?
	What?
	When?
	Where?
	Why?
6: Do not select the button to initialize folder with a ReadMe file
7: Follow the instructions on Github.com for:
...or create a new repository on the command line

	echo # 2043_2015_11_05_Practice >> README.md
	git init
	git add README.md
	git commit -m "first commit"
	git remote add origin https://github.com/jmh24/2043_2015_11_05_Practice.git
	git push -u origin master

Now I will show those instructions and their results inside the command prompt.
I will copy and paste one line at a time from Github.com into my command prompt and then execute it.
After I have finished executing these lines, I will copy the command prompt over and comment it.

Below is my command prompt activity.
1. Make a readme.md file.
```
C:\Users\LAB\Desktop\2043_git_Practice>echo # 2043_2015_11_05_Practice >> README
.md
```
2. Initialize the git folder.
```
C:\Users\LAB\Desktop\2043_git_Practice>git init
Initialized empty Git repository in C:/Users/LAB/Desktop/2043_git_Practice/.git/
```
3. Add my readme.md file.
```
C:\Users\LAB\Desktop\2043_git_Practice>git add README.md
```
4. Add all of my files.
```
C:\Users\LAB\Desktop\2043_git_Practice>git add .
```
5. Commit my files with a description of "first commit"
```
C:\Users\LAB\Desktop\2043_git_Practice>git commit -m "first commit"
```
6. Tell the machine who I am.
```
*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'LAB@STF126L-PC.(none)')

C:\Users\LAB\Desktop\2043_git_Practice>git config user.name "Jaclyn Hammond"

C:\Users\LAB\Desktop\2043_git_Practice>git config user.email "jaclynmh0624@yahoo
.com"

C:\Users\LAB\Desktop\2043_git_Practice>git commit -m "first commit"
[master (root-commit) 85049b6] first commit
 2 files changed, 2 insertions(+)
 create mode 100644 README.md
 create mode 100644 Starting_Git_2043.md

C:\Users\LAB\Desktop\2043_git_Practice>git remote add origin https://github.com/
jmh24/2043_2015_11_05_Practice.git

C:\Users\LAB\Desktop\2043_git_Practice>git push -u origin master
Username for 'https://github.com': jmh24
Password for 'https://jmh24@github.com':
Counting objects: 4, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 329 bytes | 0 bytes/s, done.
Total 4 (delta 0), reused 0 (delta 0)
To https://github.com/jmh24/2043_2015_11_05_Practice.git
 * [new branch]      master -> master
Branch master set up to track remote branch master from origin.

C:\Users\LAB\Desktop\2043_git_Practice>git status
On branch master
Your branch is up-to-date with 'origin/master'.
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   Starting_Git_2043.md

no changes added to commit (use "git add" and/or "git commit -a")

C:\Users\LAB\Desktop\2043_git_Practice>git add .

C:\Users\LAB\Desktop\2043_git_Practice>git commit -m "Added instructions and com
ments"
[master cf4440d] Added instructions and comments
 1 file changed, 90 insertions(+), 1 deletion(-)
 rewrite Starting_Git_2043.md (100%)

C:\Users\LAB\Desktop\2043_git_Practice>git push
warning: push.default is unset; its implicit value has changed in
Git 2.0 from 'matching' to 'simple'. To squelch this message
and maintain the traditional behavior, use:

  git config --global push.default matching

To squelch this message and adopt the new behavior now, use:

  git config --global push.default simple

When push.default is set to 'matching', git will push local branches
to the remote branches that already exist with the same name.

Since Git 2.0, Git defaults to the more conservative 'simple'
behavior, which only pushes the current branch to the corresponding
remote branch that 'git pull' uses to update the current branch.

See 'git help config' and search for 'push.default' for further information.
(the 'simple' mode was introduced in Git 1.7.11. Use the similar mode
'current' instead of 'simple' if you sometimes use older versions of Git)

Username for 'https://github.com': jmh24
Password for 'https://jmh24@github.com':
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.36 KiB | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/jmh24/2043_2015_11_05_Practice.git
   85049b6..cf4440d  master -> master

C:\Users\LAB\Desktop\2043_git_Practice>
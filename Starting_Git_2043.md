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
```

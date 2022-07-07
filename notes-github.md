# Lesson 3---
dir (show directory)
cd (change directory)
pwd (working directory
# Lesson 4---
git config --global user.name "full name" (configure name)
git config --global user.email "full name" (configure email , match github)
cat ~/.gitconfig (should show file with data above)
#Lesson 5---
ssh-keygen -o (generate ssh key)

- This key should be pasted into github ssk keys in seetings
# Lesson 6---
git clone (url with ssh in github)
ls -la (shows all files)
git log

# Lesson 7---
assume you have repo: gitessentials
quick setup follow on github commands
mkdir test (makes directory test)
git init (.git folder creation)
git add README.me (add file README.me to commit)
git status (shows status currently)
git commit -m "First commit"
git log
git remote add origin (add here url of your repo)
git push origin master
#Lesson 10---
unstager work
stage work
commit work
push work

flow for pushing work

creat file nano first-file.txt (create file and enter something)

now you have new file
git status (and see it has been added, untracked)

not staged yet

git add first-file.txt
git status (not it is staged, not push yet)
git commit -m "first push" (this created commited)
git push origin master (this take current commit to origin(github), uploaded an new)


# Lesson 11---
git status (run often!)

edit first-push.txt file
git status will show first-push is modified

now

git add first-push.txt or git add . (all files)

git status show this file to b comited

git commit -m

git status will show nothing, now say
git push origin master (send to github, new commit)

rm first-push.txt (removes file)
ls -la, show  files gona
git status will saym file is deleted 
#Lesson 12 ---
git add . (add all files)

git status (now will show the files is deleted)

what if we dont want to commit and unstage
git reset HEAD first-push.txt
git status
Now file is unstaged, its not undeleted

git add first-push.txt

git reset HEAD frst-push.txt

git status (shows unstaged)

how to undelete

# Lesson 13 ---
alread did rm first push

its gone

with git:

git checkout -- first-push.txt
git status, will show brach is up to date and file exist again

rm first-push.txt
git checkout first-push.txt
file came back
#lesson 14---
git remote -v, shows all rmote oigin

git push production feature branch name

# lesson 15---

git checkout -b new-branch
git checkout new-branch

still all local

git branch shows we are all now new bracnh

# lesson 16
git checkout -b new-branch makes new branch

switch between branch is with git checkout -name

create newf ile new-branch file

ls -la shows new file

git add new-branch file
git commit  -m "new branch"

git push origin new-branch

if you do origin master its not corect

now you can see github accep new coe, there is new code with file

doesnta exist in master

# lesston 17--- merging

gt cehckout newbranch

gona merge. first update master before doing something

git checkout master
git pull origin master

git merge new-branch

new file, 

git status

ls-la shows new file

github only did this local

git push origin master send to github

master now on github website has new stuff

and the file showd under master branch

# lesson 18

git log shows latest change

see latest new branch

git pull origin master, gets latest version on git

 j k moving in git log
 
 with q exti
 
# lesson 19---
 
 git pull origin master, for current branch
 
 no updates
 
 edit readme manually online
 
 add stuff 
 
 git pull origin master bring commit to computer
 
 fast forawrd and changes in file
 
 if you try to push with stuff still top pull gives error
 
 edit new branchf ile
 
 one commit behind
 
 touch empty-file.txt
 
 ls -la shows file in it, git add and commmt
 
 we dont have updaetd branch file


git push origin master rejected 

git pull origin master > this will ask to merge
dont rename file and exit, this merge

git push origin master  now works, merged together and in the right order synced git local and online

HEAD-> points to where we are, the head shows where git think we are

# Lesson 20---
git pull download all code from github, store in memory, writes the commit and skips to top

what if github have work that we don have and we dont want that

change empty file to not empty file , commited in github online

it will show in commits that we diont have in local

git log will not show it

git fetch origin master will download all code but not apply, la -la. shows empty file, but online it is changer

git fetch origin master, download that there is commit, but not apply it yet.

ls -la, nothing changed

git log shows nothinh yet, but it is accesible

git log --oneline --graph --decorate --all shows that there is something new online but we are not there yet

git pull gonna fast forward us to there, not git log --oneline ... shows that we are in the latest commit

ls -la, shows that the empty file changed

git pull = git fetch and running git merge origin/master

# Lesson 21---
git allows to look trhough code thorugh time, git log has a hash

suppose we gonna go back to initial repo

git checkout [hash]

noe it shows we are detached head state, look around and test and commit, and discard anything en ntohing wil change the original

ls -la, shows we only have 1 file, at begin of course we only had one file

git log thinks there is only commit,HEAD is at hash(not at master anymore)

now suppose we move forward

git checkout [hash]

still detached

ls -la shows the files as was the case there

git checkout new-branch, you can check the hase there as well

git status is showing head deatch, to move head to current time
git checkout master 
ls -la, git log, shows we are intthe latest version

we going to branch

we git checkout in time

git checkout -b timewarp-branch
touch timewarp.txt

git status, shows we have new file

gid add.
git commit -m "timewarp"
git push origin timewarp-branch

now the repo shows there is new branch from the place we went back to, sueful to go back to earlier version and try something new

git log now shows head is at timewarp-branch , not detached anymore

you can see new branch is created

use it when you want to go back to code version that you dont want

git checkout master
git merge timewarp-branch

git log will show timewarp is branched

we went back in time and made a change to moved forward
git push origin master and now everthing is in sync
# Lesson 22---


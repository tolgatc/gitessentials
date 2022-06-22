# Lesson 22
README.md is writtin in markdown, with different size titles

md means markdown

## git-essentials
has smaller text compared to Lesson 22 in top

what is project about, contributing rules, how to work with it, sort of instruction manual

## Good practice
updating your README.md regularly

# Lesson 23
##Viewing file differences

git diff filename.ext
ls -la

we gonna edit

nano readme.MD

git status shows readme is modified

git diff README.me, we can see the difference in red replaced and green is added

git add README.md then git commit and git push we update this file

git diff is always smart todo before commiting
# Lesson 24
sometimes we want to ignore files

We create a new file .todo

suppose we dont want to add this file

we gonna create .gitignore, and list filename and types that we dont want

now, .todo does not show when we git status 

# Lesson 25
git lg is an alias

nano ~/.gitconfig

git lg is now aliased and can be used to use a command

# Lesson 26
we make a bad-commit mesage file

git commit -m "type here"

git commit --amend (here we can edit message to commit)

opens vim edit thens tatus to check and then we push

# Lesson 27
copying repo
	we can download, clone, or fork it

forking = copying into my profile, then you can clone in your repo 

forking = taking existing project and copying to your own profile 

check licensing if you wanna use it for yourself

check django

you can continue that fork on your account if you dont acces it

# Lesson 28
git issues, not bad, mislabeled

issue place to start conversation

document a bug

create issue: make better readme, your readme could be better

close issue will issue go away

# Lesson 29
pull request is vital part of comparing code

code, issues etc, pull request biggest to use

pull request is basically saying you have version of code to incorporate into your code

git branch

going to git checkout -b pr-test

git branch and check we are pr-test

we edited read, then add commit and pushed to pr-test, shows now pull req in github

new pull requrest, we gouing to take code from pr test merge into master

we can create pull or draft
pr-test means pull requst

most people stick with merge commit


requerst teview and so on

git branch -d pr-test delets it, 

# Lesson 30
how to undo a commit / local work

supose we did git merge and something went wrong

we might have merged wrong branch

git log --oneline shows one line

suppose how to do uncommit


softor hard reset
we add file and add and commit it

git status showd we are one ahead,,

how to undo this,

git reset --hard with commit hash, undo everything till then and delete it

git reset --hard [commit id]  will delete work

and go back

touch sample.txt

suppos we add again

git reset --soft origin/master
now file still there
git reset empty.txt 
rm empty.txt

this is copmmited, undid commit, git log oneline shows it

# Lesson 31 force pushing
what if you commited and pushed to github

touch undo.txt

add,commit and push

suppose it is accident, how to undo

move forward with lot of caution, forced push

this will delete everything eelse if you do this , if you go timewarp force, it will get rid of everytghing

gonna remove the commit

git reset --hard with hash and going backt here
forced push

now git push origin master --force, gonna remove the latest commit on github and put our head, head is one ebhind due to reset in github
anddd delete the last commit

ddont really use it

# Lesson 32

rebasing

git tree gets quite tough

rebase allows cleaing the tree

where we dont see the merge commits

git checkout -b rebase_branch
added file for test purpose
one head behind
git checkout master
difference merge and rebase is cleaniliness and history

git checkout master
git rebase rebase-branch plopped on top of the tree


#Lesson 33
Conflict is two changes in same file in same place

merge conflict

rebase conflicht, almost the same

now we add merge conflict file in github

and make a similar one with a slight change in local

try to add,commit, push conflight

pull conflioct

git status now shows there is conflict

git diff filename will show the difference

nano filename now shows weird stuff

we nede to fix it 

now git commit and save and quit 

git commit shows indeed merged local

git push will bring itto github

first you edit, see differences than fix it, git add,commit and push

now we ggoing to rebase conflict

make rebase conflicht

we make rebase branch with same file slightly different,

try to rebase master, gives conflict

git diff now shows proper difference rather than ===<<<>>>>

edit and improve(can be hybrid)

git add, git rebase --continue , nice clean branch

# Lesson 34 Stashing
save it, dont show, and dont tell me its there, useful when trying to setich branches, useful for worky our
you dont want to commit, but also want to save

stash save file behind scenes, and continue later

create new branch git branch stash-example

we edited readme and see the difference with diff

we cant do git add /commit

switching to master and checking status will you show the new feature change

git checkout stash-example

switch to branch and git stash

git stash list show whole list

git stash apply 

now see work from astash
like temp save

saved, do somethinh else somewhere else, comeback and continue later, power of stashing

# Lesson 35

tagging

tagging is marking milestone

tag important

version fore xample

push to exxist

tag goes to specific point in code, with a tag

how otuntag

git tag -d nametag deleter tag localyl
git push origin --delete typo-tag

# Lesson 36

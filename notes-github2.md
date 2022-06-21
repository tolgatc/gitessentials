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


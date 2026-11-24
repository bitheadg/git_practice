# install Git and Github CLI

# basic config
#--global applies the identity to all Git repositories on this Windows account.
#check default branch
git config  init.defaultBranch
#change default branch
git config init.defaultBranch main
#if exist
git branch -m master main

git config user.name "author"
git config user.email "author@dot.com"
They are not your GitHub/GitLab username and password.

# commit to main

# create branch

# commit to dev

# Pull Request from Github

# Pull Request click and Merge pull request





############################################
#Initial project upload
$ git init
$ git remote add origin https://github.com/bitheadg/project2023.git
$ git status
$ git add MVC_Plain_Github/*
$ git commit -m "initial upload"
$ git remote -v
$ git push origin main
error: src refspec main does not match any
$ git show-ref
$ git branch -m master main
$ git show-ref
$ git push origin master(main)

#fatal: Pathspec 'MVC_Plain_Github/build.gradle' is in submodule
#git이 init되어 있는 폴더의 상위 폴더에서 다시 git init을 한 경우,
#git에서 하위폴더를 submodule로 인식해서 생기는 문제입니다.

# submodule 삭제하기
git submodule deinit -f directory
rm -rf .git/modules/directory
rm -rf directory/.git
# cache 삭제하기
git rm --cached directory
git add directory

$ git submodule deinit -f MVC_Plain_Github
$ rm -rf MVC_Plain_Github/.git
$ git rm --cached MVC_Plain_Github
$ git init
Reinitialized existing Git repository in D:/delme/.git/

#Eclipse
1) Clone repository
2) Import Projects from Git Repositories tab
https://heeeyomi.tistory.com/194
If the github has multiple sources folder, please select specific folder before Import
3) Add Gradle Nature
#remove all 
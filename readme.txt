git learning tutorial 

git init(create a local git repository)
git status(show repository current state)
git diff(show difference compare with last)
git reset --hard HEAD^(version rollback)
git log(show version historys. parameter:--pretty=oneline)
git reflog(show all version historys)
git remote add origin git@github.com:github-lqw/learngit.git(add remote repo)
git push -u origin master(push local to remote)
git checkout -b dev(create a new branch 'dev' and switch it)
the last command to be equivalent to the fallowing two command:
  git branch dev(create a new branch 'dev')
  git checkout dev(switch to branch 'dev')
git branch(show all branches)
git merge dev(merge 'dev' to current branch)
git branch -d dev(delete branch 'dev')
git log --graph --pretty=oneline --abbrev-commit(show branch merge situation)
git merge --no-ff -m "merge with no-ff" dev(merge with no-ff)
git stash(save working directory)
git remote / git remote -v(show remote repository messages)
git clone git@github.com:github-lqw/gitskills(clone a remote repository to local, only branch 'master' can be see)
git checkout -b dev origin/dev(create branch of remote origin's dev to local)
git pull(fetch from remote branch)
git branch --set-upstream dev origin/dev(when excute command 'git pull' warning 'no tracking information')
git tag v1.0(create a new tag 'v1.0')
git tag v0.9 1909be5(create a new tag 'v0.9' on history commit: 1909be5)
git tag(show tag names)
git show v0.9(show detail message of tag v0.9)
git tag -a v0.1 -m "version 0.1 released" 41a4ba1
git tag -d v0.1(delete tag v0.1)
git push origin v1.0(push tag v1.0 to remote repository)
git push origin --tags(push all tags v1.0 to remote repository)

delete remote tag:
	1、git tag -d v0.9
	2、git push origin :refs/tags/v0.9

git config --global alias.st status(create alias)
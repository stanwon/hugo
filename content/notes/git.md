---
title: "Git"
date: 2023-07-17T11:08:08+08:00
draft: true
---

# git
```shell
	git add <file>
	git add .
	git rm <file>
	git rm .
	git commit -m "some message"
	git reset HEAD
		暂存区被HEAD指向的分支覆盖，工作区不受影响
	git rm --cached <file>
		删除暂存区文件，工作区不受影响
	git checkout .
	git checkout -- <file>
		暂存区替换工作区
	git checkout HEAD .
	git chekout HEAD <file>
		HEAD指向的分支覆盖暂存区和工作区

	git init
	git clone
	git config --list
	git config -e
	git config -e --system
	git config -e --global
	git config [--global] key=val
	git diff
	git mv

	git branch (branchname)
		创建分支
	git checkout (branchname)
		切换分支
```

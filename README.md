# React For Redux Mbox Exercise

本项目用于练习 Redux 和 Mbox with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

React 中的状态如何进行管理的呢？

1.组件内部私有状态 2.通过 Mobx redux 这种 进行共享 state

使用 redux Mbox 这种东西 主要是 实现数据共享 以及 (对共享数据的规范处理)

不使用 Context 的时候 那么就每层传递 props 一层一层传递下去

使用 Context 的时候就可以直接再第一层 声明 然后每层都可以使用

### `认识Redux`

git 重命名

1. git add readme.md git delete readme
   2.git mv readme readme.md

### `git log`

git log --oneline 简洁的一行显示
git log -n4 --oneline 简洁的显示四个

git log 的以前是 当前版本的历史

### `git branch`

git branch (查看分支)
git checkout -b newBranchname master (创建基于 master 的新分支)
git branch -D test (删除分支)

### `git commit`

git commit --amend (修改最新的 message)
git rebase -i (commitid) ctrlX 切换到输入栏 :wq 退出 (修改哪一个 commit 以前一个为例)

### `git diff`

git diff (工作区和暂存区的区别比较)
git rebase -i (commitid) ctrlX 切换到输入栏 :wq 退出 (修改哪一个 commit 以前一个为例)

git reset HEAD (把暂存区所有的东西取消掉 commit 恢复到原来状态)
git checkout -- <file> (把工作区的文件恢复成和暂存区一样的状态)
git reset HEAD --<file> (把暂存区的文件移除 commit 状态)
git reset --hard HEAD 充值到之前的状态

git diff temp(分支/commitI d) master(分支/commitId) index.html 两个 commit 之间 文件的差异

## 正确删除文件的方法

让暂存区干掉他 git rm <file>

有紧急任务 代码写到一半 要回到 commit 的 状态 则 git stash (存到 stash 里面)
git stash list (stash 列表)

git stash pop (弹出来就没了)
git stash apply(把之前存放的内容弹出来 堆栈信息还在不会删除)

## 指定不需要 git 管理的工具

创建 .gitignore


##git remote 绑定远程仓库
# github教程

- git status .`：查看当前路径下的的状态。git下**最最常用**的一个命令
- `git add .`: 把工作区的所有变化，(就是你的所有改动)，都添加到 版本库/暂存区
- `git commit -m "提交时说明信息"`: 更进一步提交，并说明提交log
- `git push`: 把版本库的所有更新内容， 都推送到远程服务器。(就是推代码/推上去)
- `git pull`: 把代码从远程服务器拉取到本地。(俗称拉代码)
- `git log`:查看提交历史，与各次的提交说明
- `git diff`:比较工作区与暂存区的差异，就是比较看看你到底都做了什么修改。
- `git clone url地址`: 将远程服务器上项目克隆到新创建的目录中（第一次拉项目时使用， 后面的更新都用 `git pull`了）
- 操作时 双击`tab`键的自动提示/补全功能
- `q`或者`:q`等命令代表退出(quit)
- `ctrl+f`,`ctrl+b`快捷键在termial可以翻页，就是 上一页，下一页

```

创建ssh-key
```

`	ssh-keygen -t rsa -C "youremail@example.com"` 

git config --global user.name 

git config -global user.email

git diff 查看修改的内容

`git log`命令显示从最近到最远的提交日志 ,如果嫌输出信息太多，看得眼花缭乱的，可以试试加上`--pretty=oneline`参数

- `HEAD`指向的版本就是当前版本，因此，Git允许我们在版本的历史之间穿梭，使用命令`git reset --hard commit_id`。
- 穿梭前，用`git log`可以查看提交历史，以便确定要回退到哪个版本。
- 要重返未来，用`git reflog`查看命令历史，以便确定要回到未来的哪个版本



场景1：当你改乱了工作区某个文件的内容，想直接丢弃工作区的修改时，用命令`git checkout -- file`。

场景2：当你不但改乱了工作区某个文件的内容，还添加到了暂存区时，想丢弃修改，分两步，第一步用命令`git reset HEAD <file>`，就回到了场景1，第二步按场景1操作。

场景3：已经提交了不合适的修改到版本库时，想要撤销本次提交，参考[版本回退](https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/0013744142037508cf42e51debf49668810645e02887691000)一节，不过前提是没有推送到远程库



`git rm`用于删除一个文件

要关联一个远程库，使用命令`git remote add origin git@server-name:path/repo-name.git`

查看分支：`git branch`

创建分支：`git branch <name>`

切换分支：`git checkout <name>`

创建+切换分支：`git checkout -b <name>`

合并某分支到当前分支：`git merge <name>`

删除分支：`git branch -d <name>`

用`git log --graph`命令可以看到分支合并图

- 查看远程库信息，使用`git remote -v`；
- 本地新建的分支如果不推送到远程，对其他人就是不可见的；
- 从本地推送分支，使用`git push origin branch-name`，如果推送失败，先用`git pull`抓取远程的新提交；
- 在本地创建和远程分支对应的分支，使用`git checkout -b branch-name origin/branch-name`，本地和远程分支的名称最好一致；
- 建立本地分支和远程分支的关联，使用`git branch --set-upstream branch-name origin/branch-name`；
- 从远程抓取分支，使用`git pull`，如果有冲突，要先处理冲突
- 命令`git tag <tagname>`用于新建一个标签，默认为`HEAD`，也可以指定一个commit id；
- 命令`git tag -a <tagname> -m "blablabla..."`可以指定标签信息；
- 命令`git tag`可以查看所有标签
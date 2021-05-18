# Git 

## Git的基础配置

```shell
git config --global user.name yourName
git config --global user.email yourEmail
git config --global push.default simple
git config --global core.quotepath false
git config --global core.editor "code --wait"
git config --global core.autocrlf input
```
查看`config`列表命令

```shell
git config --list
```

## git init

初始化一个仓库，创建一个`.git`隐藏目录


## git add 

选择哪些变动是需要提交的，路径可以是`绝对路径`、`相对路径`、`·`、`*`

* `git add .`  -- 将所有修改添加到缓存区域
* `git add *`  -- 将匹配的修改内容添加

```shell
git add . 
#将demo文件夹下的所有js文件添加到缓存区域
git add demo/*.js
```

## .gitignore

描述哪些变动是**不需要提交的**

常见的有`node_modules`、`.idea`、`.vscode`、`DS_Store`

## git commit 

* -v -- 会弹出编辑器填写提交记录
* -m  

## git log

查看提交日志

## git reset 

回到对应的版本

* `--hard` --  撤销工作区中所有未提交的修改内容，将暂存区与工作区都回到上一个版本,并删除之前的所有信息提交

## git reflog

查看所有历史，包括回退的提交记录

## git log  VS git reflog

1. `git log ` 只有`commit`的内容
2. `git reflog`  不只有`commit`的内容，还有`reset`等内容

## git branch

创建分支

## git checkout 

用于切换分支

## git merge 

用于合并分支,合并分支的时候可能有冲突，也可能没有冲突。当出现冲突的时候要去解决冲突

#### 解决冲突(!important)

1. 依次打开每个文件
2. 搜索 `====` 四个等于号
3. 在等于号的上下部分选择需要保存的代码
4. 删除不要的代码，删除 `====`,`>>>>>>>`,`<<<<<<<<`
5. git add 对应的文件
6. git status 查看当前代码状态，继续解决下一个冲突 
7. 直到没有冲突，运行 git  commit(这里不需要选项) 提交代码





















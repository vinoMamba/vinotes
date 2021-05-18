# Github

## 配置Github

```shell
# 设置公钥
 ssh-keygen -t rsa -b 4096 -C "your_email@example.com" 
# 得到公钥内容
cat ~/.ssh/id_rsa.pub
# 复制内容到GitHub 的ssh里面
```
## git push 

通过`git push`来上传代码

## git clone 克隆GitHub上的代码到本地

## git pull  

`git pull`先把远程分支合并到本地对应的分支

`git pull`的时候可能会出现代码冲突的情况，需要自行解决冲突，解决方法和之前`merge`是一样的

## 高级操作 git alias

```shell
touch ~/.bashrc
echo 'alias ga="git add"' >> ~/.bashrc
echo 'alias gc="git commit -m"' >> ~/.bashrc
echo 'alias gl="git pull"' >> ~/.bashrc
echo 'alias gp="git push"' >> ~/.bashrc
echo 'alias gco="git checkout"' >> ~/.bashrc
echo 'alias gst="git status -sb"' >> ~/.bashrc
```

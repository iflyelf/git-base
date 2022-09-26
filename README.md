# git基础教程

## 创建git-base目录
```shell
mkdir -pv git-base
```
## 进入git-base目录
```shell
cd git-base
```
## 创建 README.md 文件并写入内容
```shell
echo "# git基础教程" >> README.md
```
## 初始化仓库
```shell
git init
```
## 添加文件到暂存区
```shell
git add .
```
## 将暂存区内容添加到仓库中
```shell
git commit -a -m "添加 README.md 文件"
```
## 添加远程版本库
格式: git remote add [shortname] [url]
备注: shortname 为本地的版本库
```shell
git remote add git-base https://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@github.com/iflyelf/git-base.git
```
## 显示所有远程仓库
```shell
git remote -v
```
## 上传远程代码并合并
```shell
git push --force --quiet git-base master:main
```
## 删除主机的分支
```shell
git push --force --quiet git-base --delete master
```

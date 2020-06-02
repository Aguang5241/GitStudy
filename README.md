# git使用说明
## 一、git本地操作
### 1. 基础信息设置
```
git config --global user.name 'aguang5241'
git config --global user.email '759229100@qq.com'
git config --list(查看信息)
```
### 2. 初始化一个新的git仓库
#### a. 创建文件夹
```
mkdir file_name
```
#### b. 在文件内初始化git（创建git仓库）
```
cd file_name
git init
```
### 3. 向仓库添加文件
#### a. 工作区--->暂存区
```
git status
git add files
```
#### b. 暂存区--->git仓库
```
git status
git commit -m '提交描述'
git status 
```
### 4. 修改仓库文件
#### a. 修改文件
```
vim file
i(进入修改模式)
esc(退出修改模式)
:wq(保存并退出)
git status
```
#### b. 工作区--->暂存区
```
git add file
git status
```
#### c. 暂存区--->git仓库
```
git commit -m 'xxx'
git status
```
### 5. 删除仓库文件
#### a. 删除本地文件
```
rm file
```
#### b. 从git中删除
```
git rm file
```
#### c. 提交操作
```
git commit -m 'xxx'
```
***
## 二、git远程管理仓库
### 1. 克隆远程仓库文件
```
git clone url
```
### 2. 本地修改
```
git add file
git commit -m 'xxx'
```
### 3. 提交到远程仓库
```
git push
```
### 4. 删除远程仓库文件
```
git add *
git commit -m 'xxx'
git push origin master
```
### 5. 删除远程仓库在网页直接删

### 6. 删除远程仓库在网页直接删
```
git config credential.helper store
git push
```


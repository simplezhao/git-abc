

# git-abc



## 仓库管理

### 创建本地仓库

* `git init`

```bash
mkdir git-abc
cd git-abc
git init
```

![image-20210331222402099](https://oss.smart-lifestyle.cn/file/qm2vb.png)

### 添加远程分支

* `git remote add <shortname> <url>`

```bash
git remote add origin https://github.com/simplezhao/git-abc.git
```

### 抓取远程代码

* `git fetch <remote>`

```bash
git fetch origin
```

![image-20210331223237496](https://oss.smart-lifestyle.cn/file/48gpy.png)

### 查看某个远程仓库

* `git remote show <remote>`

```bash
git remote show origin
```

![image-20210331223628444](https://oss.smart-lifestyle.cn/file/50dkt.png)

### 同步远程分支

* `git checkout -b <branch> <remote>`

```bash
git checkout -b main origin/main
```

![image-20210331224921389](https://oss.smart-lifestyle.cn/file/vkntn.png)

## 代码管理

### 查看当前分支状态

* `git status`

1. 修改readme.md文件

```bash
git status
```

提示文件被修改

![image-20210331225856222](https://oss.smart-lifestyle.cn/file/jjthz.png)

2. 新增一个readme_en.md文件

```bash
git status
```

提示有未跟踪的文件

![image-20210331230055526](https://oss.smart-lifestyle.cn/file/ttydm.png)

### 添加文件

* `git add .` 添加所有文件

* `git add <file>`添加指定文件

```bash
# 添加所有文件
git add .
```

添加成功后，显示准备提交的文件

![image-20210331230400289](https://oss.smart-lifestyle.cn/file/2m0ge.png)

### 提交文件

* `git commit -a` 在默认编辑器内增加本次提交内容
* `git commit -m <message>`简短提交

```python
git commit -m "update readme file and add new readme for english version"
```

![image-20210331230900239](https://oss.smart-lifestyle.cn/file/xkx4s.png)

### 推送到远程分支

* `git push <shortname> <branch>`

```bash
git push origin main
```

![image-20210331231029318](https://oss.smart-lifestyle.cn/file/136q4.png)

### 查看提交记录

* `git log`

```bash
git log
```

![image-20210331231130554](https://oss.smart-lifestyle.cn/file/wvarp.png)

## 代码合并

多人开发同一个项目，需要共同维护同一个代码库，假如每个人负责独立的模块，不会涉及到代码冲突

某次提交时，提示如下问题




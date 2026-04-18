## 一、什么是 Git？

Git 是一个分布式版本控制工具，用于管理代码历史记录，并方便与他人协作开发。

------

## 二、安装 Git

1. 打开官网：[***Git***](https://git-scm.com/)
2. 下载 Windows 安装包
3. 双击安装，一路点击 **Next** 即可
4. 安装完成后，打开终端输入：

```
git --version
```

------

## 三、创建并推送新仓库到 GitHub

> 请确保GitHub已经提前创建好一个新仓库

### 👉 方式一：在命令行创建新仓库

```cmd
git init 
git add README.md
git commit -m "第一次提交"
git branch -M main
git remote add origin https://github.com/用户名/仓库名.git
git push -u origin main
```

📌 说明：

- `git init`：初始化仓库
- `git add`：添加文件
- `git commit`：提交到本地仓库
- `git branch -M main`：设置主分支为 main
- `git remote add origin`：绑定远程仓库
- `git push`：推送到 GitHub

------

## 四、推送已有本地仓库到 GitHub

如果你已经有本地项目，只需执行：

```cmd
git remote add origin https://github.com/用户名/仓库名.git
git branch -M main
git push -u origin main
```

------
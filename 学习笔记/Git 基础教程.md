---
tags:
  - 学习笔记
  - Git
  - 版本控制
created: 2026-02-08
---

# Git 基础教程

## 📖 来源

- 学习平台：实践 + 在线文档
- 官方文档：https://git-scm.com/doc
- 学习日期：2026-02-08

## 🎯 学习目标

1. 理解 Git 的基本概念和工作原理
2. 掌握常用 Git 命令的使用
3. 学会 GitHub 与 Git 的协作流程
4. 能够独立创建和管理代码仓库

## 📝 核心内容

### Git 基本概念

**什么是 Git？**
- 分布式版本控制系统
- 记录文件内容的变化，方便查看历史版本
- 支持多人协作开发

**核心概念：**
- **仓库（Repository）**：存放项目文件和版本历史的地方
- **提交（Commit）**：保存项目状态的快照
- **分支（Branch）**：独立的开发线
- **远程仓库（Remote）**：托管在网络上的仓库（如 GitHub）

### 常用 Git 命令

#### 初始化配置

```bash
# 配置用户信息
git config --global user.name "你的名字"
git config --global user.email "你的邮箱"

# 初始化仓库
git init
```

#### 基本操作

```bash
# 查看仓库状态
git status

# 添加文件到暂存区
git add .              # 添加所有文件
git add 文件名         # 添加指定文件

# 提交更改
git commit -m "提交说明"

# 查看提交历史
git log
```

#### 远程仓库操作

```bash
# 关联远程仓库
git remote add origin 仓库地址

# 推送到远程仓库
git push -u origin main    # 首次推送
git push                   # 后续推送

# 拉取远程更新
git pull

# 克隆远程仓库
git clone 仓库地址
```

#### 分支操作

```bash
# 查看分支
git branch

# 创建分支
git branch 分支名

# 切换分支
git checkout 分支名

# 创建并切换分支
git checkout -b 分支名
```

### Git 工作流程

```
工作区 → 暂存区 → 本地仓库 → 远程仓库
  ↓        ↓         ↓          ↓
编辑文件  git add  git commit  git push
```

### GitHub 与 Git 的区别

| Git | GitHub |
|-----|--------|
| 版本控制工具 | 代码托管平台 |
| 本地运行 | 云端服务 |
| 管理代码版本 | 提供协作功能 |

## 💭 个人理解

Git 是开发者的必备技能，它不仅用于代码管理，也可以用于任何需要版本控制的文件（如今天的 Obsidian 笔记）。

**学习要点：**
1. 理解工作区、暂存区、仓库的概念是关键
2. `git status` 是最常用的命令，随时查看状态
3. 提交信息要清晰明了，方便后续追溯
4. 推送前先拉取，避免冲突

**实践体会：**
今天通过创建学习笔记仓库，实际使用了 Git 的完整流程。从初始化、添加文件、提交到推送到 GitHub，整个过程加深了对 Git 工作原理的理解。

## 🔗 相关链接

- [[2026-02-08 日记]]
- [[Clawbot 使用指南]]
- [[Dify 工作流实践]]

### 外部资源

- [Git 官方文档](https://git-scm.com/doc)
- [GitHub 官方教程](https://docs.github.com/zh)
- [Git 简易指南](https://rogerdudler.github.io/git-guide/index.zh.html)

## ✅ 复习计划

- [ ] 1天后复习：回顾基本命令
- [ ] 3天后复习：练习分支操作
- [ ] 1周后复习：完成一个小项目

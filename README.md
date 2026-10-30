# git-practice

我的第一个 Git 练习仓库，用来练熟 Git / GitHub 的日常操作。（主分支版 + 分支版，冲突已解决）

## 练习清单

- [x] git init 初始化仓库
- [x] git add / git commit 提交
- [x] 建分支、合并分支
- [x] 制造并解决一次冲突
- [ ] 推送到 GitHub

## 常用命令

    git status                 # 看当前状态（最常用）
    git add .                  # 工作区 -> 暂存区
    git commit -m "说明"       # 暂存区 -> 提交历史
    git log --oneline --graph  # 看提交历史图
    git switch -c 分支名       # 新建并切换分支
    git switch main            # 切回主分支
    git merge 分支名           # 把分支合并进来

## 冲突长什么样

    <<<<<<< HEAD           <- 你当前分支的版本
    主分支上的那行
    =======                <- 分隔线
    要合并进来的分支的那行
    >>>>>>> 分支名         <- 另一个分支的版本

处理办法：把标记和不要的那行删掉，留下正确内容，然后 git add + git commit。

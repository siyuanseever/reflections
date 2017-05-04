# 暂存区与工作目录和版本库有何不同？你认为它具有什么价值？

暂存区是将工作目录与版本库连接起来的过渡区域，它将工作目录中的文件成批的进行commit,保存
在版本库中，就是这样。
---

# 如何使用暂存区确保为每项逻辑更改进行一次提交？

git diff 比较 working space 与 staging area 的差别，将一项逻辑更改的文件 git add 进
暂存区；
git diff --staged 比较staging area 与 commit1 的差别，git commit；
git reset --hard 恢复 working space 与 staging area 的内容。
---
# 在哪些情况下，分支可以帮助你有序地组织历史记录？分支将如何提供帮助？

当程序需要出现两个不同的版本，并且不同版本各自还要进行后续的跟新commit时，利用git branch
能够在不同的branch之间进行切换，互不影响。这些branch都是基于一个共同的原始版本。
---
# 图表如何帮助你直观显示分支结构？

从branch name开始回溯到最原始的commit，便是在这个branch下的git log的所有commit；
那些没有branch name与之连接的commit将只能够通过commit ID来git checkout。
---
# 将两个分支合并到一起有何结果？为什么我们在图表中表示它的方式是那样的？

我们保留两个合并版本中所有（or）相比于original版本发生更改的地方；
保留两个合并版本中同时（and）相对于original版本不发生改变的内容。\
---
# Git 的自动合并与始终手动进行合并各有何优缺点？

自动合并：快捷但可能会出现conflict；
手动合并：繁琐，消除conflic。

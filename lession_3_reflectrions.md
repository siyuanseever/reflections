# 思考：使用远程版本库

1. git remote add origin https://github.com/siyuanseever/reflections.git
2. git remote (-v)
3. git push origin master
4. git pull origin master

---
# 为何你希望始终手动地拉取更改，而不是让 Git 自动与你的远程版本库保持同步？

自动pull会显得很麻烦，而且由于联网，可能pull并不成功。

---
# 说明Fork、克隆和分支之间的不同。何时使用某种功能而不是另一种？

* Fork:重建另一个属于自己的GitHub工程，拥有修改权
* Clone:github => local;local => local
* Branch:不同版本

---
#如何在不使用 Git 或 GitHub 的情况下开展协同？哪种做法更容易？哪种做法更困难？

> git branch new-branch
> git pull origin new-branch
> pull question
> merge question

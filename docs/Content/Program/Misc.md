# 杂项
---
## Git
- [Learn Git Branching](https://learngitbranching.js.org/?locale=zh_CN) :&nbsp; 通过动画的形式学习Git分支操作
- [Oh Shit, Git?!](https://ohshitgit.com/zh) :&nbsp; 一些Git问题解决方法
- [Git忽略不想修改的本地提交](https://mengqi92.github.io/posts/hide-files-from-git/)
  - `git update-index --skip-worktree /path/to/file`
  - 查看被忽略的文件 `git ls-files -v`
  - 第一列打 `S` 标记的项目就是被忽略（Skip-worktree）的项目(关于符号的更多说明可以参考[官方文档](https://git-scm.com/docs/git-ls-files))
  - 可以通过 `grep` 或是 PowerShell 中的 `Select-String` 来将这些项目过滤出来
    ``` bash
    git ls-files -v | grep -E -i /path/to/file
    git ls-files -v | Select-String -Pattern /path/to/file
    ```
  - 除了 `--skip-worktree` 的方式，Git 也有其它的机制可以忽略文件的修改，大概有这么几类：
    + [git ignore文件](https://git-scm.com/docs/gitignore)
    + `.git/info/exclude` 文件
    + `git update-index --assume-unchanged` ([官方文档](https://git-scm.com/docs/git-update-index))

## Regex
  - [RegexOne](https://regexone.com/) :&nbsp; 在线可交互正则表达式学习
  - [RegExr](https://regexr.com/) :&nbsp; 学习、构建、测试正则表达式

## SQL
  - [SQLZoo](https://sqlzoo.net/wiki/SQL_Tutorial/zh) :&nbsp; 由浅入深学习SQL

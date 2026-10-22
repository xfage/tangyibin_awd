---
name: commit-push
description: Commits all changes and pushes the project to the Gitee master branch. Use when the user asks to commit and push, 提交推送 or 推送到 gitee. Do not use for viewing git history or working with other remotes.
---

# Commit and Push Project

将本仓库的全部改动提交并推送到 Gitee。

## 步骤

1. 检查状态：运行 `git status` 查看当前改动。
2. 暂存所有更改：运行 `git add -A`。
3. 提交：运行 `git commit -m "<message>"`，使用描述性提交信息。
4. 推送：运行 `git push -u origin master`。

## 仓库信息

- 远程仓库：`https://gitee.com/tyb-2020/tyb_html.git`
- 分支：`master`

## 注意事项

- 若远程 `origin` 尚未设置，先执行：`git remote add origin https://gitee.com/tyb-2020/tyb_html.git`
- 若仓库还没有任何提交，本次即为初始提交。
- 首次推送后，后续推送可直接使用 `git push`。

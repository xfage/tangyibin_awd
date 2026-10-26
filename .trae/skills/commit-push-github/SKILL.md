---
name: commit-push-github
description: Commits all changes and pushes the project to GitHub repo xfage/tangyibin_awd as a second remote, keeping Gitee origin untouched. Use when the user asks to 提交到github or push到github. Do not use for Gitee pushes.
---

# Commit and Push to GitHub

将本仓库全部改动提交并推送到 GitHub 仓库。SSH 公钥已设置，推荐使用 SSH 地址认证。Gitee 正在使用的 `origin` 远程保持不动，本 skill 一律使用独立远程名 `github`。

## 仓库信息

- GitHub 仓库：`https://github.com/xfage/tangyibin_awd`
- SSH 地址：`git@github.com:xfage/tangyibin_awd.git`（推荐，公钥已设置）
- 远程名称：`github`
- 分支：`master`

## 步骤

1. 检查状态：运行 `git status` 查看当前改动。
2. 暂存所有更改：运行 `git add -A`。
3. 提交：运行 `git commit -m "<message>"`，使用描述性提交信息。
4. 若远程 `github` 尚未设置，先执行：`git remote add github git@github.com:xfage/tangyibin_awd.git`
5. 推送：运行 `git push -u github master`。

## 注意事项

- 不要修改、覆盖或删除已有的 `origin`（Gitee）远程。
- 若推送被拒绝（远程有新提交），先运行 `git pull --rebase github master` 再推送。
- 若 SSH 连接失败，可改用 HTTPS 地址：`git remote set-url github https://github.com/xfage/tangyibin_awd.git`
- 首次推送后，后续推送可直接使用 `git push github master`。

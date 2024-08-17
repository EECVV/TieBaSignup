# 贴吧签到Github Action版

## 今日签到状态

![Baidu Tieba Auto Sign](https://github.com/jh13champion/TieBaSignup/workflows/Baidu%20Tieba%20Auto%20Sign/badge.svg)

## 简单的使用说明

1. Fork 本仓库，然后点击你的仓库右上角的 Settings，找到 Secrets 这一项，添加一个库秘密变量（Repository secrets）。名称写 `BDUSS` ，内容写你账号的 BDUSS。
支持同时添加多个帐户，BDUSS 之间用 `#` 隔开即可。

2. 设置好环境变量后点击你的仓库上方的 `Actions` 选项，第一次打开需要点击 `I understand...` 按钮，确认在 Fork 的仓库上启用 GitHub Actions 。

3. 点击【Run workflow】按钮，执行你的第一次贴吧签到吧。

4. 至此自动签到就搭建完毕了，可以再次点击`Actions`查看工作记录，如果有`Baidu Tieba Auto Sign`则说明workflow创建成功了。点击右侧记录可以查看详细签到情况。

5. 如果需要可以通过修改`TieBaSign/.github/workflows/main.yml`文件内的`- cron: ' * * *'`修改每天签到的触发时间。
（如果你关注的贴吧很多，请适当拉长2次签到的间隔，以减少漏签的可能性）

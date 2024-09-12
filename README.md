README.md 原文可点击[这里](https://github.com/imsyy/home/blob/dev/README.md)查看。

# Home
此仓库由[imsyy](https://github.com/imsyy/home)改进而来。

# Changelog
新增 GitHub Actions 自动同步至 Alibaba OSS 功能。<br>
在页面底部增加了"公网安备"链接与"萌备"的跳转链接。<br>
在 GitHub Actions 中新增使用 sed 命令更改高德 API 的功能，以保护高德 API 不被泄露。<br>

# 说明
因 GitHub Actions 的镜像从 windows-latest 更改为 ubuntu-latest，因此`.env.example`自动更改`.env`已失效，因此直接套用原仓库将无法使用。

# How to Use
1. Fork 本仓库
2. 在 Settings => Actions secrets and variables => Actions => Repository secrets 中添加以下变量：
   - `ACCESS_KEY_ID`：阿里云 Access Key ID
   - `ACCESS_KEY_SECRET`：阿里云 Access Key Secret
   - `AMAP_KEY`：高德地图 API Key
3. commit 任意一个 dev 分支下的一个文件，启动 Actions 编译。即可成功部署你的网站。

# TODO
支持其他OSS部署，如腾讯云，Amazon S3 协议。
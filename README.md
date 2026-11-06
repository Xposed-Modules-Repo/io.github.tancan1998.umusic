# U 音

QQ 音乐净化模块，包名 `io.github.tancan1998.umusic`，需要兼容 libxposed API 102 的框架。

功能：开屏、摇一摇、蒙层、我的页和搜索广告净化，会员引导及金币入口整理，本地会员显示与音效、自动日签、元宝入口开关。

入口：QQ 音乐 → 我的 → 右上角更多 → 原设置下一行「U 音设置」。

## 源码与协议

主要代码、文档、测试和构建配置由 AI（OpenAI ChatGPT / Codex，通过 Minis）生成并迭代，由维护者提出需求、审核和提供实测反馈。

- 完整源码：https://github.com/TanCan1998/umusic
- 下载：https://github.com/Xposed-Modules-Repo/io.github.tancan1998.umusic/releases
- 开源协议：GNU GPL v3.0（GPL-3.0-only）
- 许可证原文：https://github.com/TanCan1998/umusic/blob/main/LICENSE
- 第三方版权与致谢：https://github.com/TanCan1998/umusic/blob/main/NOTICE.md

## 已实测宿主与验证边界

QQ 音乐 **20.9.8.8 / versionCode 7608**：维护者于 2026-11-06 确认已安装的 U 音 0.7 全部现有功能正常。0.8 的切号日签修复和 0.9 的新包名迁移已通过契约回归、云端构建及静态检查，尚未进行新的真机安装和真实切号验证。

本地会员显示不授予服务端权益，不保证付费歌曲全曲或下载授权。自动日签依赖宿主正常运行并已登录。连续签到天数来自本地成功记录。

## 从旧包名迁移

新版包名为 `io.github.tancan1998.umusic`，旧包名为 `com.xiandehuang.umusic`。请先停用旧模块，再安装并启用新模块、设置宿主作用域后重启宿主。不要同时启用新旧模块。本次发行没有自动替换设备上已安装的模块。

本仓库仅存放模块说明与发行包，完整对应源码及许可证保存在上述源码仓库。

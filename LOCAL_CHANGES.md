# Alan 本地补丁

日期：2026-10-24。此分支用于备份 MaiBot 本机已使用的源码补丁，原作者与许可证保持不变。

- 上游：https://github.com/ZhaoCang-QWQ/social-state
- 安装基线：`d2825d1cbb557303aacf2f5f6c04df2339754b7a`
- 补丁分支：`alan-local`（以实际安装版本为基线，避免同时升级宿主或插件）
- 改动：按可配置 QQ 白名单标记创造者，移除 /今天 命令及帮助入口。日程开关仍须自行关闭。
- 配置与数据：不上传真实运行配置、密钥、QQ 名单、聊天记录、数据库、音频、参考图库或备份文件。配置模板仅保留通用示例。
- 安装：`git clone --branch alan-local https://github.com/touching-fishfish/maibot-social-state.git`，再按原 README 配置自己的服务。
- 验证：Python 源码、JSON 与 TOML 解析及凭据模式扫描；写真插件另运行现有离线测试。未发送 QQ 消息或调用付费生图/语音服务。

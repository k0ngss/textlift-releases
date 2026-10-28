# 文跃 TextLift

Windows 10/11 x64 原生文字助手。解压后双击 TextLift.exe；无需安装运行时。

在设置中填写你的 Chat Completions API 地址、模型和密钥。选中文字后按 Ctrl+Alt+P，检查优化结果后确认替换。不会模拟 Enter 发送。

托盘菜单可检查更新、查看上次结果、打开设置和退出。更新需用户点击后才下载、确认后才安装。

配置默认存放于 `%LOCALAPPDATA%\PromptPolish\config.json`。`TextLift.exe --portable` 使用程序同目录的配置。密钥使用 Windows DPAPI 加密并绑定当前用户。更新只替换主程序，保留配置、安装目录及其他文件。

更新前的原文和结果保存于配置目录的 `update-recovery.json`，重启后可复制。该文件为明文，确认内容不再需要后可手动删除。

此仓库仅发布说明、版本清单和 Release 安装附件。源码及开发历史保存在独立私有仓库。GitHub 自动提供的 Source code 压缩包仅含本公开仓库的发布资料；请下载 TextLift-Windows-x64.exe 或 TextLift-Windows-x64.zip。

SHA256SUMS.txt 和 update.json 中的 SHA-256 用于文件完整性校验，不替代数字签名。当前发行流程尚未配置 Authenticode 签名，Windows SmartScreen 可能提示未知发布者。

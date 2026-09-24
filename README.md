# 云栈桌面版更新源

此公开仓库只保存 macOS 桌面版的正式更新包与 `latest-mac.yml`。源代码保留在私有的 `YunLeFun/cms` 仓库。

稳定更新地址：`https://github.com/YunLeFun/yunzhan-desktop-updates/releases/latest/download/`

发行模式参考 [Obsidian 的公开发行仓库](https://github.com/obsidianmd/obsidian-releases)：私有源码与公开安装包分离。云栈继续更新完整的签名 macOS 应用（包括 Electron），不使用额外的应用脚本热更新协议。

发行版本必须满足：Developer ID Application 签名、Apple 公证及装订、Gatekeeper 验证，ZIP／DMG 与 `latest-mac.yml` 的版本、文件名、大小及 SHA-512 一致。安装包附件使用 `yunzhan-<version>-<arch>` ASCII 文件名，避免 GitHub 重命名后清单失效。

在私有源码仓库完成本地 `release:check` 后，创建 `vX.Y.Z` 草稿 Release，上传 DMG、ZIP、blockmap 和 `latest-mac.yml`。核对草稿的附件清单后再发布为 Latest；草稿阶段不会改变上述稳定地址。不得覆盖已发布附件，修复版本须递增。首次面向用户开放前，先用两个真实签名版本验证自动升级和断网恢复。未完成这些检查时，不发布正式版本。本仓库目前没有签名发行版。

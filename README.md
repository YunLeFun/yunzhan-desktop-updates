# 云栈桌面版更新源

此公开仓库只保存 macOS 桌面版的正式更新包与 `latest-mac.yml`。源代码保留在私有的 `YunLeFun/cms` 仓库。

稳定更新地址：`https://github.com/YunLeFun/yunzhan-desktop-updates/releases/latest/download/`

发布版本必须满足：Developer ID Application 签名、Apple 公证及装订、Gatekeeper 验证；上传 DMG、ZIP、blockmap 和 `latest-mac.yml` 后，再从旧的已签名版本验证自动升级。未完成这些检查时，不创建标记为 latest 的正式版本。

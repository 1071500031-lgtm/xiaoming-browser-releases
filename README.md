# 小明浏览器更新发布

本仓库仅用于公开分发“小明浏览器”的正式安装包和更新元数据，不包含客户端源码、服务端源码、数据库配置、管理员资料或任何私钥。

## 发布文件

每个正式版本通过 GitHub Release 提供：

- `XiaomingBrowser-<version>-win-x64.exe`
- `XiaomingBrowser-<version>-win-x64.exe.blockmap`
- `update-manifest.json`
- `update-manifest.sig`

## 安全规则

- 更新清单必须使用离线 Ed25519 私钥签名。
- 客户端必须先验证清单签名，再验证安装包 SHA-256 和文件大小。
- 更新签名私钥严禁提交到本仓库。
- 源码、Render/Neon 配置和管理员资料严禁提交到本仓库。
- 7.4.60 是旧基线；第一版新更新链从 7.4.61 开始。

# 天琴密语 · LYRA-03

独立端到端加密聊天与文件中转服务。固定入口：
https://gonggong1234dyendui-crypto.github.io/lyra-03/

固定入口导航到独立 HTTPS 来源的客户端；不与 MARS/VIRGO 共用账号或应用存储。服务器保留路由、IP、时间、大小等元数据，但没有消息/附件的解密密钥或管理员阅读入口。

客户端采用 OpenPGP.js 6.3.2 的 RFC9580 v6 密钥、签名及 AES256-GCM，私钥备份由独立口令通过 Argon2id 保护。好友首次使用信任，提供完整指纹核对；不宣称前向保密或独立安全审计。请信任软件发布来源并保护终端。

`client-source.zip` 提供当前客户端、服务端和构建源文件；`client-build.zip` 提供发布构建。包含依赖锁定和许可证。复现：Node24，`npm ci`，`npm run build`。OpenPGP.js 完整对应源码和 LGPL 许可见构建包的 THIRD-PARTY.txt；@noble/hashes 为 MIT 许可。

这是代码与公开入口仓库。不包含真实账号、数据库、私钥、口令、文件内容、发布凭证或运行配置。

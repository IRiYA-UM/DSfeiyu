# DSfeiyu 更新源

这个仓库**只放「大肥鱼 DSfeiyu 管理器」的更新包**，源码不在这里。

管理器「功能」页  大肥鱼本体  「检查更新」走的就是本仓库的 `releases/latest`：
拿最新版号  比对本机 `config/version.json`  下载名字为 `DSfeiyuManager-Setup-<版本>.exe`
的那个 asset（带 sha256 校验） 静默重装。只换程序文件，`data\` 里的记忆、人格、聊天记录不动。

## 为什么 SnowLuma 不在安装包里

SnowLuma 的 EULA 5.4 明确禁止「并入第三方安装包」和「通过自动化脚本部署」，
所以安装包不带它：由管理器向导从 SnowLuma 官方 Release 直连下载，或沿用你本机已经装过的那一份。
QQ 由用户自己装，DSH 走官方安装包。

## 发布约定

- tag 写 `v0.1.0`（前面的 `v` 会被去掉再比）
- asset 名字必须叫 `DSfeiyuManager-Setup-0.1.0.exe`（管理器按这个名字找）
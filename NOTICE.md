# NOTICE

本仓库是上游项目的 **fork**，用于二次开发（学习与自用）。

## 上游项目 / Upstream

| 项 | 值 |
| --- | --- |
| 上游仓库 | [YuJunZhiXue/dsh-purge](https://github.com/YuJunZhiXue/dsh-purge) |
| 上游作者 | **YuJunZhiXue** |
| 上游许可 | MIT，见 [LICENSE](LICENSE) |
| Fork 仓库 | [fanqiecd/dsh-purge](https://github.com/fanqiecd/dsh-purge) |
| Fork 维护者 | **fanqiecd** |

## 署名 / Attribution

上游 [署名要求](https://github.com/YuJunZhiXue/dsh-purge#署名要求) 原文：

> 借用本项目的名称、思路、代码或提示词，必须署名，并写明来源仓库：[YuJunZhiXue/dsh-purge](https://github.com/YuJunZhiXue/dsh-purge)。
> 不署名、隐瞒来源、改头换面据为己有，作者将依法追究责任。

本 fork 的名称、思路、代码与提示词**全部**源自上游，在此明确署名并标明来源仓库。任何再从本 fork 借用上述内容的人，同样必须署名上游仓库 `YuJunZhiXue/dsh-purge`，本 fork 不构成署名替代。

## 非盈利 / Non-profit

上游为免费非盈利公益项目，严禁任何主体用于商业售卖、付费倒卖或黑灰产牟利。本 fork 完全沿用该条款，不用于任何商业用途，也不提供任何收费服务。

## 合规 / Compliance

本 fork 沿用上游 README 中「严格法律与合规免责声明」的全部条款，不新增任何对外网络攻击能力，也不放宽任何限制。测试范围仅限：使用者本机已授权安装的官方 DeepSeek Harness、离线本地靶标、或已获书面授权的受控演练环境。**禁止**对中国大陆、香港、澳门网段及其解析目标做任何访问、扫描或探测。使用者对自己的全部行为独立承担法律责任。

## 本 fork 的改动 / Changes in this fork

相对上游 `master`（v1.1.71）的全部改动，均为二开准备，**未改动任何宿主补丁逻辑**：

1. `package.json`：`repository`、`homepage`、`bugs`、`dsh.install.{tarball,zip,git}` 由上游地址改为 `fanqiecd/dsh-purge`，使一键安装/更新拉取本 fork。包名仍为 `dsh-purge`，`version` 与 `dshTarget` 未动。
2. `README.md` / `README.zh-CN.md`：顶部新增 fork 与署名声明段落。
3. 新增本文件 `NOTICE.md`。
4. 本地新增 `lib/default-prompt-inject.md`（提示词二开起点）。该文件被上游 `.gitignore` 与 `package.json#files`（`"!lib/default-prompt-inject.md"`）双重排除，**不在本仓库中，也不会发布到 npm**。
5. 本地新增 `scripts/tmp-extract-prompt.mjs`（导出上述提示词原文的辅助脚本），同样被 `.gitignore` 的 `scripts/tmp-*.mjs` 排除，不在本仓库中。

## 未改动的上游引用 / Upstream references left as-is

README 中的徽章与插件市场链接仍指向**上游**的第三方登记页：

- DeepSeek Harness Hub — `deepseek.stream/plugins/dsh-purge`
- dsh-plugin.org — `dsh-plugin.org/plugins/yujunzhixue/dsh-purge`
- awesome-dsh-plugin.com

这些是上游的登记条目，本 fork 未另行登记，也不主张继承或代表上游。若要自行登记，请自行替换这些链接与徽章。

## 上游状态 / Upstream status

上游已声明**暂停更新**：不再发版、暂不收 issue / PR，也不保证跟进新版 dsh。本 fork 不承诺跟进上游或新版 dsh。

# 见微 Jianwei Marketplace

Jianwei 专属目录，独立于其他 marketplace。市场名：`jianwei`。

产品与完整安装说明：[Jianwei](https://github.com/Lanbasara/jianwei/blob/v0.2.3/plugin/INSTALL.md)。

```bash
claude plugin marketplace add Lanbasara/jianwei-marketplace
claude plugin install jianwei@jianwei --scope user

codex plugin marketplace add Lanbasara/jianwei-marketplace
codex plugin add jianwei@jianwei
```

## DSH Desktop：添加市场索引

打开「插件 → 发现 → 添加索引源」，填入以下完整 URL：

```text
https://raw.githubusercontent.com/Lanbasara/jianwei-marketplace/main/dsh/index.json
```

这是 DSH 原生 format 1 索引，安装来源固定到 Git commit 与 `plugin/` 子目录，不要求 npm 发布。
仓库根目录仅保留 v0.1.1 兼容布局；0.2.0 及后续版本必须从 `plugin/` 安装。

CLI 直接安装仍可使用（profile 按实际情况替换）：

```bash
dsh plugin --profile web add 'git+https://github.com/Lanbasara/jianwei.git#v0.2.3&path:/plugin'
```

Python 环境和凭据需按产品说明首次配置。

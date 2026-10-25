# 见微 Jianwei Marketplace

Jianwei 专属目录，独立于其他 marketplace。市场名：`jianwei`。

产品与完整安装说明：[Jianwei](https://github.com/Lanbasara/jianwei/blob/v0.1.0/INSTALL.md)。

```bash
claude plugin marketplace add Lanbasara/jianwei-marketplace
claude plugin install jianwei@jianwei --scope user

codex plugin marketplace add Lanbasara/jianwei-marketplace
codex plugin add jianwei@jianwei
```

DSH 使用原生 profile bundle，直接安装产品版本：

```bash
dsh plugin --profile web add github:Lanbasara/jianwei#v0.1.0
```

Python 环境和凭据需按产品说明首次配置。当前含 tanyuan + research，report 尚未交付。

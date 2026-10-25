# 见微 Jianwei Marketplace

Jianwei 专属目录，独立于其他 marketplace。市场名：`jianwei`。

产品与完整安装说明：[Jianwei](https://github.com/Lanbasara/jianwei/blob/v0.1.1/INSTALL.md)。

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

选择见微 Jianwei，确认版本并安装。没有「发现」页时，在实验性插件中启用自定义插件市场。

这是 DSH 原生 format 1 索引，安装来源为 Git commit，不要求 npm 发布。当前没有发布 npm 包，不要直接从 npm 安装裸包名 `jianwei`。

**升级（DSH 0.2.1-rc.3）**：刷新见微市场；有更新时，在「已安装」卸载 Jianwei，按宿主提示重启，再回市场安装推荐版本。无需编辑版本号或更换索引 URL。已装 0.1.0 的用户同样操作。升级提示本身不是一键升级按钮。Python 环境和凭据在插件目录外，卸载插件不会自动删除它们。

CLI 直接安装仍可使用（profile 按实际情况替换）：

```bash
dsh plugin --profile web add github:Lanbasara/jianwei#v0.1.1
```

Python 环境和凭据需按产品说明首次配置。当前含 tanyuan + research，report 尚未交付。

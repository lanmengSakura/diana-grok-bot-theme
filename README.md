# Diana Grok Bot Theme

面向 Grok Bot 桌面端的嘉然（Diana）日间 / 暗夜视觉蓝图。

> **公开测试版：[`v0.1.0-beta.1`](https://github.com/lanmengSakura/diana-grok-bot-theme/releases/tag/v0.1.0-beta.1)。** Release 提供可审阅的 CSS 与目标专用美术蓝图，但不包含依赖桌面端调试接口的本机挂载器；正式稳定版等待扩大回归。

## 当前构图

`visual-blueprint/diana-grok-bot.css` 包含顶部双装饰线、左下简笔画、右侧嘉然立绘、星星糖果组、窄边外发光和 Grok 工作区特有的“黑洞”底层构图。日间与暗夜通过 `data-diana-grok-mode` 分离，不强制覆盖原生工作区的核心可读性。

CSS 中的素材占位符由实现者映射到 `assets/`：

| 占位符 | 仓库素材 |
|---|---|
| `__DIANA_CORNER__` | `diana-left-top-detailed-corner-mask-v7.png` |
| `__DIANA_UPPER__` | `diana-line-art-approved-upper.png` |
| `__DIANA_NIGHT_PORTRAIT__` / `__DIANA_DAY_PORTRAIT__` | `diana-night-v3.png` |
| `__DIANA_DOODLE__` | `diana-doodle-chalk-v2-approved.png` |
| `__DIANA_STAR__` | `diana-hand-star-reference-v2.png` |
| `__DIANA_CANDY__` / `__DIANA_LOLLIPOP__` | `diana-candy-wrapped-v1.png` / `diana-candy-lollipop-v1.png` |
| `__ACAO_HEART__` / `__ACAO_CHEER__` | `acao-heart-v3.png` / `acao-cheer-v1.png` |

蓝图中的所有美术节点均为 `pointer-events: none`。它不会单独启动或修改 Grok Bot。

## 为什么没有公开一键挂载器

Grok Bot 当前没有供第三方完整注入此美术层的稳定主题 API。已验证的本机方案需要精确版本识别、渲染器检查和本地回环调试；这些构建专用适配器、端口、进程状态、日志与截图留在私有启动器中，不进入开源仓库。

## 验证

```powershell
npm test
```

最后一轮验收范围见 [PRE_RELEASE.md](PRE_RELEASE.md)。代码使用 [MIT License](LICENSE)，角色与派生美术的边界见 [ASSET_LICENSES.md](ASSET_LICENSES.md)。本项目与 Grok Bot 或 xAI 官方无隶属或背书关系。

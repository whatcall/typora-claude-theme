# Typora Claude 主题

一款温暖、富有编辑感的 Typora 主题，灵感来自 Anthropic 的 Claude 设计语言。

> 语言：**简体中文** · [English](README.md)

包含两种变体：

- **Claude**（`claude.css`）—— 象牙白画布，陶土珊瑚色强调
- **Claude Dark**（`claude-dark.css`）—— 暖调深色界面，同样使用珊瑚色强调

## 预览

**Claude** —— 完整样式展示（标题、列表、引用、代码、表格、中英文）：

![Claude 主题 —— 标题、列表、引用、代码、表格](claude-full.png)

**Claude Dark**：

![Claude Dark 主题 —— 标题、列表、引用、代码、表格](claude-dark-full.png)

## 特性

- 源自 Claude 设计 token 的暖色调——没有冷灰，也没有纯白
- 编辑排版风格：衬线正文（Georgia）+ 衬线展示标题（Cormorant Garamond），并针对中文做了友好回退（苹方、微软雅黑、思源黑体）
- 克制的语法高亮，覆盖 CodeMirror、Pygments、GitHub Primer 三套 token
- 已主题化的侧边栏与界面 chrome

## 字体与替代方案

Claude 原生界面使用了三款私有 webfont——`anthropic-serif`、`anthropic-sans` 和 `anthropic-mono`——它们均为商业授权字体，无法随主题分发。为还原同样的视觉效果，本主题改用开源字体与系统字体，并遵循 Claude 自身的 fallback 链。

| 用途 | Claude 原生字体 | 本主题替代方案 | 授权 / 来源 |
|---|---|---|---|
| 正文（回复文字） | `anthropic-serif`（Tiempos Text） | **Georgia** | 系统字体——Claude 官方 `serif` fallback 链的首项 |
| 展示标题 | Copernicus（粗衬线） | **Cormorant Garamond** | 开源（SIL OFL） |
| 代码 | `anthropic-mono` | **JetBrains Mono** | 开源（SIL OFL） |
| 界面 chrome | Styrene B | system-ui / 苹方 | 系统字体 |
| 中文字体 | 苹方 / 微软雅黑 / 思源黑体 | 同上 | 系统字体 |

### 为什么标题使用 500 字重

Cormorant Garamond 属于极细的 garalde 字体，明显比 Copernicus（粗重的 slab-serif）更细。因此本主题将标题设为 **500** 字重，并略微放大字号、使用负字距，在保留衬线优雅感的同时缩小视觉重量差距。

### 可选字体（获得最接近 Claude 的效果）

主题开箱即用，仅依赖系统字体即可正常显示。若想最大程度贴近 Claude 的观感，建议安装以下两款开源字体：

- **[Cormorant Garamond](https://github.com/CatharsisFonts/Cormorant)** —— 展示标题（缺失时依次回退到 `EB Garamond`、`Georgia`）
- **[JetBrains Mono](https://www.jetbrains.com/lp/mono/)** —— 代码块（缺失时回退到 `Source Code Pro`、`SF Mono`、`Menlo` 等）

> **关于可变字体的提示：** 若你为自定义而安装 Inter（或其他字体），请使用**静态字重**而非可变 `.ttf` 文件。基于 Chromium 的渲染器——包括 Typora——可能无法从可变字体文件中解析出特定字重（400/500/600），从而静默回退到系统字体。

## 安装

1. 下载本仓库。
2. 将 `claude.css` 和 `claude-dark.css` 复制到 Typora 的主题目录（`偏好设置 → 外观 → 打开主题文件夹`）。
3. 重启 Typora，然后在主题菜单中选择 **Claude** 或 **Claude Dark**。

## 许可证

GPL-3.0

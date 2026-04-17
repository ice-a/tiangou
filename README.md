<div align="center">

![ai.png](./img.png)

# 🐕 tiangou-quotes

> *"舔狗舔到最后一无所有，但至少你曾经舔过。"*

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![OpenClaw Skill](https://img.shields.io/badge/OpenClaw-Skill-blueviolet)](https://openclaw.com)
[![AgentSkills](https://img.shields.io/badge/AgentSkills-Standard-green)](https://agentskills.io)

<br>

舔狗语录 & 情话金句库 — 一个 AI Skill，让 AI 帮你找到最合适的舔狗语录、情话金句和毒鸡汤。

从 260+ 条原始语录中精选去重，按 **10 个真实场景** 分类整理。不管你是被删好友、表白被拒、还是深夜 emo，都能精准推荐。

[**English**](docs/lang/README_EN.md) · [**日本語**](docs/lang/README_JA.md)

</div>

---

## ✨ 功能特性

- **场景智能匹配**：根据你描述的心情/场景，自动推荐最合适的语录
- **10 大分类**：覆盖从卑微表白到人间清醒的完整情感光谱
- **约 100 条精简语录**：去重精选，每条都是经典
- **纯 Prompt 驱动**：无脚本依赖，兼容所有 AI 平台
- **多语言支持**：中文（默认）/ English / 日本語

---

## 📋 语录分类

| 分类 | 适用场景 | 示例关键词 |
|------|---------|-----------|
| 🚫 被删好友/被拉黑 | TA 把你删了/拉黑了 | 删好友、拉黑、红色感叹号 |
| 😤 被骂/被怼 | 被对方骂或者怼回去 | 骂我、嫌弃、你算什么东西 |
| 💔 表白被拒 | 表白失败但还要继续 | 拒绝、不喜欢、表白失败 |
| 📱 被忽视/不回消息 | TA 又不回你消息 | 不回、已读不回、冷暴力 |
| 🎁 卑微送礼物 | 送东西求关注 | 送礼物、转账、红包 |
| 🤡 自我安慰/正面解读 | 强行给自己找台阶 | 没关系、至少、还在 |
| 😂 搞笑套路 | 沙雕舔狗操作 | 套路、沙雕、反转 |
| 💕 暖心表白 | 真诚走心的情话 | 喜欢、在乎、陪伴 |
| ☠️ 毒鸡汤/人间清醒 | 扎心但不失幽默 | 毒鸡汤、扎心、清醒、人间不值得 |
| ⚡ 简短金句 | 一句话击穿灵魂 | 签名、文案、短句 |

---

## 📂 项目结构

```
tiangou-quotes/
├── SKILL.md              # 核心 Skill 定义（含完整语录库）
docs/
└── lang/
    ├── README_EN.md      # English version
    └── README_JA.md      # 日本語版
```

---

## 🚀 安装 & 使用

### 方式一：OpenClaw / 龙虾（推荐）

将 `tiangou-quotes` 文件夹复制到 OpenClaw 的 skills 目录：

```bash
# macOS / Linux
cp -r tiangou-quotes ~/.openclaw/skills/

# Windows
xcopy /E /I tiangou-quotes %USERPROFILE%\.openclaw\skills\tiangou-quotes
```

重启 OpenClaw 会话即可生效。

### 方式二：Claude Code

```bash
# 安装到当前项目（在 git 仓库根目录执行）
mkdir -p .claude/skills
git clone https://github.com/YOUR_USERNAME/tiangou-quotes .claude/skills/tiangou-quotes

# 或全局安装
git clone https://github.com/YOUR_USERNAME/tiangou-quotes ~/.claude/skills/tiangou-quotes
```

### 方式三：Claude / Gemini / ChatGPT 等平台

这些平台不支持 Skill 格式，可以将 `SKILL.md` 的内容作为 **System Prompt** 或 **Context** 注入：

#### Claude (claude.ai)

1. 打开 [claude.ai](https://claude.ai)，进入 **Projects** → 创建新项目
2. 在 **Project Instructions** 中粘贴 `SKILL.md` 的内容
3. 在该 Project 中对话即可使用

#### Gemini (gemini.google.com)

1. 打开 [Gemini](https://gemini.google.com)，进入 **Settings** → **System instructions**
2. 粘贴 `SKILL.md` 的内容
3. 保存后开始对话

#### ChatGPT / Custom GPT

1. 创建 **Custom GPT**，将 SKILL.md 内容填入 Instructions
2. 或在 **Settings** → **Custom instructions** 中粘贴

#### Cursor / Windsurf / 其他 AI IDE

在项目的 `.cursorrules` 或 `.windsurfrules` 文件中添加：

```markdown
@file tiangou-quotes/SKILL.md
```

---

## 💬 使用示例

```
👤: 我表白被拒了，给我来句舔狗语录
🤖: 今天表白被拒绝了，她对我说能不能脱下裤子撒泡尿照照自己。
    当我脱下裤子的时候，她咽了下口水，说我们可以试一下。

👤: 哈哈哈哈再来一个
🤖: 今天你跟我说我很丑，让我不要骚扰你了。我听了很高兴，
    小说里的主角都像你这样，最开始表现的很厌恶，
    但最后总会被我的真心打动。你现在有多讨厌我，以后就会有多爱我。嘻嘻。

👤: emo了，来句毒鸡汤
🤖: 你以为你在等一个机会，其实你在等一个奇迹。
    而奇迹这种东西，从来不会发生在舔狗身上。
```

---

## 🛠️ 技术细节

- **格式**：纯 Markdown + YAML frontmatter，兼容 OpenClaw AgentSkills 规范
- **依赖**：零依赖，无需安装任何运行时
- **数据来源**：精选自网络热门舔狗语录和情话合集，去重后约 100 条
- **多语言**：AI 回复跟随用户语言（中/英/日），语录库保持中文

---

## 🤝 贡献

欢迎 PR！如果你有好的舔狗语录/情话/毒鸡汤，请查看 [CONTRIBUTING.md](CONTRIBUTING.md)。

---

## 📄 License

[MIT](LICENSE) — 随便用，记得 star ⭐

---

<div align="center">

## ⭐ Star History

<a href="https://www.star-history.com/#YOUR_USERNAME/tiangou-quotes&date">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=YOUR_USERNAME/tiangou-quotes&type=date&theme=dark" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=YOUR_USERNAME/tiangou-quotes&type=date" />
   <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=YOUR_USERNAME/tiangou-quotes&type=date" />
 </picture>
</a>

<br>

MIT License © 2026 tiangou-quotes contributors

</div>

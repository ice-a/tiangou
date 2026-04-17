<div align="center">

![ai.png](../../img.png)

# 🐕 tiangou-quotes

> *"A simp simp till the very end — but hey, at least you simp'd with style."*

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](../../LICENSE)
[![OpenClaw Skill](https://img.shields.io/badge/OpenClaw-Skill-blueviolet)](https://openclaw.com)
[![AgentSkills](https://img.shields.io/badge/AgentSkills-Standard-green)](https://agentskills.io)

<br>

Simp quotes, love phrases & toxic chicken soup library — an AI Skill that helps you find the perfect simp quote, romantic line, or savage roast for any situation.

Curated from 260+ raw quotes down to ~100 unique classics, organized into **10 real-life scenarios**. Whether you've been blocked, rejected, or you're just having a late-night emo moment — we've got you covered.

[**中文**](../../README.md) · [**日本語**](README_JA.md)

</div>

---

## ✨ Features

- **Smart scenario matching**: Automatically recommends the most fitting quote based on your mood/situation
- **10 categories**: Covers the full emotional spectrum from desperate confessions to brutal reality checks
- **~100 curated quotes**: Deduplicated and handpicked — every single one is a classic
- **Pure prompt-driven**: Zero script dependencies, works on any AI platform
- **Multilingual support**: 中文 (default) / English / 日本語

---

## 📋 Quote Categories

| Category | Scenario | Example Keywords |
|----------|----------|-----------------|
| 🚫 Deleted & Blocked | They deleted/blocked you | blocked, unfriended, red exclamation mark |
| 😤 Insulted & Roasted | They cursed at you | insulted, cursed, hated, "go die" |
| 💔 Rejected | Confession failed but you're not giving up | rejected, friendzoned, "I don't like you" |
| 📱 Ignored & Ghosted | They're not replying again | ghosted, left on read, cold treatment |
| 🎁 Humble Gifting | Sending gifts to get attention | gifts, money, salary, transfer |
| 🤡 Cope & Delulu | Finding silver linings where none exist | cope, delulu, "it's fine", at least |
| 😂 Funny Routines | Hilarious simp operations | jokes, funny, plot twist |
| 💕 Warm Confession | Sincere and touching love words | love, miss you, goodnight, confession |
| ☠️ Toxic Wisdom | Savage reality checks | reality check, harsh truth, wake up call |
| ⚡ Quick One-Liners | Soul-crushing single lines | bio, caption, short quote |

---

## 📂 Project Structure

```
tiangou-quotes/
├── SKILL.md              # Core Skill definition (with full quote library)
docs/
└── lang/
    ├── README_EN.md      # This file
    └── README_JA.md      # 日本語版
```

---

## 🚀 Installation & Usage

### Option 1: OpenClaw (Recommended)

Copy the `tiangou-quotes` folder to OpenClaw's skills directory:

```bash
# macOS / Linux
cp -r tiangou-quotes ~/.openclaw/skills/

# Windows
xcopy /E /I tiangou-quotes %USERPROFILE%\.openclaw\skills\tiangou-quotes
```

Restart your OpenClaw session and you're good to go.

### Option 2: Claude Code

```bash
# Install to current project (run at git repo root)
mkdir -p .claude/skills
git clone https://github.com/ice-a/tiangou-quotes .claude/skills/tiangou-quotes

# Or install globally (available in all projects)
git clone https://github.com/ice-a/tiangou-quotes ~/.claude/skills/tiangou-quotes
```

### Option 3: Claude / Gemini / ChatGPT

These platforms don't support the Skill format natively, but you can inject `SKILL.md` content as **System Prompt** or **Context**:

#### Claude (claude.ai)

1. Open [claude.ai](https://claude.ai), go to **Projects** → Create new project
2. Paste `SKILL.md` content into **Project Instructions**
3. Start chatting within that project

#### Gemini (gemini.google.com)

1. Open [Gemini](https://gemini.google.com), go to **Settings** → **System instructions**
2. Paste `SKILL.md` content
3. Save and start chatting

#### ChatGPT / Custom GPT

1. Create a **Custom GPT** and fill SKILL.md content into Instructions
2. Or paste into **Settings** → **Custom instructions**

#### Cursor / Windsurf / Other AI IDEs

Add to your project's `.cursorrules` or `.windsurfrules` file:

```markdown
@file tiangou-quotes/SKILL.md
```

---

## 💬 Usage Examples

```
👤: I just got rejected after confessing my feelings. Hit me with a simp quote.
🤖: She told me I was ugly and to stop bothering her. I was thrilled —
    in every novel, the love interest starts off hating the protagonist,
    but eventually gets won over by their sincerity.
    The more she hates me now, the more she'll love me later. Hehe.

👤: Hahaha, give me another one
🤖: My crush goes on dates with different guys every day. I figure
    eventually it'll be my turn. I asked when she could see me,
    she said "next life." How sweet — she already wants to be with
    me in the next life too.

👤: I'm feeling emo. Give me some toxic wisdom.
🤖: You think you're waiting for an opportunity,
    but actually you're waiting for a miracle.
    And miracles? They don't happen to simps. Ever.
```

---

## 🛠️ Technical Details

- **Format**: Pure Markdown + YAML frontmatter, compatible with OpenClaw AgentSkills spec
- **Dependencies**: Zero — no runtime installation needed
- **Data source**: Curated from popular Chinese simp quote and love phrase collections, ~100 unique quotes after deduplication
- **Multilingual**: AI replies follow user language (中文/English/日本語), quote library stays in Chinese

---

## 🤝 Contributing

PRs welcome! If you have great simp quotes, love phrases, or toxic wisdom, check out [CONTRIBUTING.md](../../CONTRIBUTING.md).

---

## 📄 License

[MIT](../../LICENSE) — Use freely, don't forget to star ⭐

---

<div align="center">

## ⭐ Star History

<a href="https://www.star-history.com/#ice-a/tiangou-quotes&date">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=ice-a/tiangou-quotes&type=date&theme=dark" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=ice-a/tiangou-quotes&type=date" />
   <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=ice-a/tiangou-quotes&type=date" />
 </picture>
</a>

<br>

MIT License © 2026 tiangou-quotes contributors

</div>

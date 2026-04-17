<div align="center">

![ai.png](../../img.png)

# 🐕 tiangou-quotes

> *"シンプは最後には何も残らない——でも、少なくともシンプだったことは事実だ。"*

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](../../LICENSE)
[![OpenClaw Skill](https://img.shields.io/badge/OpenClaw-Skill-blueviolet)](https://openclaw.com)
[![AgentSkills](https://img.shields.io/badge/AgentSkills-Standard-green)](https://agentskills.io)

<br>

シンプ語録 & ラブフレーズ & 毒スープライブラリ — AI Skill が、あなたの状況や気分にぴったりのシンプ語録、ラブメッセージ、またはサバケな名言を見つけます。

260件以上の語録から厳選し、重複を除外した約100件を **10 のリアルシーン** に分類。ブロックされた、告白をフラれた、深夜にエモってる……どんな状況でもピンポイントでおすすめします。

[**中文**](../../README.md) · [**English**](README_EN.md)

</div>

---

## ✨ 機能

- **シーンのスマートマッチング**：気分や状況を分析して、最適な語録を自動でおすすめ
- **10カテゴリ**：必死な告白から厳しい現実まで、感情のスペクトルを完全カバー
- **約100件の厳選語録**：重複排除・厳選、すべてがクオリティ保証
- **Pure Prompt駆動**：スクリプト依存ゼロ、すべてのAIプラットフォームで動作
- **多言語対応**：中文（デフォルト）/ English / 日本語

---

## 📋 語録カテゴリ

| カテゴリ | シーン | キーワード例 |
|----------|--------|-------------|
| 🚫 ブロック・削除 | ブロックされた/友達解除された | blocked, 削除, 赤い感叹号 |
| 😤 悪口・罵倒 | 悪口を言われた/言い返したい | 罵られた, 汚い言葉, 死ね |
| 💔 告白フラれ | 告白失敗でも諦めない | rejected, 好きじゃない, フラれた |
| 📱 無視・未読 | また既読スルーされた | ghosted, 既読無視, 冷暴力 |
| 🎁 卑屈なプレゼント | 気を引くために贈り物 | プレゼント, 送金, 赤い封筒 |
| 🤡 ポジティブ解釈 | ないものねだりで自分を慰める | cope, delulu, 関係ない, まあいいか |
| 😂 面白いヤリ方 | シンプの面白いテクニック | ネタ, 面白い, どんでん返し |
| 💕 温かい告白 | 真摯な愛の言葉 | 好き, 会いたい, おやすみ |
| ☠️ 毒スープ・現実 | 厳しい現実を突きつける名言 | 毒スープ, 厳しい真実, 現実 |
| ⚡ 一言名言 | 魂を揺さぶる一言 | プロフィール, キャプション, 短文 |

---

## 📂 プロジェクト構成

```
tiangou-quotes/
├── SKILL.md              # コアSkill定義（語録ライブラリ含む）
docs/
└── lang/
    ├── README_EN.md      # English version
    └── README_JA.md      # このファイル
```

---

## 🚀 インストール & 使い方

### 方法1：OpenClaw（推奨）

`tiangou-quotes` フォルダを OpenClaw の skills ディレクトリにコピー：

```bash
# macOS / Linux
cp -r tiangou-quotes ~/.openclaw/skills/

# Windows
xcopy /E /I tiangou-quotes %USERPROFILE%\.openclaw\skills\tiangou-quotes
```

OpenClaw セッションを再起動するだけ。

### 方法2：Claude Code

```bash
# 現在のプロジェクトにインストール（gitリポジトリルートで実行）
mkdir -p .claude/skills
git clone https://github.com/ice-a/tiangou-quotes .claude/skills/tiangou-quotes

# またはグローバルインストール
git clone https://github.com/ice-a/tiangou-quotes ~/.claude/skills/tiangou-quotes
```

### 方法3：Claude / Gemini / ChatGPT

これらのプラットフォームは Skill 形式にネイティブ対応していませんが、`SKILL.md` の内容を **System Prompt** または **Context** として注入できます：

#### Claude (claude.ai)

1. [claude.ai](https://claude.ai) を開き、**Projects** → 新規プロジェクト作成
2. **Project Instructions** に `SKILL.md` の内容を貼り付け
3. そのプロジェクト内で会話を開始

#### Gemini (gemini.google.com)

1. [Gemini](https://gemini.google.com) を開き、**Settings** → **System instructions**
2. `SKILL.md` の内容を貼り付け
3. 保存して会話開始

#### ChatGPT / Custom GPT

1. **Custom GPT** を作成し、SKILL.md の内容を Instructions に入力
2. または **Settings** → **Custom instructions** に貼り付け

#### Cursor / Windsurf / その他 AI IDE

プロジェクトの `.cursorrules` または `.windsurfrules` ファイルに追加：

```markdown
@file tiangou-quotes/SKILL.md
```

---

## 💬 使い方サンプル

```
👤: 告白フラれた…シンプ語録ちょうだい
🤖: 「告白フラれた。彼女は『ズボン下ろして自分を写してみろ』と言った。
    下ろしたら彼女はゴクリと飲み込んで、『試してみようか』と言った。」

👤: ｗｗｗ もう一つ
🤖: 「俺の好きな子は毎日違う男とデートしてる。いつか俺の番が来るだろうと
    思ってた。いつ会えるか聞いたら『来世ね』って。来世も一緒にいてくれるなんて、
    優しい。」

👤: エモい…毒スープちょうだい
🤖: 「君はチャンスを待ってるつもりかもしれない。
    でも実は奇跡を待ってるんだ。
    で、奇跡ってのは——シンプには絶対に起きないものだ。」
```

---

## 🛠️ 技術詳細

- **フォーマット**：Pure Markdown + YAML frontmatter、OpenClaw AgentSkills 仕様準拠
- **依存**：ゼロ — ランタイムインストール不要
- **データソース**：人気の中国語シンプ語録・ラブフレーズ集から厳選、重複除外後約100件
- **多言語**：AI返信はユーザーの言語に追従（中文/English/日本語）、語録ライブラリは中国語のまま

---

## 🤝 コントリビュート

PR大歓迎！良いシンプ語録、ラブフレーズ、毒スープがあれば [CONTRIBUTING.md](../../CONTRIBUTING.md) をご覧ください。

---

## 📄 License

[MIT](../../LICENSE) — ご自由にお使いください、star ⭐ 忘れずに！

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

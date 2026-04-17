# AI Skills Distillation 🤖💝

基于本地txt文件内容，通过蒸馏技术生成的AI恋爱建议技能集合。

English | [中文](#中文文档)

## Features ✨

- **Romantic Advisor**: Traditional romantic advice and love phrase generation
- **Humorous Relationship**: Modern humorous relationship advice and funny responses
- **Local Operation**: No external APIs required, runs completely locally
- **Chinese Optimized**: Content tailored for Chinese cultural context
- **Easy Integration**: Simple Python imports and function calls

## Installation 📦

```bash
# Clone the repository
git clone https://github.com/your-username/ai-skills-distillation.git
cd ai-skills-distillation

# The skills work with standard Python - no additional dependencies required
python demo.py
```

## Quick Start 🚀

### Romantic Advisor
```python
from romantic_advisor_skill import romantic_advice, generate_love_phrase

# Get romantic advice for a situation
advice = romantic_advice("我被拒绝了")
print(advice)

# Generate a romantic phrase
phrase = generate_love_phrase()
print(phrase)
```

### Humorous Relationship
```python
from humorous_relationship_skill import (
    humorous_relationship_advice,
    generate_humorous_response,
    modern_love_advice
)

# Get humorous advice
advice = humorous_relationship_advice("我被当舔狗了")
print(advice)

# Generate funny response
response = generate_humorous_response("她已读不回")
print(response)

# Get modern relationship advice
modern_tip = modern_love_advice()
print(modern_tip)
```

## Skills Overview 📚

### 1. Romantic Advisor Skill
- **Source**: 情话.txt + 情话宝典.txt
- **Function**: Traditional romantic expressions and advice
- **Best for**: Serious relationship consultation, romantic phrase generation

### 2. Humorous Relationship Skill  
- **Source**: 舔狗语录.txt
- **Function**: Modern humorous responses and internet culture-based advice
- **Best for**: Light-hearted relationship humor, funny responses

## Project Structure 📁

```
ai-skills-distillation/
├── romantic_advisor_skill.py     # Romantic advice skill
├── humorous_relationship_skill.py # Humorous relationship skill
├── skill_config.json             # Skill configuration
├── demo.py                       # Usage demonstration
├── requirements.txt              # Dependencies (empty - no external deps)
└── docs/
    ├── README.md                 # This file
    └── usage_examples.md         # Detailed usage examples
```

## Configuration ⚙️

The `skill_config.json` file contains skill metadata and function definitions:

```json
{
  "skills": {
    "romantic_advisor": {
      "name": "Romantic Advisor",
      "description": "基于情话宝典提供浪漫建议和情话生成"
    }
  }
}
```

## API Reference 📖

### Romantic Advisor Functions

#### `romantic_advice(situation: str = "") -> str`
Provides romantic advice based on the given situation.

#### `generate_love_phrase() -> str`
Generates a classic romantic phrase.

### Humorous Relationship Functions

#### `humorous_relationship_advice(situation: str = "") -> str`
Provides humorous relationship advice.

#### `generate_humorous_response(context: str = "") -> str`
Generates a funny response based on context.

#### `modern_love_advice() -> str`
Returns modern relationship advice.

## Examples 💡

Run the demonstration:
```bash
python demo.py
```

See detailed examples in `docs/usage_examples.md`.

## Content Sources 📝

The skills are distilled from three Chinese text files:
1. **情话.txt**: Realistic love perspectives and advice
2. **情话宝典.txt**: Traditional romantic expressions
3. **舔狗语录.txt**: Modern humorous relationship content

## Contributing 🤝

Contributions are welcome! Please feel free to:
- Add more text content for distillation
- Improve skill algorithms and logic
- Add new skill functionalities
- Optimize user experience

## License 📄

MIT License - see [LICENSE](LICENSE) file for details.

## Author ✍️

Created with Claude Code and AI assistance.

---

# 中文文档

## 功能特点 ✨

- **浪漫建议师**: 提供传统浪漫建议和情话生成
- **幽默恋爱顾问**: 提供现代幽默恋爱建议和搞笑回复
- **本地运行**: 无需外部API，完全本地运行
- **中文优化**: 内容完全基于中文语境
- **易于集成**: 简单的Python导入和函数调用

## 安装方法 📦

```bash
# 克隆仓库
git clone https://github.com/your-username/ai-skills-distillation.git
cd ai-skills-distillation

# 技能使用标准Python - 无需额外依赖
python demo.py
```

## 快速开始 🚀

### 浪漫建议技能
```python
from romantic_advisor_skill import romantic_advice, generate_love_phrase

# 获取情感建议
advice = romantic_advice("我被拒绝了")
print(advice)

# 生成情话
phrase = generate_love_phrase()
print(phrase)
```

### 幽默恋爱技能
```python
from humorous_relationship_skill import (
    humorous_relationship_advice,
    generate_humorous_response,
    modern_love_advice
)

# 获取幽默建议
advice = humorous_relationship_advice("我被当舔狗了")
print(advice)

# 生成幽默回复
response = generate_humorous_response("她已读不回")
print(response)

# 获取现代建议
modern_advice = modern_love_advice()
print(modern_advice)
```

## 技能说明 📚

### 1. 浪漫建议技能
- **来源**: 情话.txt + 情话宝典.txt
- **功能**: 传统浪漫表达和建议
- **适用**: 正式情感咨询，情话生成

### 2. 幽默恋爱技能
- **来源**: 舔狗语录.txt  
- **功能**: 现代幽默回复和网络文化建议
- **适用**: 轻松情感调节，搞笑回复

## 项目结构 📁

```
ai-skills-distillation/
├── romantic_advisor_skill.py     # 浪漫建议技能
├── humorous_relationship_skill.py # 幽默恋爱技能
├── skill_config.json             # 技能配置
├── demo.py                       # 演示脚本
├── requirements.txt              # 依赖文件（空-无外部依赖）
└── docs/
    ├── README.md                 # 本文件
    └── usage_examples.md         # 详细使用示例
```

## 使用说明 📖

运行演示程序：
```bash
python demo.py
```

详细使用示例请查看 `docs/usage_examples.md`。

## 内容来源 📝

技能基于三个中文文本文件蒸馏生成：
1. **情话.txt**: 现实主义爱情观点和建议
2. **情话宝典.txt**: 传统浪漫表达和经典情话
3. **舔狗语录.txt**: 现代幽默恋爱表达和网络梗

## 参与贡献 🤝

欢迎贡献！您可以：
- 添加更多用于蒸馏的文本内容
- 改进技能算法和逻辑
- 增加新的技能功能
- 优化用户体验

## 许可证 📄

MIT许可证 - 详见[LICENSE](LICENSE)文件。

## 作者 ✍️

由Claude Code和AI助手创建。
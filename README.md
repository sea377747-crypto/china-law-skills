# My Skills

一组用于 AI 助手（Claude Code / 豆包等支持 Agent Skills 的环境）的结构化技能。

## 包含的技能

| 目录 | 说明 |
|---|---|
| [`book-to-skill/`](./book-to-skill) | 把书籍/文档（PDF、EPUB、DOCX、HTML、Markdown、TXT 等）转换为结构化技能的工具技能。 |
| [`china-civil-code/`](./china-civil-code) | 《中华人民共和国民法典》（2021 年施行，七编 1260 条）结构化技能：条文检索、构成要件、法律后果。 |
| [`china-labor-law/`](./china-labor-law) | 《中华人民共和国劳动法》＋《中华人民共和国劳动合同法》结构化技能：劳动合同、解除补偿、工时工资、劳务派遣、争议处理。 |

## 目录结构

```
my-skills/
├── book-to-skill/       # SKILL.md + scripts/ + docs/ ...
├── china-civil-code/    # SKILL.md + chapters/ + glossary/patterns/cheatsheet
└── china-labor-law/     # SKILL.md + chapters/ + glossary/patterns/cheatsheet
```

每个技能以 `SKILL.md` 为入口，`chapters/` 为分章内容，并按需提供 `glossary.md`（术语表）、`patterns.md`（分析框架）、`cheatsheet.md`（速查表）。

## 安装

把需要的技能目录复制到你的 Agent Skills 目录即可（例如 `~/.claude/skills/` 或对应环境的用户技能目录）。

## 使用

加载技能后直接提问，例如：
- “被公司违法辞退能要多少赔偿？”
- “加班费怎么算？”
- “合同成立的要件是什么？”

## 来源与许可声明

- **`book-to-skill/`** 为第三方开源项目，源自 <https://github.com/virgiliojr94/book-to-skill>，依据 **MIT 许可证**分发；其 `LICENSE.md` 及版权声明已原样保留，版权归原作者所有。
- **`china-civil-code/`、`china-labor-law/`** 为基于中国现行法律整理生成的结构化内容。根据《中华人民共和国著作权法》，法律、法规等官方文件本身不适用著作权法保护；技能内容为要件化、表格化的提炼整理。
- 法律内容可能随立法、行政法规及司法解释更新，使用时请以最新官方文本为准；本仓库内容不构成法律意见。

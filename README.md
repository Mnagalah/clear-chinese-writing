# 清晰中文写作

版本 **1.0.0** · [更新记录](CHANGELOG.md)

这是一个用于中文起草、修改、摘要和材料综合的 Agent Skill。它关注句子怎样断开、段落怎样衔接，以及修改后是否保留了原来的意思和口吻，适合报告、解释、访谈整理、专题文章和技术说明。

技能会根据任务选择参考文件。简短问答直接回答，实质改稿侧重句段与语气，长文起草和材料综合侧重内容组织。语言学、标点和文档规范的相关内容已整理成包内摘记，并注明出处；使用时无需先下载教材或打开来源链接。

## 安装到 Codex

1. 下载仓库 ZIP 或版本附件并解压，将含有 `SKILL.md` 的文件夹命名为 `clear-chinese-writing`。
2. 将整个文件夹放入个人技能目录 `~/.agents/skills/`。如果只想在一个项目中使用，也可放入该项目的 `.agents/skills/`。
3. 在 Codex 中选择“清晰中文写作”。CLI 和 IDE 扩展可输入 `$clear-chinese-writing` 调用；如果技能没有出现，重启 Codex 后再试。

个人安装后的文件位置应为：

```text
~/.agents/skills/clear-chinese-writing/SKILL.md
~/.agents/skills/clear-chinese-writing/agents/openai.yaml
~/.agents/skills/clear-chinese-writing/references/…
```

请保留整个文件夹，不要只复制 `SKILL.md`。已有同名技能时，先把旧版移到技能目录之外备份，避免同时加载两份。

安装路径和调用方式依据 [OpenAI 的技能文档](https://learn.chatgpt.com/docs/build-skills)，于 2026-10-22 核对。本技能由文本文件组成，不需要安装额外的脚本或软件依赖。

## 使用示例

输入以下任一句，再附上原文或材料：

```text
$clear-chinese-writing 润色以下文字。
```

```text
$clear-chinese-writing 整理以下访谈，保留受访者的口吻。
```

```text
$clear-chinese-writing 根据以下材料写一篇分析。
```

有读者、篇幅或文体要求时，再补充说明。

## 试用与反馈

建议先用自己熟悉的原稿试改，留着原文对照。改稿可能修顺了一句话，却改变了人物语气或打断段落；反馈这类问题时，请带上前后文。也欢迎提供只需小改、甚至适合保持原样的例子。

可在仓库的 Issues 中选择“写作试用反馈”，或参照[反馈模板](.github/ISSUE_TEMPLATE/writing-feedback.md)记录。请注明使用的工具、模型、技能版本，附上任务要求、原文、实际输出，并指出具体哪里不合适；有更顺的改法也可以一并提供。提交前请去除不便公开的内容。

不同模型和材料的效果可能不同。包内例句用于说明编辑取舍，不能作为固定句式套用，也不能代替对完整改稿的判断。

## 文件说明

| 文件 | 用途 |
|---|---|
| [SKILL.md](SKILL.md) | 任务入口与共同要求 |
| `agents/openai.yaml` | 界面名称和调用提示 |
| [editing.md](references/editing.md) | 断句、语气、段落衔接与改稿取舍 |
| [craft.md](references/craft.md) | 材料综合、解释与叙述、标题与收尾 |
| [choices.md](references/choices.md) | 不同文体和标题的完整示例 |
| [evidence-review.md](references/evidence-review.md) | 复杂事实、数字和引语核对 |
| [document-conventions.md](references/document-conventions.md) | 文档格式与排版 |
| [reference-choices.md](references/reference-choices.md) | 三份离线资料摘记的查阅导航 |
| `references/source-notes/` | 语言与篇章、标点与标题、格式规范的摘记及出处 |
| [evaluation.md](references/evaluation.md) | 维护者使用的试写比较方法 |

参考文件按需读取，不必在每次写作前全部加载。

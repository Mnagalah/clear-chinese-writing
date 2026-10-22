# 清晰中文写作

版本 **1.0.0** · [更新记录](CHANGELOG.md)

一个用于中文写作的 Agent Skill，可用于修改文章、整理访谈，以及根据材料起草报告、摘要和分析。修改时着重理顺文章的逻辑、分段和表达，保留原文的意思与口吻。

## 安装到 Codex

1. 下载仓库 ZIP 并解压，将含有 `SKILL.md` 的文件夹命名为 `clear-chinese-writing`。
2. 将整个文件夹放入 `~/.agents/skills/`；仅供单个项目使用时，放入该项目的 `.agents/skills/`。
3. 在 Codex 中选择“清晰中文写作”，或在 CLI、IDE 扩展中输入 `$clear-chinese-writing`。如果技能没有出现，重启 Codex 后再试。

个人安装后，入口文件位于：

```text
~/.agents/skills/clear-chinese-writing/SKILL.md
```

已有同名技能时，先将旧文件夹移到技能目录之外备份，再放入新版。安装说明参见 [OpenAI 技能文档](https://learn.chatgpt.com/docs/build-skills)。

## 使用方法

输入要求后，附上原文或材料。有明确的读者、用途或篇幅要求时，一并说明。

### 调整文章结构

需要重新梳理文章的顺序和段落时，可以这样写：

```text
$clear-chinese-writing 修改以下文章，调整好文章的逻辑和分段。
```

### 其他常见用法

| 任务 | 提示词 |
|---|---|
| 润色文字 | `$clear-chinese-writing 润色以下文字。` |
| 整理访谈 | `$clear-chinese-writing 整理以下访谈，保留受访者的口吻。` |
| 根据材料写作 | `$clear-chinese-writing 根据以下材料写一篇分析。` |

## 反馈问题

如果改稿有不自然、改变原意或段落不顺的地方，可在仓库的 Issues 中选择“写作试用反馈”。请按[反馈模板](.github/ISSUE_TEMPLATE/writing-feedback.md)附上原文、提示词和输出结果，注明模型及技能版本，并指出具体问题。有自己的改法，也可以一并提供。

公开提交前，请删去私人信息。

## 参考资料

写作要求见 [SKILL.md](SKILL.md)。语言学、标点和文档规范的要点已整理在技能文件夹中，并注明出处，Codex 会按任务读取。

<details>
<summary>查看文件与资料</summary>

- 文章修改：[句段与语气](references/editing.md)、[内容组织](references/craft.md)、[改写示例](references/choices.md)。
- 核对与排版：[事实、数字和引语](references/evidence-review.md)、[文档规范](references/document-conventions.md)。
- 资料出处：[参考说明](references/reference-choices.md)。
- 技能维护：[试写比较方法](references/evaluation.md)。

</details>

# dbskill

dontbesilent 商业诊断工具箱。基于 12,307 条推文提炼的方法论，用 Claude Code skill 实现。

## 工具箱

| Skill | 触发方式 | 做什么 |
|---|---|---|
| `/dbs` | `/dbs`、`帮我看看` | 主入口，自动路由到对的工具 |
| `/dbs-diagnosis` | `/dbs-诊断`、`我有个商业问题` | 商业模式诊断。消解问题，不回答问题 |
| `/dbs-benchmark` | `/dbs-对标`、`我该模仿谁` | 对标分析。五重过滤，排除噪音 |
| `/dbs-topic` | `/dbs-选题`、`这个选题怎么样` | 选题判断。IP 五大公理逐条检验 |
| `/dbs-content` | `/dbs-content`、`这个内容怎么做` | 内容创作诊断。五维检测 |
| `/dbs-unblock` | `/dbs-自检`、`我总是拖延` | 执行力诊断。阿德勒框架 |
| `/dbs-deconstruct` | `/dbs-拆概念`、`这个词什么意思` | 概念拆解。维特根斯坦式审查 |

## 工作流

```
diagnosis（商业模式对不对）
    ↓
benchmark（找谁模仿）
    ↓
topic（选题值不值得做）
    ↓
content（内容怎么做）
    ↓
unblock（做不动怎么办）

deconstruct（随时拆概念）
```

## 使用方式

1. 把 `dbskill/` 目录放到你的项目中
2. 每个子目录的 `SKILL.md` 是完整的 skill 定义
3. 在 Claude Code 中用 `/dbs` 启动，或直接调用具体 skill

## 知识库

skill 依赖本地知识库（未包含在仓库中），从推文中按 8 个主题分类：

- 商业本体论（609 条）
- IP 与内容（872 条）
- 思维与哲学（135 条）
- 实操运营（206 条）
- AI 与工具（559 条）
- 教育与课程（59 条）
- 心理与执行（69 条）
- 人生与认知（33 条）

## 作者

[dontbesilent](https://x.com/dontbesilent)

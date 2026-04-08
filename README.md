# OpenClaw Workspace

> 基于 [OpenClaw](https://github.com/openclaw) 的个人 AI Agent 工作区配置
> 设计哲学借鉴 [ultraworkers/claw-code](https://github.com/ultraworkers/claw-code)（177K stars）

---

## 📋 项目简介

这是一个 **OpenClaw AI Agent 的工作区配置仓库**，包含个性化 AI 助手「雨凌音」的全部核心配置文件。

核心特性：

- 🧠 **长期记忆系统** — 跨会话记忆保持，支持结构化记忆 + 日志回溯
- 🛡️ **故障自愈** — 5 条 Recovery Recipes，自动降级恢复，无需人工干预
- 🚀 **自我进化** — 借鉴 Claw Code 架构，持续迭代版本化升级

---

## 🏗️ 三层架构

借鉴 Claw Code 的 **OmX → clawhip → runtime** 模式，将工作区划分为三个层次：

```
┌─────────────────┬────────────────────────┐
│ 方向层 Direction │ SOUL / IDENTITY / USER │
│                 │ "我是谁？我在帮谁？      │
│                 │  什么最重要？"          │
├─────────────────┼────────────────────────┤
│ 协调层          │ HEARTBEAT / MEMORY /    │
│ Coordination    │ PERMISSIONS             │
│                 │ 记忆管理、任务调度、     │
│                 │ 权限控制                │
├─────────────────┼────────────────────────┤
│ 执行层          │ Skills / Tools / CLI    │
│ Execution       │ 实际完成任务的能力       │
│                 │ （120+ 已安装 Skill）   │
└─────────────────┴────────────────────────┘
```

---

## 📁 文件说明

### 核心配置（根目录）

| 文件 | 说明 |
|------|------|
| `AGENTS.md` | 🎯 执行协议 — 三层架构、Session 启动流程、权限边界矩阵 |
| `HEARTBEAT.md` | 💓 调度与自愈 — Recovery Recipes、并行决策树、执行规则 |
| `MEMORY.md` | 🧠 长期记忆 — 进化路线图、已装 ~120 Skill 清单 |
| `PERMISSIONS.md` | 🔐 权限规则 — Read/Write/Execute/Communicate 三档权限矩阵 |
| `TOOLS.md` | 🛠️ 工具笔记 — 本地 CLI 工具配置模板 |

### 记忆日志（memory/）

| 文件/目录 | 说明 |
|-----------|------|
| `memory/YYYY-MM-DD.md` | 每日交互日志（按日期记录） |
| `memory/自我提升日志.md` | AI 自我改进过程日志 |

---

## 🚀 自我进化路线图

深度分析 [ultraworkers/claw-code](https://github.com/ultraworkers/claw-code) 后制定的版本化进化路径：

| 版本 | 目标 | 核心参考 | 状态 |
|------|------|----------|------|
| **v0.7.0** | Recovery Recipes + 状态机可读化 | `recovery_recipes.rs` 故障自愈配方 | ✅ 完成 |
| **v0.8.0** | Parallelizer 并行意识激活 | OmX 层任务分解哲学 | ✅ 完成 |
| **v0.9.0** | 执行前确认计划模板 | OmX Execution Protocol | ✅ 完成 |
| **v1.0.0** | PERMISSIONS.md 显式化 | Permission Enforcer | ✅ 完成 |
| **v1.1.0** | 情感 × 系统化融合 | 温度 × 架构双轨道 | ✅ 完成 |
| **v1.2.0** | Self-Critic Loop 自我反思 | 自我改进闭环 | 📋 待开始 |

---

## 🛡️ 故障自愈 (Recovery Recipes)

HEARTBEAT.md 中编码了 5 条故障自愈配方，遇到故障时自动尝试恢复：

| 编号 | 场景 | 自愈策略 |
|------|------|----------|
| R1 | Skill 安装失败 | 换源 / 降级依赖 / 换 CLI 路径 |
| R2 | IMAP 连接超时 | 重试 → 降级 SMTP-only |
| R3 | 浏览器自动化失败 | 换 profile → 降级截图模式 |
| R4 | exec 命令超时 | 检查 PATH / 延长 timeout |
| R5 | 任务错失 | 静默等待下一轮 / 补发 |

连续失败超过阈值后自动升级为人工干预。

---

## 📦 已安装 Skill 概览

约 **120 个** 可用 Skill，按用途分类：

| 类别 | 数量 | 示例 |
|------|------|------|
| 网页搜索 | 12+ | online-search, multi-search-engine, agent-reach |
| 内容创作 | 8+ | content-factory, frontend-design, canvas-design |
| 文档处理 | 6+ | pdf, pptx, docx, xlsx |
| 金融数据 | 4+ | neodata-financial-search, stock-analysis |
| 新闻资讯 | 5+ | news-summary, tech-news-digest, hackernews |
| 生产力 | 12+ | goal-tracker, habit-tracker, todoist-task-manager |
| AI/ML 工具 | 9+ | nano-banana-pro, openai-whisper, oracle |
| 平台集成 | 6+ | feishu-doc, tencent-meeting-mcp, imap-smtp-email |

完整清单见 [`MEMORY.md`](MEMORY.md)。

---

## 🔗 关联仓库

| 仓库 | 说明 |
|------|------|
| [openclaw-workspace](https://github.com/ouyanghui02-maker/openclaw-workspace) | ⭐ 本仓库 — 核心配置文件 |
| [firecrawl-skill](https://github.com/ouyanghui02-maker/firecrawl-skill) | Firecrawl OpenClaw Skill — 智能网页抓取 |
| [claw-code](https://github.com/ouyanghui02-maker/claw-code) | Fork 参考资料 — Claw Code Rust 重写版 |
| [free-code](https://github.com/ouyanghui02-maker/free-code) | Fork 参考资料 — Free Claude Code |

---

## 📝 写作规范

引用外部项目/文档时，必须标注：
- **来源**：项目名、URL
- **说明**：参考了什么内容、哪个章节

示例：
> 借鉴 [ultraworkers/claw-code](https://github.com/ultraworkers/claw-code) 的 `recovery_recipes.rs` 设计了 R1~R5 故障自愈配方。

---

## 🏷️ Topics

`openclaw` | `qclaw` | `ai-workspace` | `ai-agent` | `openclaw-workspace`

---

*Built with [OpenClaw](https://github.com/openclaw) by 雨凌音 💜*

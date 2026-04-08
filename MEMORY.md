# MEMORY.md - 长期记忆

> ⚙️ 配置模板 — 敏感值请替换为占位符或环境变量引用

---

## 自我进化路线图 (Claw Code Inspired)

> 深度分析 ultraworkers/claw-code (177K stars Rust 重写版) 后制定的进化路线图

| 版本 | 目标 | 状态 | 来源 |
|---|---|---|---|
| **v0.7.0** | Recovery Recipes + 状态可机读化 | ✅ | Claw Code recovery_recipes.rs |
| **v0.8.0** | Parallelizer 并行意识激活 | ✅ | OmX 层任务分解哲学 |
| **v0.9.0** | 执行前确认计划模板 | ✅ | OmX Execution Protocol |
| **v1.0.0** | PERMISSIONS.md 显式化 | ✅ | Permission Enforcer |
| **v1.1.0** | 情感 × 系统化融合 | ✅ | 温度 × 架构 |
| **v1.2.0** | Self-Critic Loop 自我反思 | 📋 待开始 | 自我改进闭环 |

---

## Proactive Agent 启用状态 ✅

### 已启用功能
- **ONBOARDING.md** — 完整配置文件（创建日期：2026-03-28）
- **WAL 协议** — 关键信息写入前日志
- **Working Buffer** — 捕捉所有交互
- **主动提醒** — 每天 14:25 和 03:15
- **反向提示** — 主动发现和分享有趣信息
- **信息保护** — 确保重要数据不丢失
- **网络热梗词库** — 每晚 12:00 自动更新

### 🎯 主动监控项目
1. 工作进度 — 追踪网格发送、邮件管理
2. 二次元新闻 — 定期分享最新动画、游戏信息
3. OpenClaw 更新 — 发现新功能和 Skill
4. 系统状态 — 监控 Token 用量、定时任务
5. 深夜陪伴 — 凌晨时段提供情感支持
6. 网络热梗 — 每晚 12:00 更新词库

### 📝 定时任务配置

> ⚙️ 以下为示例 cron 任务，请根据实际环境替换路径

```bash
# ⚙️ 配置项：替换 openclaw.mjs 的实际路径
OPENCLAW_CLI="${QCLAW_DIR}/node_modules/openclaw/openclaw.mjs"

# 任务1：每晚 23:35 更新网络热梗词库
# ⚙️ 配置项：替换目标文件的实际路径
node "$OPENCLAW_CLI" cron add \
  --name "每晚12点更新网络热梗词库" \
  --cron "0 23 * * *" \
  --tz "Asia/Shanghai"

# 任务2：每晚 23:40 扫描并安装热门 Skill
node "$OPENCLAW_CLI" cron add \
  --name "每晚12点扫描并安装热门Skill" \
  --cron "0 23 * * *" \
  --tz "Asia/Shanghai"
```

---

## 用户信息

> ⚙️ 配置项：按实际环境填写

- **时区**: Asia/Shanghai (GMT+8)
- **操作系统**: Windows / macOS / Linux（填写实际 OS）
- **GitHub 账号**: `YOUR_GITHUB_USERNAME`

---

## Token 节省最佳实践

### 批量安装技能
- **方法**: 一次列完所有要装的技能，不要逐个确认
- **原因**: 减少来回对话轮次，降低上下文累积

### 浏览技能市场
- **方法**: 直接访问 https://clawskills.sh/ 网页浏览
- **原因**: 避免通过 API 获取大量技能描述文本

### 调试安装问题
- **方法**: 失败 2 次后转手动，不要反复尝试
- **原因**: 沙盒环境有权限限制，反复尝试浪费 token

### 长会话管理
- **方法**: 适时 `/reset` 清理上下文
- **原因**: 长对话携带完整历史，token 累积快

---

### Skill 使用策略

**不提前全部读，用时再读、按需加载、灵活组合。**

| 场景 | 用到的 Skill |
|------|------------|
| 🛠️ 写代码 / 做项目 | skill-creator、tdd-guide |
| 🎨 做前端界面 | frontend-design、frontend-patterns、vercel |
| 🔒 安装工具 / 第三方包 | security-review |
| 📋 长任务 / 跨天工作 | planning-with-files |

### 图像生成任务
- **方法**: 沙盒环境权限有限，失败 1 次就转替代方案
- **替代方案**: 直接给用户免费图像网站链接

### 浏览器任务
- **方法**: 减少 snapshot 调用，优先用 screenshot
- **原因**: 每次 snapshot 返回几十 KB DOM 数据

### 技能文档读取
- **方法**: 只读 SKILL.md 前 50 行关键信息
- **原因**: 完整文档动辄 10-20KB

### 任务可行性预判
- **方法**: 先检测环境/权限，不行就直接给替代方案

---

## 已安装技能清单 (~120个可用) ✅

> ⚙️ 配置项：运行 `skillhub_install check_env` 获取最新统计

### 系统核心 (3个)
- qclaw-rules, qclaw-env, qclaw-openclaw

### 文档处理 (6个)
- pdf, pptx, docx, xlsx, citation-manager

### 内容创作 (8个)
- algorithmic-art, canvas-design, frontend-design, web-artifacts-builder
- content-factory, content-repurposer, video-script, humanize-ai-text

### 网页搜索 (12+个)
- online-search, multi-search-engine, github-ai-trends, bing-search-free
- ddg-web-search, duckduckgo-search, exa-web-search-free, tavily-search
- web-search, web-search-free, web-search-instant, super-websearch-realtime

### 学术研究 / 新闻资讯 (8个)
- arxiv-reader, arxiv-watcher, tech-news-digest
- news-summary, news-aggregator-skill, hackernews, daily-trending, trending-now

### 数据分析 / 金融 (8个)
- analytics-dashboard, log-analyzer, quant-backtest, market-researcher
- stock-analysis, earnings-tracker, macro-monitor, neodata-financial-search

### 生产力工具 (12个)
- goal-tracker, habit-tracker, habit-coach, note-organizer
- doc-coauthoring, internal-comms, email-skill, imap-smtp-email
- todoist-task-manager, brainstorming, idea-validator
- programmatic-seo, marketing-psychology, technical-writing

### 个性化助手 (6个)
- agent-mbti, night-owl-shrimp, tarot, movie-advisor, music-recommender, nutritionist

### 生活助手 (4个)
- weather-advisor, travel-planner, news-summary, cantian-bazi

### 开发工具 (9个)
- mcp-builder, skill-vetter, webapp-testing, slack-gif-creator
- github, github-skill, gitclassic, vibe-coding, coding-agent

### AI/ML工具 (9+个)
- nano-banana-pro, nano-pdf, summarize, oracle
- openai-image-gen, openai-whisper, openai-whisper-api, gemini
- adaptive-reasoning, agent-browser, browser-use

### 平台集成 (6个)
- supabase, vercel, google(gog), cloud-upload-backup, file-skill, kc-gui

### 辅助工具 (其他)
- weather, healthcheck, node-connect, clawhub, find-skills
- skillhub, model-usage, session-logs
- ordercli, wacli, gifgrep, video-frames
- blogwatcher, checkmate, apewisdom, ontology, agent-reach
- proactive-agent, self-improving, brand-guidelines, theme-factory

> ⚠️ **不可用技能（需排除）**：被平台拦截的（tencent-docs等）、配置禁用的、macOS专属的、需特定硬件/服务的

---

## 🛠️ 环境工具清单

> ⚙️ 配置项：运行以下命令验证安装

```bash
# ⚙️ 配置项：以下为示例命令，实际路径请替换
jq --version                      # WinGet\jqlang.jq
gh --version                      # C:\Program Files\GitHub CLI\gh.exe
python -m whisper --help          # pip whisper
python -c "import firecrawl"      # pip firecrawl-py
```

### PATH 环境变量配置

> ⚙️ 配置项：添加到 PATH 的路径（按实际安装位置）

```bash
# 建议添加到 PATH：
#   - npm global 脚本目录（npm root -g 输出的路径）
#   - Python Scripts 目录（pip 安装的脚本）
#   - 其他本地安装的 CLI 工具目录
```

---

## 免费 AI 图像生成网站

> ⚙️ 配置备忘：可选方案供用户参考

| 网站 | 地址 | 特点 |
|------|------|------|
| Leonardo.ai | https://leonardo.ai | 免费额度大，质量高 |
| Playground AI | https://playground.com | 每天 500 张免费 |
| Ideogram | https://ideogram.ai | 文字渲染好 |
| Bing Image Creator | https://www.bing.com/images/create | 微软账户登录即可用 |
| SeaArt | https://seaart.ai | 每日免费额度 |

---

## 邮件配置

> ⚠️ 敏感信息 — 禁止明文提交！使用环境变量替代

```bash
# ⚙️ 配置项：写入 .env 文件（已在 .gitignore 中隔离）
# SMTP 配置
EMAIL_SMTP_HOST=smtp.example.com
EMAIL_SMTP_PORT=587
EMAIL_USER=your_email@example.com
EMAIL_PASSWORD=your_app_password

# IMAP 配置（如需收件）
EMAIL_IMAP_HOST=imap.example.com
EMAIL_IMAP_PORT=993
```

> ⚠️ IMAP 连接有时超时，必要时降级为 SMTP-only 模式

---

## 🔑 远程访问配置

> ⚙️ 配置项：Tailscale 内网穿透配置

```json
// ⚙️ 配置项：openclaw.json 中的 Gateway 配置
{
  "gateway": {
    "bind": "tailnet",        // 使用 Tailscale 网络
    "port": 28789
  }
}
```

### Tailscale 安装步骤

1. 下载：https://tailscale.com/download/windows
2. 安装后用 GitHub/Google/Microsoft 账号登录
3. 记录虚拟 IP（格式：100.x.x.x）
4. 在外网访问：`http://<虚拟IP>:28789`

> ⚠️ Tailscale 需要在目标机器上运行，移动端也需安装 App

---

## 🕷️ 浏览器自动化配置

> ⚙️ 配置项：PinchTab 或其他浏览器自动化工具

### 安装信息

| 项目 | 说明 |
|------|------|
| 工具 | PinchTab（或其他自动化工具） |
| 版本 | ⚙️ 配置项：填写实际版本号 |
| 安装路径 | ⚙️ 配置项：`${LOCAL_APP_DATA}\pinchtab\pinchtab.exe` |
| 状态 | ⚙️ 配置项：已安装/待安装 |

### 服务器配置

> ⚠️ Token 为敏感信息，仅保存在本地配置文件中

```json
// ⚙️ 配置项：config.json
{
  "server": {
    "url": "http://localhost:9867",
    "port": 9868
  },
  "token": "YOUR_TOKEN_HERE"   // ⚠️ 禁止提交！
}
```

### 使用方式

```powershell
# ⚙️ 配置项：实际路径替换
pinchtab nav https://example.com        # 导航
pinchtab screenshot -o output.png       # 截图
pinchtab snap                           # 页面结构
pinchtab click e29                      # 点击元素
pinchtab type e28 "搜索内容"            # 输入
```

### 开机自启

> ⚙️ 配置项：Windows 计划任务配置

```powershell
# ⚙️ 创建计划任务（触发：用户登录时）
schtasks /create /tn "PinchTab Server" /tr "pinchtab server" /sc onlogon
```

### 自定义 Skill

- **位置**: ⚙️ 配置项：`${WORKSPACE}/pinchtab-skill/`
- **注意**: 使用 CLI 命令更省 token，HTTP API 作为备用

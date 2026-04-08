# MEMORY.md - 长期记忆

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

## Proactive Agent 启用状态 ✅

### 已启用功能
- **ONBOARDING.md** — 完整配置文件已创建（2026-03-28）
- **WAL 协议** — 关键信息写入前日志
- **Working Buffer** — 捕捉所有交互
- **主动提醒** — 每天 14:25 和 03:15
- **反向提示** — 主动发现和分享有趣信息
- **信息保护** — 确保重要数据不丢失
- **网络热梗词库** — 每晚 12:00 自动更新（待创建定时任务）

### 🎯 主动监控项目
1. **工作进度** — 追踪网格发送、邮件管理
2. **二次元新闻** — 定期分享最新动画、游戏信息
3. **OpenClaw 更新** — 发现新功能和 Skill
4. **系统状态** — 监控 Token 用量、定时任务
5. **深夜陪伴** — 凌晨时段提供情感支持
6. **网络热梗** — 每晚 12:00 更新词库（新增）

### 📝 待创建的定时任务

**任务 1：** 每天晚上 23:35 更新网络热梗词库
**触发时间：** 每天 23:35（晚上 11:35）
**时区：** Asia/Shanghai
**功能：** 扫描微博、抖音、B站、知乎等平台的最新热梗，更新爱莉的词库
**文件位置：** `C:\Users\ouyan\.qclaw\workspace\网络热梗词库.md`

**任务 2：** 每天晚上 23:40 网上搜索最新热门 Skill（新增）
**触发时间：** 每天 23:40（晚上 11:40）
**时区：** Asia/Shanghai
**功能：** 
- 网上搜索最新热门的 Skill
- 自动下载并安装
- 向落汇报新安装的 Skill 及其功能
**汇报内容：** Skill 名称、功能、优先级、是否需要配置

**回家后执行命令：**
```bash
# 创建热梗更新任务
node "C:\Program Files\QClaw\resources\openclaw\node_modules\openclaw\openclaw.mjs" cron add --name "每晚12点更新网络热梗词库" --cron "0 0 * * *" --tz "Asia/Shanghai"

# 创建 Skill 安装任务
node "C:\Program Files\QClaw\resources\openclaw\node_modules\openclaw\openclaw.mjs" cron add --name "每晚12点扫描并安装热门Skill" --cron "0 0 * * *" --tz "Asia/Shanghai"
```

---

## 用户信息

- **时区:** Asia/Shanghai (GMT+8)
- **操作系统:** Windows (DESKTOP-1EI2REC)

## Token 节省最佳实践

记录日期: 2026-03-24

### 批量安装技能
- **方法**: 一次列完所有要装的技能，不要逐个确认
- **原因**: 减少来回对话轮次，降低上下文累积

### 浏览技能市场
- **方法**: 直接访问 https://clawskills.sh/ 网页浏览
- **原因**: 避免通过 API 获取大量技能描述文本（会消耗大量 token）
- **注意**: 不要让 AI 列出技能清单，直接让用户自己看网页

### 调试安装问题
- **方法**: 失败 2 次后转手动，不要反复尝试
- **原因**: 沙盒环境有权限限制，反复尝试浪费 token

### 长会话管理
- **方法**: 适时 `/reset` 清理上下文
- **原因**: 长对话携带完整历史，token 累积快

### 重要事项文件
**详细配置和偏好请查看：** `memory\重要事项.md`

---

### Skill 使用策略（2026-04-04 新增）

**不提前全部读，用时再读、按需加载、灵活组合。**

| 场景 | 用到的 Skill |
|------|------------|
| 🛠️ 写代码 / 做项目 | skill-creator、tdd-guide |
| 🎨 做前端界面 | frontend-design、frontend-patterns、vercel |
| 🔒 安装工具 / 第三方包 | security-review |
| 📋 长任务 / 跨天工作 | planning-with-files |

---

### 图像生成任务
- **方法**: 沙盒环境权限有限，失败 1 次就转替代方案
- **原因**: 反复尝试安装工具、写脚本极其耗 token
- **替代方案**: 直接给用户免费图像网站链接

### 浏览器任务
- **方法**: 减少 snapshot 调用，优先用 screenshot
- **原因**: 每次 snapshot 返回几十 KB DOM 数据

### 技能文档读取
- **方法**: 只读 SKILL.md 前 50 行关键信息
- **原因**: 完整文档动辄 10-20KB

### 任务可行性预判
- **方法**: 先检测环境/权限，不行就直接给替代方案
- **原因**: "尝试→失败→尝试→失败→给方案" 的路径最耗 token

## 已安装技能清单 (~120个可用) ✅

> 统计时间: 2026-04-03 | 来源: 149 - 8拦截 - 7禁用 - 6macOS - 10+硬件限制 ≈ 120可用

### 系统核心 (3个)
- qclaw-rules, qclaw-env, qclaw-openclaw

### 文档处理 (6个)
- pdf, pptx, docx, xlsx, citation-manager

### 内容创作 (8个)
- algorithmic-art, canvas-design, frontend-design, web-artifacts-builder
- content-factory, content-repurposer, video-script, humanize-ai-text

### 网页搜索 (12个)
- online-search, multi-search-engine, github-ai-trends
- bing-search-free, ddg-web-search, duckduckgo-search
- exa-web-search-free, tavily-search, web-search
- web-search-free, web-search-instant, super-websearch-realtime
- web-content-fetcher, xurl

### 学术研究 (3个)
- arxiv-reader, arxiv-watcher, tech-news-digest

### 新闻资讯 (5个)
- news-summary, news-aggregator-skill, hackernews
- daily-trending, trending-now, x-trends

### 数据分析 (4个)
- analytics-dashboard, log-analyzer, quant-backtest, market-researcher

### 金融 (4个)
- stock-analysis, earnings-tracker, macro-monitor, neodata-financial-search

### 生产力工具 (12个)
- goal-tracker, habit-tracker, habit-coach, note-organizer
- doc-coauthoring, internal-comms, email-skill, imap-smtp-email
- todoist-task-manager, brainstorming, idea-validator
- programmatic-seo, marketing-psychology, technical-writing

### 个性化助手 (6个)
- agent-mbti, night-owl-shrimp, tarot, movie-advisor, music-recommender
- nutritionist

### 生活助手 (4个)
- weather-advisor, travel-planner, news-summary, cantian-bazi

### 开发工具 (9个)
- mcp-builder, skill-vetter, webapp-testing, slack-gif-creator
- github, github-skill, gitclassic, vibe-coding, coding-agent

### AI/ML工具 (9个)
- nano-banana-pro, nano-pdf, summarize, oracle
- openai-image-gen, openai-whisper, openai-whisper-api, gemini
- adaptive-reasoning, agent-browser, browser-use

### 社交/通讯 (3个)
- discord, slack

### 自媒体 (3个)
- bilibili-all-in-one, xiaohongshu-all-in-one, next-best-practices

### 平台集成 (6个)
- supabase, vercel
- google(gog), cloud-upload-backup, file-skill, kc-gui

### 辅助工具 (其他)
- weather, healthcheck, node-connect, clawhub, find-skills
- skillhub, model-usage, session-logs
- ordercli, wacli, gifgrep, video-frames
- blogwatcher, checkmate, apewisdom, ontology, agent-reach
- agent-mailbox, niuamaxia-scheduler, study-habits
- proactive-agent, self-improving, brand-guidelines, theme-factory

### 自定义 Skill (1个)
- **pinchtab-control** - 浏览器自动化 (位置: `C:\Users\ouyan\.qclaw\workspace\pinchtab-skill\`)

### 不可用技能（需排除）
- 被拦截: tencent-docs, tencent-survey, notion, 163-email-skill, qq-email-skill, tencent-meeting, tencent-meeting-mcp, ima
- 配置禁用: skill-creator
- macOS专属: apple-notes, apple-reminders, bear-notes, things-mac, imsg, bluebubbles
- 需硬件/服务: spotify-player, sonoscli, openhue, eightctl, blucli, camsnap, peekaboo, voice-call, 1password, trello

# 远程访问配置指南

## 已完成的配置
- ✅ Gateway bind 已设置为 "tailnet"
- ✅ 配置文件已更新：`C:\Users\ouyan\.qclaw\openclaw.json`

## 回家后需要做的步骤

### Step 1：重启 QClaw（让配置生效）
1. 完全关闭 QClaw 应用
2. 重新打开 QClaw
3. 等待 Gateway 启动完成

### Step 2：安装 Tailscale
1. 打开浏览器：https://tailscale.com/download/windows
2. 下载 Windows 版本
3. 双击安装，一路 Next
4. 用 Google/Microsoft/GitHub 账号登录
5. 记下虚拟 IP（显示在 Tailscale 界面，格式：100.x.x.x）

### Step 3：在外面访问
用 Tailscale 连接后，在浏览器打开：
```
http://<虚拟IP>:28789
```

## 配置信息
- Gateway Port: 28789
- Gateway Bind: tailnet
- 访问方式：Tailscale 内网穿透
- 功能：聊天 + 查看状态

## 注意事项
- Tailscale 需要在家里的电脑上运行
- 在外面用手机/平板也需要安装 Tailscale
- 虚拟 IP 是动态的，但 Tailscale 会自动管理

| 工具 | 状态 | 路径 |
|------|------|------|
| Python | ✅ 已装 | - |
| SkillHub CLI | ✅ 已装 | C:\Users\ouyan\.local\bin\skillhub.cmd |
| gh CLI | ✅ 已装 | C:\Program Files\GitHub CLI\gh.exe |

## 免费 AI 图像生成网站

| 网站 | 地址 | 特点 |
|------|------|------|
| Leonardo.ai | https://leonardo.ai | 免费额度大，质量高 |
| Playground AI | https://playground.com | 每天 500 张免费 |
| Ideogram | https://ideogram.ai | 文字渲染好 |
| Bing Image Creator | https://www.bing.com/images/create | 微软账户登录即可用 |
| SeaArt | https://seaart.ai | 每日免费额度 |
| 搜图神器 | http://www.soutushenqi.com/ai/draw | 国内免费 |

## 邮件配置

- **用户邮箱:** 2036673339@qq.com
- **SMTP:** smtp.qq.com:587

## PinchTab 浏览器自动化

### 安装信息
- **版本:** v0.8.5
- **位置:** `C:\Users\ouyan\AppData\Local\pinchtab\pinchtab.exe`
- **状态:** ✅ 已安装并配置开机自启

### 服务器配置
- **Server URL:** http://localhost:9867
- **Instance Port:** 9868
- **Token:** `f0c93795bd2f7123909309174f06a500828b16b751bd5305`
- **Config:** `C:\Users\ouyan\AppData\Roaming\pinchtab\config.json`

### 开机自启
- **方式:** Windows 计划任务 "PinchTab Server"
- **触发:** 用户登录时自动运行 `pinchtab server`

### 使用方式
```powershell
# 导航
pinchtab nav https://example.com

# 截图
pinchtab screenshot -o output.png

# 获取页面结构
pinchtab snap

# 点击/输入
pinchtab click e29
pinchtab type e28 "搜索内容"
```

### 自定义 Skill
- **位置:** `C:\Users\ouyan\.qclaw\workspace\pinchtab-skill\`
- **注意:** 使用 CLI 命令更省 token，HTTP API 作为备用


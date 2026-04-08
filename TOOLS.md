# TOOLS.md - 本地工具配置说明

> ⚙️ 配置模板 — 所有敏感值（路径/账号/密钥）请替换为实际内容或环境变量引用

---

## 📧 邮箱配置

> ⚙️ 配置项：替换为自己的邮箱账号和配置路径

```markdown
- **邮箱**: YOUR_EMAIL@example.com
- **IMAP/SMTP**: 已在配置文件中设置
- **配置文件**: ${WORKSPACE}/.env
- **skill 目录**: ${WORKSPACE}/email-skill
```

### 配置步骤

1. **SMTP 发件**
   ```bash
   node ${WORKSPACE}/email-skill/smtp-test.js
   ```

2. **IMAP 收件**
   ```bash
   node ${WORKSPACE}/email-skill/imap.js check --limit 10
   ```

> ⚠️ IMAP 连接有时超时（检查网络或 SMTP-only 模式降级）

---

## 🛠️ CLI 工具清单

> ⚙️ 配置项：按实际安装的工具和路径填写

| 工具 | 用途 | 来源 | 备注 |
|------|------|------|------|
| jq | JSON 处理 | winget / brew | — |
| ripgrep | 文本搜索 | winget / brew | — |
| ffmpeg | 音视频处理 | winget | — |
| gh | GitHub CLI | winget | 需 `gh auth login` |
| uv | Python 包管理 | npm | — |
| mcporter | MCP 工具调用 | npm global | — |
| clawhub | SkillHub 管理 | npm global | — |
| whisper | 语音转文字 | pip | Python312 |
| himalaya | 邮箱管理 | GitHub | — |
| sag | 语音合成（TTS） | GitHub | — |

### PATH 配置

> ⚙️ 配置项：添加以下路径到系统 PATH
```
${PATH_APPEND}:
  - ${HIMALAYA_DIR}        # himalaya CLI
  - ${SAG_DIR}             # sag TTS
  - ${PYTHON_SCRIPTS_DIR}  # pip 安装的脚本
  - ${LOCAL_BIN_DIR}       # npm global 脚本
```

### 验证安装

```bash
jq --version
gh auth status
python -m whisper --help
```

---

## 🔑 环境变量

> ⚙️ 将以下变量写入 `${WORKSPACE}/.env`（不提交到 Git）

```bash
# 邮箱
EMAIL_SMTP_HOST=smtp.example.com
EMAIL_SMTP_PORT=587
EMAIL_USER=your_email@example.com
EMAIL_PASSWORD=your_app_password

# GitHub
GH_TOKEN=ghp_xxxxxxxxxxxx

# 其他 API Keys
FIRECRAWL_API_KEY=fc-xxxxxxxx
```

> ⚠️ **安全规则**：.env 禁止提交！已加入 .gitignore

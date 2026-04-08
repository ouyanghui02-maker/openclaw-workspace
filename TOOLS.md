# TOOLS.md - Local Notes

Skills define _how_ tools work. This file is for _your_ specifics — the stuff that's unique to your setup.

## What Goes Here

Things like:

- Camera names and locations
- SSH hosts and aliases
- Preferred voices for TTS
- Speaker/room names
- Device nicknames
- Anything environment-specific

## Examples

```markdown
### Cameras

- living-room → Main area, 180° wide angle
- front-door → Entrance, motion-triggered

### SSH

- home-server → 192.168.1.100, user: admin

### TTS

- Preferred voice: "Nova" (warm, slightly British)
- Default speaker: Kitchen HomePod
```

## Why Separate?

Skills are shared. Your setup is yours. Keeping them apart means you can update skills without losing your notes, and share skills without leaking your infrastructure.

---

## 📧 邮箱配置（模板）

```markdown
### Email
- **Provider**: QQ Mail / Gmail / Outlook
- **IMAP**: imap.example.com:993
- **SMTP**: smtp.example.com:587
- **Config**: ${ENV_FILE_PATH}
```

## 🛠️ CLI 工具参考

常用工具及安装方式：

| 工具 | 用途 | 安装方式 |
|------|------|----------|
| jq | JSON 处理 | winget / brew |
| ripgrep | 快速搜索 | winget / brew |
| ffmpeg | 音视频处理 | winget / brew |
| gh | GitHub CLI | winget / brew |
| uv | Python 包管理 | npm |
| skillhub | Skill 管理 | npm |
| clawhub | Skill 发布 | npm |
| himalaya | 终端邮件 | GitHub Release |
| whisper | 语音转文字 | pip |

Add whatever helps you do your job. This is your cheat sheet.

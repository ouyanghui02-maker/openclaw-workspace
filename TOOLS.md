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

## 📧 邮箱配置

- **QQ 邮箱**: `2036673339@qq.com`
- **IMAP/SMTP 已配置**（SMTP 发件正常，IMAP 收件需网络支持）
- **配置文件**: `C:\Users\ouyan\.qclaw\.env`
- **skill 目录**: `C:\Users\ouyan\.qclaw\email-skill`
- **发件测试**: `node C:\Users\ouyan\.qclaw\email-skill\smtp-test.js`
- **收件命令**: `node C:\Users\ouyan\.qclaw\email-skill\imap.js check --limit 10`

## ⚠️ 已知问题

- IMAP 连接（imap.qq.com:993）有时超时，可能是网络封锁

## 🛠️ 已安装 CLI 工具

| 工具 | 版本 | 来源 | 路径 |
|------|------|------|------|
| jq | 1.8.1 | winget | WinGet\jqlang.jq |
| ripgrep | 15.1.0 | winget | WinGet\ripgrep |
| ffmpeg | 8.1 | winget | WinGet\Gyan.FFmpeg |
| gh | 2.88.1 | winget | C:\Program Files\GitHub CLI |
| uv | 0.11.1 | npm | C:\Users\ouyan\.local\bin |
| mcporter | ✅ | npm | npm global |
| oracle | ✅ | npm | npm global |
| clawhub | ✅ | npm | npm global |
| obsidian-cli | ✅ | npm | npm global |
| whisper | ✅ | pip | Python312 |
| himalaya | v1.2.0 | GitHub | C:\Users\ouyan\AppData\Local\Programs\Himalaya |
| sag | 0.2.2 | GitHub | C:\Users\ouyan\AppData\Local\Programs\sag |

**PATH 已更新到用户环境变量，包含：**
- C:\Users\ouyan\AppData\Local\Programs\Himalaya
- C:\Users\ouyan\AppData\Local\Programs\sag
- C:\Users\ouyan\AppData\Local\Programs\Python\Python312\Scripts
- C:\Users\ouyan\.local\bin

Add whatever helps you do your job. This is your cheat sheet.

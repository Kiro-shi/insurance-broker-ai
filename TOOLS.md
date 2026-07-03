# TOOLS.md — KK 的本地环境

## 硬件
- **Mac mini** — Apple Silicon (arm64)，macOS，24×7 运行 OpenClaw Gateway
- 无外接摄像头/音箱等外设配置

## Shell & 包管理
- **Shell:** zsh
- **Homebrew:** 6.0.6（/opt/homebrew）
- **Node.js:** v24.16.0（~/.local/opt/node-v24.16.0-darwin-arm64/bin）
- **Python:** 3.9.6（系统自带）

## CLI 工具
- **GitHub CLI (gh):** 已登录，账号 Kiro-shi
- **Claude Code:** @anthropic-ai/claude-code（全局安装，未使用）

## 搜索工具策略
- **默认优先：Tavily** — 做常规网页搜索、新闻检索、资料查找、URL 内容抽取时，优先使用 Tavily 驱动的 `web_search`/`web_fetch` 或 Tavily 插件能力。
- **补充方案：multi-search-engine** — 当 Tavily 结果不够、需要更多知识面/交叉验证、需要中文搜索源（百度、搜狗、微信、360、神马等）或特定搜索引擎语法时，用 `multi-search-engine` Skill 作为备选和补充。
- **隐私边界** — 不把密钥、客户信息、内部项目名、敏感个人信息放进公开搜索引擎查询；这类查询先本地或授权数据源查。

## 飞书
- Bot 名称：Little KK
- 权限：docx:document、drive:drive、wiki:wiki
- 群策略：open（任何有 bot 的群都能 @）

## 其他
- 无 SSH 别名
- 无 TTS 配置

# MEMORY.md — 小KK的长期记忆

## KK
- 名字：KK
- 时区：Asia/Shanghai (UTC+8)
- 位置：上海
- 设备：Mac mini（Apple Silicon M 系列，本地 hosting）

## KK的偏好与风格
- 沟通：简洁、直接，不要废话
- 兴趣：全球财经、科技趋势、加密货币
- 决策：先给方案让他选，别替他决定
- 节奏：非紧急事务等他说，不主动打扰
- 配置：喜欢干净，没用的东西不占着
- 搜索：优先用 Tavily；需要更广知识面、中文搜索源或交叉验证时，用 multi-search-engine Skill 补充。

## 重要配置决策
- 2026-06-16：飞书 Bot "Little KK" 上线，配对成功
- 2026-06-16：Mac mini 设成不休眠 24x7
- 2026-06-16：心跳设为 1 小时，用 Flash 模型省钱
- 2026-06-16：心跳配全球财经新闻巡检任务
- 2026-06-24：IDENTITY.md + SOUL.md 个性化初版
- 2026-06-24：周报 cron job 重建（旧版连续失败，新版简化配置）
- 2026-07-02：Homebrew 安装（KK 手动安装，6.0.6）
- 2026-07-02：大扫除 — 删 canvas 插件、清理备份文件、清理 memory 冗余
- 2026-07-02：搜索工具策略定为 Tavily 优先，multi-search-engine 作为知识面扩展和备选补充。

## 当前系统状态（2026-07-02 大扫除后）
- 模型：deepseek/deepseek-v4-pro（心跳用 flash）
- 已激活插件：browser-automation、feishu-doc/drive/perm/wiki
- 全局工具：Homebrew、GitHub CLI（Kiro-shi）、Node.js v24、Python 3.9
- 周报 cron：每周一 9AM，6/24 首次手动跑成功，6/30 定时跑超时失败，待验证
- 已知问题：256 个孤儿 transcript（~105MB）、Memory Search 索引需重建

## 经验教训
- 2026-07-04：说"不能读飞书表格"是错的——应该先 `openclaw skills search` 搜 ClawHub 有没有插件再下结论。feishu-sheet 插件装了就能用。同理适用于任何能力边界问题。

## 当前系统状态（2026-07-04 更新）
- 新增插件：feishu-sheet（飞书表格读写）
- 新增 skill：insurance-broker（保险经纪人AI，含Q&A知识库）
- 新增工具：cloudflared（Cloudflare Tunnel，用于公网访问）
- 新增工具：openpyxl（Python Excel 读取）
- 活跃项目：保险经纪人AI应用（GitHub: Kiro-shi/insurance-broker-ai）

## 已完成
- 2026-06-16：飞书权限补全、GitHub CLI 安装登录、上下文管理部署、Task Management Protocol
- 2026-06-24：SOUL.md + IDENTITY.md 去模板化
- 2026-07-02：配置大扫除（删 canvas 插件、清理 openclaw.json 备份、合并冗余 memory 文件）
- 2026-07-03：保险经纪人AI MVP 跑通（data schema + skill + 1款产品 + 模拟客户 + GitHub 备份 + WebChat 公网方案验证）

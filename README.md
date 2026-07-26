# 独立游戏开发者技能库

> AI Agent Skills for Indie Game Developers —— 覆盖创意→设计→原型→美术→编程→发布全流程

## 定位

为独立游戏开发者（特别是单人/小团队）提供一套可安装的 AI Agent 技能，让 Claude Code / OpenClaw 等 AI 编程助手成为你的游戏开发搭档。

## 核心理念

> 用 AI 撬动创意，用技能加速交付，一人公司也能做完游戏。

- **每个技能聚焦一个环节**——不贪大求全，单个技能做到可落地
- **2 周可出 MVP**——技能设计匹配快节奏独立开发周期
- **一次交付，持续销售**——面向 Steam / itch.io / App Store 等买断制平台

## 技能清单

| 环节 | 技能 | 描述 | 来源 |
|------|------|------|------|
| 💡 创意 | `game-designer` | 一句话点子 → 完整游戏设计方案 | 原创 |
| 📝 设计 | `gdd-generator` | 生成专业游戏设计文档（GDD） | 原创 |
| 🏗️ 原型 | `web-game-prototype` | Three.js 3D 浏览器游戏快速原型 | 原创 |
| 🎨 美术 | `pixel-art-studio` | AI 像素艺术素材生成管线 | 原创 |
| 🎵 音乐 | `game-music-generator` | 游戏背景音乐和音效生成 | 原创 |
| 🔧 编程 | `game-developer` | Unity/Unreal/Godot 编程指导 | 原创 |
| 🤖 AI | `game-ai-systems` | 游戏 AI 行为设计（FSM/BT/GOAP） | 原创 |
| 🧪 测试 | `game-tester` | 自动化游戏测试循环 | 原创 |
| 📦 发布 | `steam-launch` | Steam 上架就绪检查清单 | 原创 |
| 📊 运营 | `indie-hacker-strategy` | 独立黑客营销与增长策略 | 原创 |

## 快速开始

### 1. 安装技能

```bash
# 安装全部技能
npx skills add skills-repo/indie-game-developer@<skill-name> -g -y

# 最小安装集（6 个核心技能）
npx skills add skills-repo/indie-game-developer@game-designer -g -y
npx skills add skills-repo/indie-game-developer@web-game-prototype -g -y
npx skills add skills-repo/indie-game-developer@pixel-art-studio -g -y
npx skills add skills-repo/indie-game-developer@game-music-generator -g -y
npx skills add skills-repo/indie-game-developer@game-developer -g -y
npx skills add skills-repo/indie-game-developer@steam-launch -g -y
```

### 2. 使用技能

安装后，在 Claude Code 或 OpenClaw 中使用 `/skill-name` 调用对应技能。

### 3. 推荐工作流

```
创意 → 设计 → 原型 → 美术+音乐 → 编程+AI → 测试 → 发布 → 运营
game-  gdd-    web-    pixel-art  game-    game-  steam-  indie-
designer gen   game-   studio     devel-   tester launch  hacker-
               proto   game-      oper             strategy
               type    music-     
                       generator   
```

## 适用平台

| 平台 | 推荐技能组合 |
|------|-------------|
| **Steam** | game-designer + gdd-generator + game-developer + steam-launch |
| **itch.io** | game-designer + web-game-prototype + pixel-art-studio |
| **App Store (iOS)** | game-designer + ios-developer + app-store-submit |
| **微信小游戏** | game-designer + web-game-prototype + douyin-mini-game |

## 贡献

欢迎提交 PR 贡献新的技能或改进现有技能。

每个技能放在 `skills/<skill-name>/` 目录下，包含：
- `SKILL.md` — 技能定义文件
- 相关资源和参考文件

## 许可

MIT

## 相关资源

- [Claude Code Skills](https://docs.anthropic.com/en/docs/claude-code/skills)
- [skills.sh](https://skills.sh) — 技能市场
- [ClawHub](https://clawhub.ai) — AI 技能平台

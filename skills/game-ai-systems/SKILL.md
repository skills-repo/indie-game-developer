---
name: game-ai-systems
description: 游戏中 NPC/敌人的 AI 行为设计与实现（FSM/行为树/GOAP）
source:
  type: original
  repo: skills-repo/indie-game-developer
  path: skills/game-ai-systems/SKILL.md
  version: 1.0.0
  updated: 2026-07-26
metadata:
  category: AI
  platform: Unity,Godot
  difficulty: 进阶
---

# 游戏 AI 系统

> 让游戏里的敌人不再傻站，NPC 的行为不再出戏。

## 能力

- **AI 架构选择**：帮你判断用 FSM、行为树、效用系统还是 GOAP
- **FSM（有限状态机）**：简单敌人巡逻/追击/攻击/死亡、Boss 阶段切换
- **行为树（BT）**：复杂 NPC 日常行为、战术 AI 决策
- **效用系统（Utility AI）**：模拟人生类、多目标优化
- **GOAP（目标导向行动规划）**：智能敌人自主规划行为
- **A* 寻路**：完整实现和优化（Jump Point Search 等变体）
- **代码示例**：C# / GDScript 完整可运行示例

## 使用方式

```
/game-ai-systems "我的潜入游戏中，守卫需要巡逻→发现可疑→调查→警报→追击→失去目标→返回巡逻。用哪种 AI 架构最合适？"
```

## 工作流

1. 描述 NPC/敌人的行为需求（状态有哪些、触发条件是什么）
2. AI 推荐最合适的架构并提供理由
3. 给出代码骨架和关键逻辑
4. 集成并调参

## 架构选择指南

| 复杂度 | 行为数量 | 推荐架构 | 示例 |
|--------|---------|---------|------|
| 低 | <5 | FSM | 炮台：待机→激活→射击 |
| 中 | 5-15 | 行为树 | 守卫：巡逻/调查/追击/警报 |
| 高 | 15+ | 效用系统 | 模拟人生 NPC |
| 极高 | 动态 | GOAP | 策略游戏 AI 对手 |

## 适用场景

- 单机游戏中需要敌人 AI
- NPC 需要可信的日常行为
- Boss 战需要分阶段 AI

## 限制

- 不涉及机器学习/强化学习 AI
- 不做联网游戏的服务器端 AI
- 不做寻路图生成（NavMesh 烘焙是引擎功能）

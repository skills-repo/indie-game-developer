---
name: pixel-art-studio
description: 像素艺术游戏构建：16x16 精灵生成、12 色调色板、放置/增量游戏机制
source:
  type: derived
  repo: skills-repo/indie-game-developer
  path: skills/pixel-art-studio/SKILL.md
  version: 1.0.0
  updated: 2026-07-26
  url: https://skills.sh/cooksaw/claude-skills/pixel-art-game-builder
metadata:
  category: 游戏美术
  platform: Web
  difficulty: 入门
---

# 像素艺术工坊

> 像素艺术放置/增量游戏构建：Canvas API 程序化精灵生成、React/Zustand 架构、冥想式游戏设计。

## 能力

- **像素精灵生成**：16×16 精灵的程序化生成，4 色/精灵，12 色调色板
- **放置游戏机制**：自动生产、升级系统、收藏机制
- **游戏经济设计**：平衡曲线、稀有度系统、升级路径
- **视觉风格**：暗色背景、发光效果、缓慢有机动画
- **技术实现**：React + TypeScript + Zustand + Canvas API

## 使用方式

```
/pixel-art-studio 创建一个像素风放置游戏
/pixel-art-studio 为这个游戏生成像素精灵
/pixel-art-studio 设计一个收藏系统的稀有度体系
```

## 工作流

1. 设计游戏概念和核心循环
2. 搭建 React + Vite + Zustand 项目
3. 实现 Canvas 像素精灵生成器
4. 构建放置/增量游戏机制
5. 迭代视觉和平衡

## 适用场景

- 像素风放置游戏（Idle/Incremental）
- 收藏类游戏（Collection-based）
- 冥想式/休闲游戏
- 像素精灵资源生成

## 限制

- 仅覆盖像素风（16×16），不涉及其它美术风格
- 不涉及 3D 渲染
- 不涉及多人联机
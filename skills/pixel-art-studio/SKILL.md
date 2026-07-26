---
name: pixel-art-studio
description: AI 像素艺术素材生成管线，支持角色、瓦片、动画全流程
source:
  type: original
  repo: skills-repo/indie-game-developer
  path: skills/pixel-art-studio/SKILL.md
  version: 1.0.0
  updated: 2026-07-26
metadata:
  category: 美术
  platform: 通用
  difficulty: 入门
---

# 像素艺术工作室

> 不会画画？没关系，AI 替你把像素素材一条龙搞定。

## 能力

- **角色生成**：多姿态角色表（正面/侧面/行走/攻击/死亡），保持跨帧一致性
- **环境瓦片**：地面、墙壁、植被、道具瓦片集，支持无缝拼接
- **精灵动画**：单张角色图 → AI 生成 16 帧像素动画（idle / walk / jump / attack）
- **场景概念**：关卡氛围图、视差背景层
- **AI 管线**：AI 生图 → 去背景 → 像素化 → 切帧 → 合并 Sprite Sheet

## 使用方式

```
/pixel-art-studio "为我的平台跳跃游戏生成主角角色表：一个戴帽子的像素猫，16x16 风格，需要 idle/walk/jump/fall 四组动画帧"
```

## 工作流

1. 描述角色/场景需求（风格、尺寸、动画需求）
2. AI 生成初始素材
3. 审查一致性（角色在不同帧中的特征是否保持）
4. 按需调整（颜色调色板、像素密度、动画速度）
5. 导出为 PNG Sprite Sheet，直接导入引擎

## 推荐风格

- 16x16 / 32x32 像素艺术（最友好、最易保持一致性）
- 推荐引擎：Godot（有原生像素支持）> Unity > 其他

## 适用场景

- 独立游戏开发者无美术背景
- 原型阶段需要快速出素材
- 像素风游戏的资产生产管线

## 限制

- AI 生成的角色跨帧一致性不如手绘——需要人工审查
- 不适合高分辨率/写实风格
- 不生成 3D 模型（那是另一个技能的事）
- 像素艺术风格最稳健，其他风格一致性会更差

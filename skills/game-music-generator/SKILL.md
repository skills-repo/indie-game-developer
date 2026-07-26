---
name: game-music-generator
description: 为游戏生成背景音乐和音效，支持多风格、多 Provider
source:
  type: original
  repo: skills-repo/indie-game-developer
  path: skills/game-music-generator/SKILL.md
  version: 1.0.0
  updated: 2026-07-26
metadata:
  category: 音乐
  platform: 通用
  difficulty: 入门
---

# 游戏音乐生成器

> 没有作曲预算？AI 给你的游戏配上不违和的 BGM 和音效。

## 能力

- **背景音乐生成**：按场景风格生成完整 BGM（菜单/战斗/探索/Boss/胜利/失败）
- **音效生成**：UI 点击、攻击命中、拾取道具、环境音效
- **多 Provider 支持**：Suno、Udio、Stable Audio、MusicGen、Mubert、Soundraw、Riffusion
- **风格提示词技巧**：风格 → 情绪 → 乐器 → BPM → 参考艺术家
- **授权指南**：个人使用 vs 商业使用的授权边界说明

## 使用方式

```
/game-music-generator "为我的像素风地牢探索游戏生成一首背景音乐：阴暗氛围、慢节奏、管风琴+低音弦乐、60BPM"
```

## 工作流

1. 列出游戏需要的所有音乐/音效清单
2. 按场景逐个描述风格需求
3. AI 根据描述推荐 Provider 和生成参数
4. 生成并试听
5. 满意后导出音频文件（WAV/MP3）

## 清单模板

```
菜单BGM：  _______（风格/情绪/乐器/BPM）
关卡1BGM： _______ 
Boss战BGM：_______
胜利音效： _______
失败音效： _______
UI 音效：  _______（点击/hover/确认/取消）
战斗音效： _______（攻击/受击/技能/暴击）
环境音效： _______（风/雨/脚步/门）
```

## 适用场景

- 独立游戏需要配乐但请不起作曲
- Game Jam 快速出片
- 原型阶段需要氛围参考

## 限制

- AI 生成的音乐不能用于需要版权独占的平台
- 商业使用前检查 Provider 的授权条款
- 不保证艺术水准——是"够用"不是"惊艳"
- 不提供定制化编曲（需要反复试）

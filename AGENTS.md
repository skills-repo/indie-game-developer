# AGENTS.md

## 仓库性质

这是一个 **AI Agent 技能库**，不是软件项目。所有内容为 Markdown 格式的技能定义文件。

## 目录约定

```
indie-game-developer/
├── README.md              # 项目介绍和使用指南
├── AGENTS.md              # AI 助手使用指引（本文件）
└── skills/                # 技能目录
    ├── <skill-name>/      # 单个技能目录
    │   └── SKILL.md       # 技能定义文件
    └── ...
```

## SKILL.md 格式

每个技能文件遵循以下结构：

```markdown
---
name: <skill-name>
description: <一句话描述，显示在技能列表中>
metadata:
  category: <创意|设计|原型|美术|音乐|编程|AI|测试|发布|运营>
  platform: <Steam|itch.io|iOS|Web|通用>
  difficulty: <入门|进阶|专家>
---

# <技能名称>

> <一句话简介>

## 能力

- 能力点 1
- 能力点 2

## 使用方式

在 Claude Code / OpenClaw 中使用 `/skill-name` 调用。

## 工作流

1. 步骤 1
2. 步骤 2

## 适用场景

- 场景 A
- 场景 B

## 限制

- 不擅长的领域
```

## 工作约定

- 所有技能内容使用中文编写
- 技能聚焦单一环节，不贪大求全
- 每个技能需明确"能做什么"和"不能做什么"
- 优先覆盖独立开发者（单人/小团队）场景
- 面向 Steam / itch.io / App Store 等买断制平台

## 技能添加流程

1. 在 `skills/` 下创建以技能名命名的目录
2. 编写 `SKILL.md`
3. 确保 `metadata` 字段完整
4. 更新 `README.md` 中的技能清单表

## 不做什么

- 不创建需要服务器/账号体系的产品技能
- 不创建面向大团队协作的技能
- 不创建免费+IAP/广告变现模式的技能（专注买断制）

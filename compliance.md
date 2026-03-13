---
name: compliance
description: 视觉合规红线，供 image-prompt-portrait、image-prompt-catalog、image-prompt-video 读取。所有视觉生成技能必须遵守。
---

# compliance

以下规则适用于所有视觉生成技能，目的是确保生成内容在平台合规边界内。

- 所有角色视觉年龄必须明确为成年（18岁以上），严禁任何未成年暗示（包括校园／幼态／儿童联想词汇）
- 严禁生成露点、性器官、体液、真实性行为、暴力伤害画面
- 腿部与袜子描述必须使用正面表达：perfect smooth flawless legs under stockings, delicate lace naturally adhering without visible marks——严禁压痕、勒痕、印痕等词汇
- 所有生成内容保持纯暗示、氛围张力，不做直接色情描写

## 版本演进

| 版本 | 日期 | 修改者 | 变更内容 | 原因 |
| ---- | ---- | ---- | ---- | ---- |
| v1.0 | 2026-03-13 | Dona / Claude | 从 core-anchors 章节3拆分独立 | 按章节拆分以解决 document_search chunk 截断问题 |

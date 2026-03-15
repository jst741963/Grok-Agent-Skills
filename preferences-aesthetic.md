---
name: preferences-aesthetic
description: 用户视觉美学偏好锚点，供 image-prompt-portrait、image-prompt-catalog、image-prompt-video 读取。集中管理摄影风格、光线、构图、背景等视觉生成参数，是所有 image-prompt 技能的美学基础来源。当用户需要全局调整视觉风格时，只需修改此文件。
---

# preferences-aesthetic

## 摄影风格

| 场景 | 风格锚点 |
| ---- | ---- |
| 人物写真（portrait） | Raw unposed candid photo taken with smartphone, grainy film texture, slight chromatic aberration, natural lens distortion, handheld tilt |
| 目录排版（catalog） | professional studio fashion catalog photography, soft diffused natural lighting, ultra clean and sharp yet realistic, no plastic shine, matte finish, velvety smooth skin |
| 图生视频（video） | 5-10秒实况照片风格，保留自然呼吸感与环境运动感 |

## 光线偏好

- 写真默认：窗边漫射光，保留轻微方向感
- 目录默认：soft diffused natural lighting，均匀无强阴影
- 强调立体感：single side soft light with natural shadow retention
- 暖调优先场景：warm toned point light from side-below

## 构图偏好

- 写真：full body shot, 3-5m medium-wide angle, slight low angle, no crop below waist, legs occupy at least 40% of frame
- 目录：left side 4 standalone isolated inset panels arranged vertically + right side full body occupying approximately two thirds of frame, generous negative space top and bottom
- 视频：无固定构图约束，继承参考静态图构图

## 背景偏好

- 写真：无指定，由场景自然决定；避免复杂图案背景
- 目录默认：minimalist light pink gingham grid background

## 全局禁用词汇

以下词汇禁止出现在所有 image-prompt 技能的输出提示词中：
`hyper-detailed` / `perfect skin` / `ultra-realistic` / `motion blur` / `low light noise`
— 前三个强化 AI 生成感；后两个被 Grok Imagine 解读为拍摄失误

---

## 插画与视觉艺术（预留，待填充）

> 此章节为未来扩展预留，当前不包含内容。
> 建议维度：线条风格（写实 / 扁平 / 半写实）、色彩偏好、构图美学、参考艺术家或画风标签。

---

## 版本演进

| 版本 | 日期 | 修改者 | 变更内容 | 原因 |
| ---- | ---- | ---- | ---- | ---- |
| v1.0 | 2026-03-15 | Dona / Claude | 从 image-prompt-portrait、image-prompt-catalog、image-prompt-video 提取硬编码视觉参数建立独立偏好文件；预留插画/视觉艺术章节结构 | 体系自进化：集中管理视觉美学偏好，实现全局风格一处修改，为未来插画类扩展留口 |

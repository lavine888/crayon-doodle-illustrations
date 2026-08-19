<div align="center">

# Crayon Doodle Illustrations

**把“抽象观点”，画成能看懂、能记住、能传播的彩铅知识卡。**

中文内容 → 认知锚点 → 物理隐喻 → 3:4 / 4:5 手绘轮播

![Codex Skill](https://img.shields.io/badge/Codex-Skill-111111?style=flat-square)
![Chinese First](https://img.shields.io/badge/Chinese-First-D95B32?style=flat-square)
![MIT License](https://img.shields.io/badge/License-MIT-2E63A8?style=flat-square)

</div>

---

## 先看效果

这不是 5 张随机风格图，而是一组由同一个 Skill 生成的完整叙事：

**Prompt 只是入口 → Prompt ≠ 结果 → 判断更稀缺 → 工作流让结果稳定 → 判断 × 工作流**

<p align="center">
  <img src="https://github.com/user-attachments/assets/9424b2b7-c458-4d5d-b9f9-e8c2f94c8c7c" width="29%" alt="Prompt 只是入口">
  <img src="https://github.com/user-attachments/assets/a641b853-08c5-4ff9-b362-8ff5a7faf2cf" width="29%" alt="Prompt 不等于结果">
  <img src="https://github.com/user-attachments/assets/3b8e8084-6156-4b6c-9fac-bbd852aea682" width="29%" alt="真正稀缺的是判断">
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/3a80d59d-1141-4053-8880-4f22891790b0" width="29%" alt="工作流把偶然变稳定">
  <img src="https://github.com/user-attachments/assets/fd88a997-22b8-4eec-8b68-9cb03d5d16bd" width="29%" alt="判断乘以工作流">
</p>

> 目标不是“画得像彩铅”，而是让一套内容从**判断、文案、隐喻到视觉**都保持同一种语言。

---

## 这个 Skill 到底做什么？

很多图像模型会画“手绘”，但结果经常漂成儿童绘本、商业扁平插画、PPT 信息图，或者一张很好看但没有观点的装饰图。

**Crayon Doodle Illustrations** 做的不是给 prompt 加一句 `crayon style`，而是把内容生产拆成一条可重复的流程：

```text
原始文章 / 观点
      ↓
找出真正值得画的认知锚点
      ↓
压缩成一页能读懂的短文案
      ↓
把抽象关系翻译成一个物理隐喻
      ↓
生成统一的彩铅知识卡
      ↓
QA：文字 / 构图 / 质感 / 系列一致性
```

所以它更像一个**视觉内容 Agent 的工作方法**，而不是一条生图 prompt。

---

## 30 秒开始用

### 1. 安装

```bash
git clone https://github.com/lavine888/crayon-doodle-illustrations.git
cd crayon-doodle-illustrations

mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
cp -R ./crayon-doodle-illustrations "${CODEX_HOME:-$HOME/.codex}/skills/"
```

### 2. 直接丢一篇文章

```text
Use $crayon-doodle-illustrations 把下面这篇文章做成 7 页彩铅涂鸦风小红书轮播。

<粘贴文章>
```

Skill 会自己完成：**拆观点 → 写单页文案 → 发明隐喻 → 设计轮播 → 生成图片 → QA。**

---

## 它为什么比“直接让 AI 画一张图”稳定？

| 普通生图 | Crayon Doodle Illustrations |
|---|---|
| 先想画面 | 先判断这页到底想说什么 |
| 把文字塞进图里 | 先把长文压成单页判断 |
| 抽象概念直接画图标 | 先翻译成真实物理动作 |
| 每张图各画各的 | 先定义整组视觉系统 |
| 生成完就交付 | 生成后跑 QA / benchmark |

核心原则只有一句：

> **插画不是装饰，它是观点的第二种表达语言。**

---

## 视觉 DNA

| 维度 | 默认规则 |
|---|---|
| **Paper** | 暖米白 / 象牙色纸张，不做纯白 UI |
| **Palette** | 橙红 + 钴蓝为主，石墨灰辅助 |
| **Material** | 明显彩铅 / 蜡笔 / 木颜色铅笔颗粒 |
| **Typography** | 中文手写感，允许轻微歪斜和笔触毛边 |
| **Layout** | 上半区短文案，下半区一个完整视觉隐喻 |
| **Metaphor** | 桥、河、水管、旧机器、箱子、工具、轨道等低科技物件 |
| **Character** | 人物比例自然、动作明确，不做 Q 版 mascot |
| **Density** | 大量留白，一页只讲一个核心认知动作 |

### 明确不要

`PPT 信息图` · `正式流程图` · `复杂架构图` · `科技 Dashboard` · `3D 渲染` · `商业扁平插画` · `儿童绘本` · `密集文字海报`

---

## 最适合拿来画什么？

特别适合那些“文字讲得清楚，但普通配图很难画”的内容：

- AI / Agent / 产品 / 创业 / 商业
- 反常识观点与概念拆解
- 职业选择与方法论
- 用户研究与产品验证
- 收入模型与商业机制
- Build in Public / 开源产品复盘
- 小红书 5–9 页轮播
- 公众号、博客、Notion 正文插图

不推荐拿它做严格统计图、复杂技术拓扑、真实产品 UI、高端摄影 KV，或者精确复刻某个既有 IP。

---

## 常用调用方式

### 一篇文章 → 一组轮播

```text
Use $crayon-doodle-illustrations 把下面文章做成 7 页轮播。
每页只保留一个核心判断，并为每页重新发明一个视觉隐喻。
保持整组纸张、色板、笔触和人物语言一致。

<文章>
```

### 一个观点 → 一张知识卡

```text
Use $crayon-doodle-illustrations 为这个观点生成一张 3:4 中文知识卡：

“产品能跑，不等于产品能卖。”

不要直接画漏斗或人民币符号，先把它翻译成一个具体物理隐喻。
```

### 只规划，不生图

```text
Use $crayon-doodle-illustrations 先不要生成图片。
把下面内容拆成 6 页，并为每页输出：
核心判断 / 主标题 / 短解释 / 强调句 / 视觉隐喻 / 人物动作 / 构图。

<内容>
```

更多场景见 [`examples/prompts.md`](examples/prompts.md)。

---

## 一页知识卡是怎么被设计出来的？

默认只保留四层信息：

1. **主标题**：1–3 行，先把判断说出来；
2. **短解释**：2–6 行，只补最必要的因果；
3. **强调句**：可选，用橙红色制造停顿；
4. **视觉隐喻**：不用图标解释，而是用一个具体场景让人“秒懂”。

例如：

> 不是能收费，而是能持续收钱。

不画一个普通人民币符号。

可以画成：**一边是短暂暴雨砸进桶里，另一边是稳定水流汇成河。**

`暴雨 = 一次爆单`，`河流 = 可重复收入`。

这就是这个 Skill 最核心的能力：**把抽象关系变成能被画出来的物理动作。**

---

## Skill 里面有什么？

真正决定输出稳定性的东西都在 [`crayon-doodle-illustrations/references/`](crayon-doodle-illustrations/references/)：

| 文件 | 负责什么 |
|---|---|
| `style-dna.md` | 纸张、材质、色板、线条 |
| `layout-system.md` | 封面 / 正文 / 图文比例与留白 |
| `copywriting-system.md` | 把长文压缩成单页手写文案 |
| `visual-metaphors.md` | 从抽象观点发明原创物理隐喻 |
| `character-language.md` | 人物比例、动作和系列角色语言 |
| `carousel-sequencing.md` | 5–9 页轮播如何有推进感 |
| `prompt-template.md` | 单页 / 封面 / 系列生图模板 |
| `editing-recipes.md` | 太 PPT、文字错、画面挤等修图方法 |
| `qa-checklist.md` | 生成后的必过检查 |
| `benchmark-rubric.md` | 20 分制质量 benchmark |

如果只想使用 Skill，直接安装子目录 `crayon-doodle-illustrations/` 即可。

---

## 设计原则

这个项目只抽取一种“手绘讲义式知识卡”的**通用视觉语法**：纸张、笔触、色板、信息密度、版式与隐喻方法。

它不要求复制任何特定参考图中的人物、文案、构图或物件。

**借语法，不抄句子；借材质，不抄构图。**

---

## About

Made by [Lavine](https://github.com/lavine888) for people who want AI-generated content to have a little more **judgment, texture and personality**.

MIT License · See [`LICENSE`](LICENSE) and [`NOTICE.md`](NOTICE.md).

# Crayon Doodle Illustrations

> 把中文文章里的判断、方法和抽象概念，变成一张张暖米白纸上的「手写讲义 + 彩铅隐喻画」。
>
> 3:4 / 4:5 竖版 | 红橙蓝手写字 | 彩铅 / 蜡笔颗粒 | 中文知识卡 | Codex Skill

---

## 这个仓库是什么

Crayon Doodle Illustrations 是一个面向 Codex / AI Agent 的中文配图 Skill。

它不是普通的“给文章配一张插画”，而是把一篇文章先拆成若干个**单页判断**，再为每个判断设计一个具体、好懂、带一点奇思妙想的视觉隐喻，生成适合小红书轮播、公众号正文、知识型社交内容的竖版图文卡片。

一句话：**像一个很会讲东西的人，拿红蓝彩铅在一本创意笔记上边讲边画。**

---

## 视觉 DNA

默认风格：

- 暖米白 / 象牙色纸张背景，而不是纯白 UI
- 明显的彩铅、蜡笔、木颜色铅笔颗粒
- 橙红 + 钴蓝为主，石墨灰作为辅助
- 中文手写标题，允许轻微歪斜、粗细不均和笔触毛边
- 页面上半部是短标题与解释，下半部是一个完整视觉隐喻
- 构图清爽，留白大，但不是极简矢量风
- 物件带一点机械、创客、学生手账、科普草图气质
- 可以有重复出现的“创客观察者”角色，但不依赖固定 IP
- 一页只讲一个核心认知动作

禁止：PPT 信息图、商业扁平插画、3D 渲染、科技 UI、过度精致矢量、密集长文、平台截图 UI。

---

## 适合什么内容

特别适合：

- AI / 产品 / 创业 / 商业 / 职业方法论
- 反常识观点与认知拆解
- 流程、对比、因果、行动建议
- 小红书 5-9 页轮播
- 公众号正文插图
- Build in Public / 产品复盘 / 知识型内容

不适合：

- 需要严格数据精度的图表
- 正式企业架构图
- 复杂技术拓扑
- 真实产品 UI 截图
- 高端商业 KV / 摄影海报

---

## 安装

```bash
git clone https://github.com/lavine888/crayon-doodle-illustrations.git
cd crayon-doodle-illustrations

mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
cp -R ./crayon-doodle-illustrations "${CODEX_HOME:-$HOME/.codex}/skills/"
```

安装后可直接：

```text
Use $crayon-doodle-illustrations 把下面这篇文章做成 7 页彩铅涂鸦风小红书轮播。

<粘贴文章>
```

---

## 用法

### 1. 先规划，不生图

```text
Use $crayon-doodle-illustrations 先不要生成图片。
请把下面文章拆成 7 页轮播，输出每一页的：核心判断、标题、短解释、强调句、视觉隐喻和构图。

<文章>
```

### 2. 直接生成整组轮播

```text
Use $crayon-doodle-illustrations 把下面文章做成 6 页竖版图文卡。
要求：3:4，暖米白纸张，橙红和钴蓝手写字，彩铅/蜡笔颗粒，上文下图，每页只讲一个观点。

<文章>
```

### 3. 单个概念做一张

```text
Use $crayon-doodle-illustrations 为“产品不等于销售”做一张竖版知识卡。
不要直接画漏斗，重新发明一个更具象的物理隐喻。
```

### 4. 做封面

```text
Use $crayon-doodle-illustrations 为这组轮播生成封面。
标题控制在两到三行，底部用一个强隐喻主体，视觉比正文页更集中。
```

更多示例见 `examples/prompts.md`。

---

## 工作流程

1. 读懂文章，不平均分段
2. 找出 5-9 个认知锚点
3. 每页压缩成一个单页判断
4. 给每页写短标题、短解释、强调句
5. 为每页重新发明一个视觉隐喻
6. 保持整组色板、纸张、字迹和版式一致
7. 每页单独生成，不拼九宫格
8. 按 QA checklist 检查文字、留白、质感和平台 UI 污染
9. 必要时重生成或局部编辑

---

## 目录结构

```text
.
├── README.md
├── examples/
│   └── prompts.md
└── crayon-doodle-illustrations/
    ├── SKILL.md
    ├── agents/
    │   └── openai.yaml
    └── references/
        ├── style-dna.md
        ├── layout-system.md
        ├── visual-metaphors.md
        ├── prompt-template.md
        └── qa-checklist.md
```

真正需要复制进 Codex Skills 目录的是 `crayon-doodle-illustrations/` 子目录。

---

## 设计原则

这个 Skill 的参考来自一种“手绘讲义式知识卡”的视觉语言：它只抽取**通用视觉语法**——纸张、笔触、色板、版式、信息密度、隐喻方法——不要求复制任何特定参考图中的人物、文案、构图或物件。

输出应该保持原创：**借语法，不抄句子；借材质，不抄构图。**

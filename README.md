# Crayon Doodle Illustrations

> 把中文文章里的判断、方法和抽象概念，变成一张张暖米白纸上的「手写讲义 + 彩铅隐喻画」。
>
> 3:4 / 4:5 竖版 | 橙红 + 钴蓝 | 彩铅 / 蜡笔颗粒 | 中文知识卡 | Codex Skill

---

## 这个仓库是什么

Crayon Doodle Illustrations 是一个面向 Codex / AI Agent 的中文配图 Skill，用来把文章、帖子、方法论、产品观点、创业经验和抽象概念，转译成一组有统一视觉语言的手绘知识卡。

它不是“给文章随便配张图”，也不是 PPT 信息图模板。

它的核心流程是：

1. 先理解文章真正的认知锚点；
2. 把每个锚点压缩成一句适合图上的判断；
3. 为这句话重新发明一个具体的物理隐喻；
4. 用暖米白纸、彩铅 / 蜡笔颗粒、橙红和钴蓝手写字，把它画成一页知识卡；
5. 再把 5-9 页串成一组有推进感的轮播。

一句话：**像一个很会讲东西的人，拿红蓝彩铅在一本创意笔记上边讲边画。**

---

## Showcase

下面预留 5 个高清原图位置。直接在 GitHub 编辑 README，把图片拖到对应位置即可。

### 01

<img width="1086" height="1448" alt="ChatGPT Image 2026年8月19日 16_22_07 (1)" src="https://github.com/user-attachments/assets/9424b2b7-c458-4d5d-b9f9-e8c2f94c8c7c" />


### 02

<img width="1086" height="1448" alt="ChatGPT Image 2026年8月19日 16_22_08 (2)" src="https://github.com/user-attachments/assets/a641b853-08c5-4ff9-b362-8ff5a7faf2cf" />

### 03


<img width="1086" height="1448" alt="ChatGPT Image 2026年8月19日 16_22_09 (3)" src="https://github.com/user-attachments/assets/3b8e8084-6156-4b6c-9fac-bbd852aea682" />

### 04


<img width="1086" height="1448" alt="ChatGPT Image 2026年8月19日 16_22_09 (4)" src="https://github.com/user-attachments/assets/3a80d59d-1141-4053-8880-4f22891790b0" />


### 05

<img width="1086" height="1448" alt="ChatGPT Image 2026年8月19日 16_22_10 (5)" src="https://github.com/user-attachments/assets/fd88a997-22b8-4eec-8b68-9cb03d5d16bd" />
---

## 为什么单独做一个 Skill

很多图像模型能画“手绘”，但很容易漂成四种东西：

- 儿童绘本
- 商业扁平插画
- PPT 信息图
- 精致但没有观点的装饰图

这个 Skill 不是只加一句 `crayon style`，而是把视觉系统拆成：

- 纸张和材质
- 色板和手写层级
- 单页文案压缩
- 视觉隐喻生成
- 人物动作语言
- 轮播叙事
- 生图提示词
- 编辑配方
- QA checklist
- benchmark 评分

这样 Agent 才不只是“模仿一个画风”，而是学会**怎样用这套画风解释东西**。

---

## 视觉 DNA

默认视觉语言：

- 暖米白 / 象牙色纸张背景
- 明显的彩铅、蜡笔、木颜色铅笔颗粒
- 橙红 + 钴蓝为主，石墨灰辅助
- 中文手写标题，允许轻微歪斜、粗细不均、笔触毛边
- 上半区是短标题与短解释，下半区是一个完整物理场景
- 大量安静留白，不塞满画面
- 低科技、生活化的物件：桥、河、水管、箱子、旧机器、工具、桌子、插头、容器、轨道
- 人物比例自然，动作明确，不做 Q 版 mascot
- 一页只讲一个核心认知动作

### 不是这种风格

- PPT 信息图
- 正式流程图
- 复杂架构图
- 商业扁平插画
- 科技 UI / dashboard
- 3D 渲染
- glossy AI art
- 儿童绘本
- 密集文字海报
- 真实 App 截图

---

## 适合什么内容

特别适合：

- AI / Agent / 产品 / 创业 / 商业
- 职业选择与方法论
- 反常识观点
- 概念拆解
- 前后对比
- 因果机制
- 用户研究
- 收入模型
- Build in Public
- 开源产品复盘
- 小红书 5-9 页轮播
- 公众号正文插图
- Notion / 博客 / 方法论文档

不太适合：

- 需要严格数据精度的统计图表
- 正式企业架构图
- 复杂技术拓扑
- 真实产品 UI 演示
- 高端商业 KV / 摄影海报
- 需要精确复刻某个已存在 IP 的任务

---

## 一页是怎么组成的

默认最多四层：

1. **主标题**：1-3 行，通常 10-24 个中文字；
2. **短解释**：2-6 行；
3. **强调句**：可选，用橙红色；
4. **插画内标注**：0-5 个短词。

插画不是装饰，而是这页的第二种表达语言。

例如：

> 不是能收费，而是能持续收钱。

不要画一个普通的人民币符号。

可以画：一边是短暂暴雨砸进桶里，另一边是稳定水流汇成河。文字解释“暴雨 = 一次爆单，河流 = 可重复收入”。

这就是 Skill 里的“物理隐喻”。

---

## 安装

克隆仓库：

```bash
git clone https://github.com/lavine888/crayon-doodle-illustrations.git
cd crayon-doodle-illustrations
```

复制 Skill 到 Codex skills 目录：

```bash
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
cp -R ./crayon-doodle-illustrations "${CODEX_HOME:-$HOME/.codex}/skills/"
```

安装后，在 Codex 里直接：

```text
Use $crayon-doodle-illustrations 把下面这篇文章做成 7 页彩铅涂鸦风小红书轮播。

<粘贴文章>
```

---

## 怎么用

### 只做轮播规划

```text
Use $crayon-doodle-illustrations 先不要生成图片。
把下面文章拆成 7 页轮播。

每页输出：
- 核心判断
- 主标题
- 短解释
- 橙红强调句
- 核心视觉隐喻
- 人物动作
- 主要物件
- 构图

最后检查连续两页有没有同构。

<文章>
```

### 直接生成整组轮播

```text
Use $crayon-doodle-illustrations 把下面文章做成 6 页竖版图文卡并直接生成图片。

要求：
- 3:4
- 暖米白纸张
- 橙红 + 钴蓝中文手写字
- 明显彩铅 / 蜡笔颗粒
- 上文下图
- 每页一个物理隐喻
- 不要 PPT 信息图
- 不要平台 UI
- 每页单独生成

<文章>
```

### 长文配图策略

```text
Use $crayon-doodle-illustrations 给这篇长文做配图策略。
不要平均配图，只挑认知锚点：反常识判断、核心机制、前后对比、商业后果、边界条件、行动建议。
默认 6-8 张，先输出 shot list，不要生图。

<文章>
```

### 单个观点做一张图

```text
Use $crayon-doodle-illustrations 为这个观点生成一张 3:4 中文知识卡：

“产品能跑，不等于产品能卖。”

不要直接画漏斗或人民币符号。
重新发明一个具体物理隐喻。
```

### 做封面

```text
Use $crayon-doodle-illustrations 为这组轮播生成封面。
标题控制在 1-3 行，解释尽量少，底部只保留一个强隐喻主体。
让它比正文页更集中，但仍保持同一纸张、色板和笔触。
```

### 改图：去掉平台 UI

```text
Use $crayon-doodle-illustrations 编辑这张图。
去掉 1/9 页码、左右箭头、底部轮播圆点和其他 App UI。
补回相同暖米白纸张，其他画面不变。
```

### 改图：太像 PPT

```text
Use $crayon-doodle-illustrations 这张图的意思对，但太像 PPT。
保留核心判断，去掉规则方框、网格、正式箭头和 dashboard 感。
改成一个具体物理场景，用彩铅和手写字重新表达。
```

更多可复制 prompt 见 [`examples/prompts.md`](examples/prompts.md)。

---

## Skill 内部工作流

1. 读取文章 / Markdown / Notion / 截图 / 主题
2. 提炼真正的认知锚点
3. 把每页压缩成一个“单页判断”
4. 生成短标题、短解释、强调句
5. 把抽象关系变成物理动作
6. 选择一个低科技物件或场景承载动作
7. 设计 5-9 页的叙事顺序
8. 每页单独调用图像模型
9. 保持暖米白、橙红、钴蓝和彩铅颗粒稳定
10. 检查平台 UI、中文错字、PPT 感和构图重复
11. 必要时用编辑配方局部修图
12. 重要输出跑 benchmark rubric
13. 保存最终 PNG，并报告用途和路径

---

## Reference System

真正的稳定性来自 `references/`，不是 README 里的几句 prompt。

| 文件 | 作用 |
|---|---|
| `style-dna.md` | 纸张、材质、色板、线条、禁忌 |
| `layout-system.md` | 封面 / 正文 / 图文比例与留白 |
| `copywriting-system.md` | 把长文压缩成单页手写文案 |
| `visual-metaphors.md` | 原创物理隐喻生成法 |
| `character-language.md` | 创客观察者、多人关系、动作库 |
| `carousel-sequencing.md` | 5-9 页轮播推进与连续性 |
| `prompt-template.md` | 生图 / 封面 / 系列 / 编辑提示词 |
| `editing-recipes.md` | 常见失败的局部修图方法 |
| `qa-checklist.md` | 生成后必过检查 |
| `benchmark-rubric.md` | 20 分制质量 benchmark |

---

## 示例与 Benchmark

`examples/` 不是只有 prompt，还承担公开 benchmark。

目前结构：

```text
examples/
├── README.md
├── prompts.md
├── shot-list-examples.md
└── images/
    └── README.md
```

建议最终补齐至少 8 张原创样片：

- 产品验证
- 持续收入
- AI 交付系统
- 城市产业密度
- 内容复利
- 开源产品化
- 用户痛点
- 完整产品 / 交付

公开 benchmark 图片应该是**由这个 Skill 生成的原创样片**，不要把第三方参考截图直接放进仓库。

---

## 参考图怎么用

这个 Skill 的视觉研究来自用户提供的一组“手绘讲义式知识卡”参考图。

只抽取通用视觉语法：

- 暖米白纸张
- 彩铅 / 蜡笔颗粒
- 橙红 + 钴蓝
- 中文手写标题
- 上文下图
- 低科技物理隐喻
- 轻微不完美的线条
- 系列轮播的一致性

不复制：

- 具体人物
- 精确服装
- 原文案
- 独特机器 / 动物 / 桥梁组合
- 精确构图
- 平台 UI

原则：**借语法，不抄句子；借材质，不抄构图。**

详见 [`NOTICE.md`](NOTICE.md)。

---

## 为什么明确禁止平台 UI

很多参考图来自社交平台截图，截图里会混入：

- `1/9` 页码
- 左右翻页箭头
- 底部轮播圆点
- App 控件

这些不是原画的一部分。

Skill 在 `SKILL.md`、`prompt-template.md`、`editing-recipes.md` 和 QA 中都明确把它们当作污染项处理。

---

## Benchmark 标准

正式公开前可以按 10 个维度打分，每项 0-2：

- Paper
- Material
- Palette
- Typography
- Metaphor
- Composition
- Character use
- Series consistency
- Text accuracy
- Originality

一般建议至少 **16/20**，且纸张、材质、色板、文字、隐喻五项不能出现 0 分。

完整标准见 [`crayon-doodle-illustrations/references/benchmark-rubric.md`](crayon-doodle-illustrations/references/benchmark-rubric.md)。

---

## 目录结构

```text
.
├── .gitignore
├── LICENSE
├── NOTICE.md
├── README.md
├── examples/
│   ├── README.md
│   ├── prompts.md
│   ├── shot-list-examples.md
│   └── images/
│       └── README.md
└── crayon-doodle-illustrations/
    ├── SKILL.md
    ├── agents/
    │   └── openai.yaml
    ├── assets/
    │   └── examples/
    │       └── README.md
    └── references/
        ├── style-dna.md
        ├── layout-system.md
        ├── copywriting-system.md
        ├── visual-metaphors.md
        ├── character-language.md
        ├── carousel-sequencing.md
        ├── prompt-template.md
        ├── editing-recipes.md
        ├── qa-checklist.md
        └── benchmark-rubric.md
```

真正需要安装到 Codex 的是：

```text
crayon-doodle-illustrations/
```

---

## 和“小黑配图 Skill”的关系

两者可以解决相似的“把文章认知画出来”问题，但视觉语言不同：

**Ian Xiaohei Illustrations**

- 纯白
- 黑色线稿
- 小黑 IP
- 16:9 正文解释图
- 怪诞产品草图

**Crayon Doodle Illustrations**

- 暖米白
- 彩铅 / 蜡笔颗粒
- 橙红 + 钴蓝中文手写字
- 3:4 / 4:5 竖版知识卡
- 手绘讲义 / 创意笔记
- 更强调完整轮播叙事和图上短文案

不是替代关系，是两套不同视觉资产生产系统。

---

## License

MIT License。详见 [`LICENSE`](LICENSE)。

参考图与生成图的使用边界见 [`NOTICE.md`](NOTICE.md)。

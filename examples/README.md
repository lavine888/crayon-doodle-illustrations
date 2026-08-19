# Examples

这个目录用于放可直接复用的 prompt、shot list 和最终风格样片。

## 现在包含

- `prompts.md`：常用调用模板。
- `shot-list-examples.md`：把文章拆成 5-9 页的完整示例。
- `images/`：最终生成的 benchmark 图片目录。

## 推荐 benchmark 主题

为了测试 Skill 是否真的稳定，不要只生成同一类“创业知识卡”。建议至少覆盖：

1. **产品验证**：Demo 能跑 ≠ 有人愿意买。
2. **持续收入**：一次性成交 vs 可重复续费。
3. **AI 工作流**：模型能力 vs 交付系统。
4. **职业选择**：学校品牌 vs 城市产业密度。
5. **内容系统**：一次爆款 vs 长期内容资产。
6. **开源增长**：代码仓库 vs 可传播产品。
7. **用户研究**：自己觉得有用 vs 用户真的会痛。
8. **复杂系统**：代码只是核心，部署/服务/硬件/交付组成完整产品。

## Benchmark 通过标准

一组 8 张样片应该同时做到：

- 第一眼明显属于同一套视觉语言。
- 不是 8 张同构模板。
- 每张都有新隐喻。
- 暖米白纸张稳定。
- 橙红 / 钴蓝稳定。
- 彩铅颗粒明显，但不脏。
- 中文信息足够短，错字可控。
- 没有平台 UI。
- 没有 PPT / 矢量信息图感。
- 不依赖参考截图里的具体人物或物件。

## 图片命名

```text
examples/images/
├── 01-product-validation.png
├── 02-recurring-revenue.png
├── 03-ai-delivery-system.png
├── 04-city-industry-density.png
├── 05-content-compounding.png
├── 06-open-source-product.png
├── 07-user-pain.png
└── 08-whole-product.png
```

Skill 安装目录中的 `assets/examples/` 可以放低频风格校准图；根目录 `examples/images/` 用于 README 展示和公开 benchmark。两者用途不同。

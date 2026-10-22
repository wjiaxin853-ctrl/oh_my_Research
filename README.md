<div align="center">

# 🌌 Oh My Research

### ✨ 我的论文阅读与研究笔记 · My Research Garden

**把论文读薄，把问题想深；让零散的阅读，慢慢长成自己的研究地图。**

📚 论文阅读　·　🧠 方法拆解　·　🧪 实验思考　·　🌱 持续积累

![Research Notes](https://img.shields.io/badge/Research-Notes-6C63FF?style=for-the-badge)
![Paper Reading](https://img.shields.io/badge/Paper-Reading-00A896?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Growing-F4A261?style=for-the-badge)
![Language](https://img.shields.io/badge/Notes-中文-E76F51?style=for-the-badge)

**[🗺️ 研究地图](#-研究地图) · [🌟 精选入口](#-精选阅读入口) · [📂 仓库结构](#-仓库结构) · [🔖 如何使用](#-如何使用)**

</div>

---

## 👋 欢迎来到我的研究花园

这里记录我在论文阅读、方法理解和研究实践中的阶段性思考。

仓库不会只保存论文 PDF，也会保存阅读过程中真正有价值的内容：一张图的解释、一个公式的拆解、一种训练策略的直觉，以及从论文方法延伸出来的问题。

> 🌱 **研究笔记不是论文的复述，而是理解留下的痕迹。**<br>
> 从“论文讲了什么”，走向“为什么这样设计”，再走向“我还能怎样验证”。

## 🗺️ 研究地图

当前仓库从 **CoT 压缩与大模型推理** 专题开始，后续会逐步扩展到更多论文方向。

| 方向 | 这里记录什么 | 当前入口 |
| :--- | :--- | :--- |
| 🧠 **大模型推理** | 思维链、推理模型、推理长度与模型能力 | [CoT 专题](论文/CoT/) |
| 🗜️ **CoT 压缩** | 语义压缩、问题感知压缩器、Token 重要性 | [Extra-CoT 笔记](论文/CoT/Extra-CoT.md) |
| 🎯 **训练方法** | Mixed-ratio SFT、压缩数据构造与训练流程 | [方法拆解](论文/CoT/Extra-CoT.md) |
| 🧪 **研究思考** | 论文图表解读、公式直觉与可验证的问题 | [阅读记录](论文/CoT/Extra-CoT.md) |

<details>
<summary><strong>🔭 未来可能扩展的方向</strong></summary>

模型结构、视觉语言模型、深度估计、多模态理解，以及与实际工程问题相关的论文阅读记录。

</details>

## 🌟 精选阅读入口

不必从头浏览整个仓库，可以从一个具体问题开始。

### 🗜️ CoT 压缩：如何让推理更短，但语义不丢失？

| 想了解什么 | 推荐入口 |
| :--- | :--- |
| 论文研究了什么问题 | [Extra-CoT 论文笔记](论文/CoT/Extra-CoT.md) |
| CoT Compressor 如何工作 | [语义压缩器拆解](论文/CoT/Extra-CoT.md) |
| Word-level 与 Token-level 的关系 | [原子化分割与 Token 映射](论文/CoT/Extra-CoT.md) |
| Question-aware 是什么意思 | [问题感知的重要性评分](论文/CoT/Extra-CoT.md) |
| Mixed-ratio SFT 如何理解 | [混合比例监督微调](论文/CoT/Extra-CoT.md) |

<details>
<summary><strong>🧭 一条可选的阅读路线</strong></summary>

```text
理解论文问题
      ↓
拆解整体方法与训练阶段
      ↓
区分 Word / Formula / Token
      ↓
理解重要性评分与掩码机制
      ↓
思考压缩率、语义保持与推理能力之间的关系
      ↓
提出可验证的实验问题
```

这是一条辅助理解的路线，不要求所有论文都按同样顺序阅读。

</details>

## 📂 仓库结构

```text
oh_my_Research/
├── README.md                         # 研究仓库首页
├── 论文/
│   └── CoT/                          # Chain-of-Thought 专题
│       └── Extra-CoT.md              # CoT 压缩论文阅读笔记
└── imgs/                             # 笔记中的论文图示与截图
    ├── Pasted image ...png
    └── 截屏...png
```

> 目录会随着阅读主题增加而调整。每个专题尽量保留“原始材料 + 结构化笔记 + 图示素材”的关联关系。

## 🔖 如何使用

**在线阅读**：从 [研究地图](#-研究地图) 进入专题，或直接打开 [CoT 笔记](论文/CoT/Extra-CoT.md)。

**本地阅读**：克隆仓库后，用支持 Markdown 的编辑器打开笔记；图片已经统一放在 `imgs/` 目录中，并通过相对路径引用。

```bash
git clone https://github.com/wjiaxin853-ctrl/oh_my_Research.git
cd oh_my_Research
```

**继续维护**：新增论文时，建议同步补充三部分内容：

- 一份简洁的论文定位：研究问题、核心贡献和适用场景。
- 一份结构化的方法拆解：关键模块、训练流程、公式和图表。
- 一组可复用的图片素材：统一放入 `imgs/`，并在 Markdown 中使用相对路径。

## 🌱 我的阅读方式

我希望每篇笔记都逐步回答下面几个问题：

- **问题**：论文试图解决什么困难？
- **方法**：作者提出了什么机制？它为什么可能有效？
- **证据**：实验如何证明方法有效？还有哪些边界？
- **理解**：我能否用自己的语言、公式或图示重新讲清楚？
- **延伸**：这个方法还能应用到哪里？下一步可以验证什么？

论文笔记会随着再次阅读、实验验证和讨论持续修订。这里记录的是一个不断生长的研究过程，而不是一次性完成的资料汇编。

欢迎通过 [Issues](https://github.com/wjiaxin853-ctrl/oh_my_Research/issues) 交流论文理解、补充资料或提出修改建议。

---

<div align="center">

### ✨ Read Deeply · Think Clearly · Build Continuously

**以问题为起点，以理解为过程，以验证为答案。**

<sub>📚 Made for reading, thinking & researching.</sub>

</div>

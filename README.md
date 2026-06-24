# Shupuppy Illustrations

> 用固定的白色小狗 IP「薯条」，为中文文章生成彩铅/蜡笔质感的概念正文配图。
>
> 16:9 横版 | 白底 | 蓝色手绘线 | 蓝黄红小色块 | 中文文章概念配图 | Codex Skill

## 这个仓库是什么

Shupuppy Illustrations 是一个 Codex Skill，用来指导 AI Agent 为中文文章、帖子、博客、Notion 文档、方法论内容和工作流内容生成正文配图 prompt，必要时也可以直接调用图像模型生成图片。

它不是宠物写真 prompt，也不是萌宠头像生成器。它的目标是把文章里的一个判断、流程、结构、状态或隐喻，变成一张有记忆点的概念配图，并让白色小狗「薯条」参与核心动作。

薯条的定版记忆点是：大黑圆鼻、小黑豆眼、大耳朵、白色圆头、小围兜。画风是彩铅/蜡笔质感、蓝色手绘线、白底、蓝黄红小色块。

## 适合谁用

适合：

- 写中文文章，需要正文配图的人
- 做知识型内容、方法论内容、AI 工作流内容的人
- 想把抽象判断画成具体隐喻的人
- 想复用一套有固定角色和个人风格的配图语言的人

不适合：

- 想生成宠物写真、真实比熊肖像或萌宠头像的人
- 想做复杂 PPT 信息图、正式流程图或架构图的人
- 想把大量正文和完整说明塞进一张图的人
- 需要严格可编辑矢量源文件的人

## 安装

克隆仓库：

```bash
git clone https://github.com/Agengcc/shupuppy-illustrations.git
cd shupuppy-illustrations
```

复制 skill 到 Codex skills 目录：

```bash
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
cp -R ./shupuppy-illustrations "${CODEX_HOME:-$HOME/.codex}/skills/"
```

安装后，在 Codex 里使用：

```text
Use $shupuppy-illustrations 给这篇文章配一张薯条插图。
```

## 怎么用

### 为单个观点生成一张图

```text
Use $shupuppy-illustrations 为这个观点生成一张薯条文章配图：

真正重要的不是把所有信息都塞进去，而是叼走那个能解释问题的重点。
```

### 给文章做配图策略

```text
Use $shupuppy-illustrations 先不要生图。
请分析下面这篇文章哪里值得配图，输出 4 张左右的 shot list。
每张图写清楚：放在哪段后、主题、核心意思、结构类型、薯条在做什么、建议中文标注词。

<粘贴文章>
```

### 直接生成正文配图

```text
Use $shupuppy-illustrations 把下面这篇文章生成 3 张薯条正文配图。
要求：16:9 横版、白底、彩铅/蜡笔质感、蓝色手绘线、蓝黄红小色块。

<粘贴文章>
```

## 目录结构

```text
.
├── README.md
├── LICENSE
├── NOTICE.md
└── shupuppy-illustrations/
    ├── SKILL.md
    ├── agents/
    │   └── openai.yaml
    ├── gotchas.md
    └── references/
        ├── shutiao-ip.md
        ├── style-dna.md
        ├── composition-patterns.md
        └── prompt-template.md
```

真正需要安装到 Codex 的是子目录：

```text
shupuppy-illustrations/
```

## 设计原则

- 薯条必须参与核心动作，不能只是坐在角落卖萌。
- 一张图只表达一个核心判断、结构、状态或隐喻。
- 中文标注要少、短、像手写批注，不要变成说明书。
- 不追求真实比熊还原，不做宠物写真。
- 保持大黑圆鼻、小黑豆眼、大耳朵、白色圆头、小围兜。
- 使用彩铅/蜡笔质感、蓝色手绘线、白底、蓝黄红小色块。

## 声明

本项目参考并改造自 [Ian Xiaohei Illustrations](https://github.com/helloianneo/ian-xiaohei-illustrations) 的仓库结构和 skill 工作流。原项目的「小黑」IP、示例图片和视觉语言属于 Ian 的项目，本仓库不包含这些资产；本仓库定义的是独立的「薯条」白色小狗文章配图 IP。


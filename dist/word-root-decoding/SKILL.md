---
name: word-root-decoding
description: |
  当用户想理解或记忆英语单词的词义来源时使用：看到生词想"拆开看"、问"这个词怎么拆/词根词缀什么意思"、想按词根成批记词、或分不清 ject/port、fer/mit/duc 等近义词根时。
  核心是把词拆成"25 个具象动作词根 + 方向前缀"，用"先找动作再看方向"现场推导词义；覆盖词=动作+方向的模型、生词拆解流程、近义动作手感辨析、词族批量记忆。
  不适用于：希腊词根词、单音节基础词、拟声词、只需读音拼写用法的场景，或需要权威词源/精确释义的学术与考试答案场景；本技能是助记推导法，不是严格词源学。
  Triggers: 拆词, 词根, 词缀, 怎么记单词, 近义词根区别, word root, prefix, break down word, decode word, word family。
metadata:
  cangjie.generated-by: cangjie-tools v2.5.0
  cangjie.variant: single
  cangjie.bundle-id: bundle.word-root-decoding
  cangjie.capability-count: 4
  cangjie.entrypoint-count: 1
---
# 词根动作拆词法 — 全书能力入口

## 触发与不触发

**适用**：与本书能力域相关的咨询与任务（见下方路由表的意图列）。
**不适用**：
- 希腊词根词（photo/tele/geo…）、单音节基础词、拟声词、外来词
- 需要严格学术词源或权威标准释义的场景
- 单词的读音、拼写、搭配、语域、用法（本技能只解决理解与记忆入口）

## 核心原则（常驻速览，概览类问题读到这里即可回答）

1. 词 = 一个具象动作词根 + 一个方向前缀，词义是动作被方向修饰后的结果
2. 记 25 个动作而非 191 个孤立的词，靠推导而非死记
3. 遇到生词先找动作、再看方向、组合词义，最后校验
4. 近义动作根靠动作过程的手感差异辨析，不靠中文释义
5. 一个动作根配方向前缀表可批量成族记忆

## 能力路由（先读本表，按意图加载 1 张能力卡）

| 用户意图 | 先读 | 补读/备注 |
|---|---|---|
| 理解某个词为什么是这个意思；询问词根词缀法是什么；搞懂一族词的构成 | references/capabilities/word-decoding-core.md | references/capabilities/word-decode-flow.md、references/capabilities/root-feel-discrimination.md |
| 遇到没见过的生词想现场推断含义；想知道怎么拆词/怎么自己推导词义；想自测是否掌握拆词法 | references/capabilities/word-decode-flow.md | references/capabilities/word-decoding-core.md、references/capabilities/root-feel-discrimination.md、references/capabilities/word-family-scaling.md |
| 分不清两个近义词根的区别；拆词时在多个动作根之间犹豫；想系统整理易混词根对照 | references/capabilities/root-feel-discrimination.md | references/capabilities/word-decoding-core.md、references/capabilities/word-decode-flow.md |
| 想批量记单词/按词根串起来记；想列全某个词根家族的词；想复习巩固某类词根 | references/capabilities/word-family-scaling.md | references/capabilities/word-decoding-core.md、references/capabilities/word-decode-flow.md |

**非能力类查询**：
- 书名/作者/章节/整书概览 → references/overview.md
- 术语解释 → references/glossary.md
- 决策规则速查（不需要原文依据时） → references/cheatsheet.md
- 完整意图与关键词索引（本表未覆盖的意图先查这里） → references/capability-index.md

## 加载规则

- 每次任务先读本文件，再按路由表加载 **1** 张能力卡；任务明确跨域时最多加载 2 张。
- 概览/书名类问题不加载能力卡，用「核心原则」与 overview.md 回答。
- 路由表与 capability-index.md 都无法命中的意图，明确告知超出本书范围，不要硬套。

## 边界与判停

- 生词不含 25 个动作根中的任何一个时，停止强行拆解，改用语境/词典
- 词根动作感明显不透明（如 effect 效果、object 物体）时，标注存疑而非编造动作故事
- 推导出的词义牵强或无法自圆其说时，建议查词典确认

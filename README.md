# 词根动作拆词法（word-root-decoding）

把一段英语词汇教学长视频的字幕，用 [cangjie-skill](https://github.com/) 的 RIA-TV++ 流水线蒸馏成一套 agent 可执行的「拆词推理」技能。

> 核心思想：**词 = 一个具象动作（词根）+ 一个方向（前缀）**。
> 记住 25 个动作和一张方向表，遇到生词走「先找动作 → 再看方向 → 组合词义 → 校验」，就能现场推导，而不是死记硬背。

## 这是什么

源材料是一段长视频字幕（UP 主未署名），讲的是英语词根词缀记忆法。本仓库保存了从原始字幕到一个可安装技能（skill）的完整蒸馏过程与产物：

- **DIGEST.md** — 面向读者的精华长文（4 个核心方法论 + 陷阱 + 作者局限）
- **BOOK_OVERVIEW.md** — 阶段 0 整书理解（结构 / 解释 / 批判 / 应用）
- **GLOSSARY.md** — 术语词典（7 方法论术语 + 25 动作根 + 22 方向前缀）
- **verified.md** — 三重验证结果（通过 4 个、淘汰 2 个及理由）
- **candidates/** — 5 路并行提取的 115 条原始候选（框架 / 原则 / 案例 / 反例 / 术语）
- **rejected/** — 淘汰单元及原因
- **.cangjie/capabilities/** — Capability Bundle（4 张 RIA 能力卡 + verified.yaml + 压力测试）
- **dist/word-root-decoding/** — 编译后的可安装 skill（single 模式：1 入口 + 4 能力卡）
- **PIPELINE_STATE.md** — 流水线状态与关键决策记录

## 四个核心能力

| 能力卡 | 作用 |
|---|---|
| `word-decoding-core` | 拆词核心模型：词 = 动作词根 + 方向前缀 |
| `word-decode-flow` | 生词现场拆解流程：先找动作 → 看方向 → 组合 → 校验 |
| `root-feel-discrimination` | 近义动作根手感辨析（ject/port、fer/mit/duc…靠动作过程差异区分） |
| `word-family-scaling` | 词族批量扩展与记忆减负 |

## 质量验证

- 三重验证：115 条候选合并去重后通过 4 个方法论单元
- 压力测试：独立 sub-agent 盲测 **10/10 通过**（正向精准命中、诱饵零误触发、边界正确判停）
- 编译校验：`validate_skill_pack.py` → 0 errors / 0 warnings

## 安装

把 `dist/word-root-decoding/` 整个目录复制到你的 skills 目录即可（如 `~/.workbuddy/skills/word-root-decoding`）。

安装后，遇到「reject 为什么是拒绝」「这个词怎么拆」「ject 和 port 啥区别」「怎么按词根成批记词」这类问题会自动触发。

## 蒸馏流水线

基于 RIA-TV++（阶段 0→5）：整书理解 → 5 路并行提取 → 三重验证 → 晋级门 → RIA++ 能力卡 → Zettelkasten 链接 → 压力测试 → single 编译交付。

## 说明

- 源字幕为语音自动转写，含同音错字（「磁根」=词根、「前坠」=前缀），蒸馏时已按语义还原。
- 这套方法是**助记推导法**，不是严格词源学；只覆盖拉丁动作根 + 前缀路径，希腊词根词（photo/tele/geo）不在射程内。

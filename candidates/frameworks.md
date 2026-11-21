# 框架候选（framework-extractor 产出）

> 来源：视频字幕 3602a2da_VID_1178.txt（1035 行）。字幕为语音自动转写，引用处已按语义还原同音错字（磁根=词根、前坠=前缀、意=词缀等），不照抄错字。
> 不做筛选，宁错杀，交阶段 1.5 三重验证。

```yaml
- id: f01
  title: 核心拆词模型——词 = 动作(词根) + 方向(前缀)
  type: framework
  source_chapter: 字幕行 2-9 / 997-999
  source_quote: |
    "英语里700多个常用词，你看一眼就能拆开。每座城是一个词根一个动作，每条线是一个前缀一个方向。25个动作，191个词，全在这一张图上。"
  summary: |
    把每个常用词看成"一个具象动作(词根) + 一个方向(前缀)"的组合：词根提供动作画面（扔/扛/带/送/引/做/垒/压/折/拉/挂/转/破/关/拿/握/放/伸/站/走/迈/来/跑/看），前缀提供一个空间或逻辑方向（回/里/外/前/下/一起/分开/穿过/中间…）。
    词义 = 动作被方向修饰后的结果。
    这是全篇的地基思维模型，后续的生词推导、手感辨析、词族扩展都由此展开。
  tags: [mental-model, word-decoding, 构词, core]

- id: f02
  title: 生词现场拆解流程——先找动作，再看方向，组合词义
  type: framework
  source_chapter: 字幕行 1000-1003 / 1030-1032
  source_quote: |
    "最后三道题都是没讲过的词，你自己拆。下次再碰到生词，先找动作，再看方向。"
  summary: |
    面对没见过的生词时的通用推理流程：
    ①在词里定位 25 个动作根之一（找到动作画面）；
    ②读前缀，读出方向；
    ③把动作与方向组合，推出词义；
    ④可用"半路拿走→intercept、搬走→deport、来到一起→convene"这类没讲过的自测词现场验证可迁移性。
    这是从已知推向未知的核心路径，也是全篇最能迁移到任意新词的推理方法。
  tags: [reasoning, procedure, word-decoding, transferable]

- id: f03
  title: 近义动作"手感"辨析框架
  type: framework
  source_chapter: 字幕行 52-54 / 127-128 / 167-168 / 344-345 / 628-629 / 663-666 / 707-708 等（多处复现）
  source_quote: |
    "带是跟着走，送是放手让它去；送出去就不管了，引是一路领着走；拿是一下抓起，握是钻着不松；放是放下不动，伸是往外撑开。"
  summary: |
    近义动作根不靠中文释义区分，而靠动作过程的身体"手感"差异：
    扔是一下离手 vs 扛是一路带着走；带是跟着走 vs 送是放手让它去 vs 引是一路领着走；压是往下按 vs 折是叠起来；拉是往这边拽 vs 挂是吊着不落地；转是绕着转 vs 破是一下崩开；拿是一下抓起 vs 握是钻着不松 vs 放是撒手；放是放下不动 vs 伸是往外撑开；走是一路往前 vs 迈是一步一阶台阶；来是到了就停 vs 跑是一刻不停。
    抓住"过程感"即可精细辨析易混词根，避免用错。
  tags: [reasoning, discrimination, 手感, near-synonyms]

- id: f04
  title: 词族批量扩展框架——一个动作根带一串词
  type: framework
  source_chapter: 字幕行 29-46 / 51-86 / 997-999
  source_quote: |
    "25个动作，191个词，全在这一张图上。你记住的是25个动作，下次再碰到生词先找动作再看方向。"
  summary: |
    以单一动作词根为核心，配一张方向前缀表，批量生成并复习一整族词：
    ject→reject/inject/eject/project/object/adjective/trajectory；
    port→import/export/support/report/transport/passport/portfolio；
    mit→submit/promise/permit/admit/transmit/emit/dismiss/mission…。
    用"根 × 方向"的组合系统替代 191 个孤立单词的记忆，记一个根等于记一串词，显著压缩记忆负荷，是全篇"规模复用"的框架。
  tags: [mental-model, scale, word-family, 记忆负荷]

- id: f05
  title: 动作意象化记忆法——把词根转成看得见的身体画面
  type: framework
  source_chapter: 字幕行 10-13 / 195-198 / 585-587 等（贯穿全篇）
  source_quote: |
    "扔，投石机一甩，石头离手，飞出去就不管了。做，铁锤一下一下把东西做出来。拿，铁钳往下一探一合，把铜币拿了起来。"
  summary: |
    记词根时不记抽象中文释义，而把它还原成一个看得见、可想象的身体动作画面：投石机甩石头(ject)、人扛货一路走(port)、铁锤一锤锤做东西(fact)、铁钳夹铜币(cept)、水车转(vert)、绳子绷紧拉(trac)…。
    具象画面成为记忆锚点，抽象词义由画面推导、再由方向前缀修饰。
    这是贯穿全篇的记忆/推理方法，也是"手感辨析"能成立的前提。
  tags: [mental-model, imagery, memory, 具象化]

- id: f06
  title: 前缀统一重框为"方向"——把构词部件纳入方向坐标系
  type: framework
  source_chapter: 字幕行 9 / 15-31 / 63-68 等（贯穿全篇）
  source_quote: |
    "每条线是一个前缀一个方向：往回、向里、向外、向前、从下面拖着、跨过去、在中间、一起。"
  summary: |
    面对前缀时不再逐个死记词义，而是把所有前缀统一还原为一种"方向"语义：回(re)/里(in,im)/外(ex,e)/前(pro)/下(sub,de)/一起(con,com)/分开(dis)/穿过(per,trans)/中间(inter)/朝着(ad)/离开(ab,de)…。
    把零散构词部件纳入统一的方向坐标系，降低记忆维度、提升推导一致性。
    注意：对 con(一起)、per(到底)、ad(朝着) 等抽象引申义，把前缀一律解释为"方向"是一种简化（详见 BOOK_OVERVIEW 批判），此框架带有该边界。
  tags: [mental-model, reframe, prefix, 方向]

- id: f07
  title: 演示归纳法——"意象→配前缀→释义→自测"的讲根模板
  type: framework
  source_chapter: 字幕行 997-1024 / 全篇结构
  source_quote: |
    "25个动作，191个词，全在这一张图上。最后三道题都是没讲过的词，你自己拆，答案先打在弹幕里。"
  summary: |
    讲解或学习任一词根的标准序列：先给一个具象动作意象 → 依次配上不同方向前缀 → 逐个给出"动作+方向"的词义 → 覆盖成词族 → 最后用没讲过的生词（intercept/deport/convene）现场自测验证。
    由演示归纳代替死记，把方法论从"看懂"推到"会用"，是全篇论证链的结构化流程。
  tags: [procedure, teaching, 演示归纳, validation]
```

# 原则 / 清单 / 规则 / 断言 — 候选单元（principle-extractor 产出）

> 说明：字幕为语音自动转写，source_quote 已按语义还原同音错字（磁根→词根、磁→词、前坠→前缀、意→词缀、键→建等）。不做筛选，宁错杀。

```yaml
- id: p01
  title: 拆词总规则：词 = 一个动作词根 + 一个方向前缀
  type: principle
  source_chapter: 开篇总纲（字幕 L8-L9）
  source_quote: |
    "每个词是一个词根一个动作，每条线是一个前缀一个方向。"
  summary: |
    作者给出的总原则：把任意一个词拆成"具象动作（词根）+ 空间/逻辑方向（前缀）"两块。
    词义 = 动作被方向修饰后的结果。这是后续所有拆解的出发点。
  tags: [principle, core-model, 拆词, 动作+方向]

- id: p02
  title: 生词现场拆解口诀：先找动作，再看方向
  type: principle
  source_chapter: 收尾（字幕 L1030-L1032）
  source_quote: |
    "下次再碰到生词，先找动作，再看方向。"
  summary: |
    遇到没见过的词的可执行顺序：先在词里定位 25 个动作根之一，再读前缀方向，
    最后组合出词义。作者强调这是可迁移到任意新词的动作口诀。
  tags: [principle, rule, 拆词流程, 口诀, 可迁移]

- id: p03
  title: 记忆策略：记 25 个动作，而不是 191 个孤立的词
  type: principle
  source_chapter: 收尾（字幕 L997-L999, L1025-L1029）
  source_quote: |
    "25 个动作，191 个词，全在这一张图上。你已经把 191 个词从头拆到了尾，一个都没死记，你记住的是 25 个动作。"
  summary: |
    作者主张把记忆对象从"词"换成"动作"：记 25 个动作画面而非 191 个词，
    靠推导而不是死记来掌握生词，降低记忆负荷。
  tags: [principle, 记忆策略, 减负, 动作优先]

- id: p04
  title: 自测规则：用没讲过的词现场拆
  type: principle
  source_chapter: 课后自测（字幕 L1000-L1003）
  source_quote: |
    "最后三道题都是没讲过的词，你自己拆，答案先打在弹幕里。"
  summary: |
    学完流程后必须用未讲过的生词（intercept/deport/convene）自己套流程拆解，
    以验证方法是否真正可迁移，而不是只会复述讲过的词。
  tags: [principle, rule, 自测, 迁移]

- id: p05
  title: 记忆策略：建议先收藏，反复看
  type: principle
  source_chapter: 开篇（字幕 L6-L7）
  source_quote: |
    "建议先收藏，反复看。"
  summary: |
    作者明确给出的行为建议：先收藏视频并反复观看，按动作图反复对照记忆。
    （口号式话术，方法论价值低，但属"要这样做"式断言，按宁错杀原则收录。）
  tags: [principle, 记忆策略, 口号, 低置信]

- id: p06
  title: 方向前缀映射规则（清单）：前缀一律读作方向
  type: checklist
  source_chapter: 全文总纲及各词根段
  source_quote: |
    "每条线是一个前缀一个方向。"（re 往回 / in 向里 / ex 向外 / pro 向前 / sub 下面 / con 一起 / dis 分开…）
  summary: |
    把前缀统一映射为方向：re=往回、in/im=里、ex/e=外、pro=前、sub/de=下、con/com=一起、
    dis=分开、per/trans=穿过、inter=中间、ad/ob=朝着、pre=前、post=后、ab=离开、
    sus=下面、oc=迎面、retro=往后、uni=一。拆词时先读出前缀方向。
  tags: [checklist, 前缀, 方向映射, 清单]

- id: p07
  title: 扔 vs 扛：扔是一下离手，扛是一路扛着走
  type: principle
  source_chapter: ject / port 段（字幕 L47-L54）
  source_quote: |
    "扔是一下离手，扛是一路扛着走。"
  summary: |
    区分扔(ject)与扛(port)的手感：扔是投石机一甩、石头离手飞出去就不管；
    扛是扛着货一路带过去。一个"离手即止"，一个"持续承载"。
  tags: [principle, rule, 手感辨析, 扔, 扛, ject, port]

- id: p08
  title: 带 vs 送：带是跟着走，送是放手让它去
  type: principle
  source_chapter: fer / mit 段（字幕 L123-L128）
  source_quote: |
    "带是跟着走，送是放手让它去。"
  summary: |
    区分带(fer)与送(mit/miss)的手感：带是承载东西跟着自己一起走；
    送是把东西交出去、放手让它自己去，不再随行。
  tags: [principle, rule, 手感辨析, 带, 送, fer, mit]

- id: p09
  title: 送 vs 引：送出去就不管，引是一路领着走
  type: principle
  source_chapter: mit / duct 段（字幕 L164-L168）
  source_quote: |
    "送出去就不管了，引是一路领着走。"
  summary: |
    区分送(mit)与引(duc/duct)的手感：送是放手让对象自己去；
    引是自己领着对象一路走（如把水引出来、把电引过去）。
  tags: [principle, rule, 手感辨析, 送, 引, mit, duct]

- id: p10
  title: 做 vs 垒：做是一锤一锤，垒是一块一块往上垒
  type: principle
  source_chapter: fact / struct 段（字幕 L195-L198, L233-L236）
  source_quote: |
    "做是一锤一锤，垒是一块一块往上垒。"
  summary: |
    区分做(fact)与建/垒(struct)的手感：做是用锤一下一下敲打成形；
    垒是一块一块向上堆叠搭建。反过来往下拆即 destroy。
  tags: [principle, rule, 手感辨析, 做, 垒, fact, struct]

- id: p11
  title: 垒 vs 型：垒出来的是结构，倒进模子出来的是型
  type: principle
  source_chapter: struct / form 段（字幕 L271-L275）
  source_quote: |
    "累出来的是结构，倒进模子出来的是型。"
  summary: |
    区分 struct 与 form：一块块垒起来的叫结构(structure)；
    倒进模子定形出来的叫型(form)。
  tags: [principle, rule, 手感辨析, 垒, 型, struct, form]

- id: p12
  title: 压 vs 折：压是往下按，折是叠起来
  type: principle
  source_chapter: press / plic 段（字幕 L341-L345）
  source_quote: |
    "压是往下按，折是叠起来。"
  summary: |
    区分压(press)与折(plic/ply)的手感：压是硬按下去留下印子；
    折是一层层叠起来（复杂 implicit 即"折在里面"）。
  tags: [principle, rule, 手感辨析, 压, 折, press, plic]

- id: p13
  title: 拉 vs 挂：拉是往这边拽，挂是吊着不落地
  type: principle
  source_chapter: tract / pand 段（字幕 L379-L382, L418-L421）
  source_quote: |
    "拉是往这边拽，挂是吊着不落地。"
  summary: |
    区分拉(tract)与挂(pend/pand)的手感：拉是绳子绷紧一路往自己这边拽；
    挂是吊在秤/钩上悬着、不落地（depend=挂在别人下面）。
  tags: [principle, rule, 手感辨析, 拉, 挂, tract, pend]

- id: p14
  title: 挂 vs 转：挂是吊着不动，转是绕着轴打转
  type: principle
  source_chapter: pand / vert 段（字幕 L468-L472）
  source_quote: |
    "挂是吊着不动，转是绕着轴打转。"
  summary: |
    区分挂(pend)与转(vert)的手感：挂是悬着静止；
    转是像水车一样绕轴打转，带动整条水道动起来。
  tags: [principle, rule, 手感辨析, 挂, 转, pend, vert]

- id: p15
  title: 转 vs 破：转是绕着转，破是一下崩开
  type: principle
  source_chapter: vert / rupt 段（字幕 L509-L514）
  source_quote: |
    "转是绕着转，破是一下崩开。"
  summary: |
    区分转(vert)与破(rupt)的手感：转是连续绕圈运动；
    破是一下崩开裂开一道缝（erupt 从里面破开冲出、interrupt 中间打断）。
  tags: [principle, rule, 手感辨析, 转, 破, vert, rupt]

- id: p16
  title: 破 vs 关：破是崩开，关是合上
  type: principle
  source_chapter: rupt / clud 段（字幕 L548-L552）
  source_quote: |
    "破是崩开，关是合上。"
  summary: |
    区分破(rupt)与关(clud/clus)的手感：破是向外崩裂；
    关是两扇大门一合、门闩落下。include=关在里面，exclude=关在外面。
  tags: [principle, rule, 手感辨析, 破, 关, rupt, clud]

- id: p17
  title: 拿 vs 握：拿是一下抓起，握是攥着不松
  type: principle
  source_chapter: cept / tane 段（字幕 L583-L587, L626-L629）
  source_quote: |
    "拿是一下抓起，握是攥着不松。"
  summary: |
    区分拿(cept/cap)与握(ten/tane)的手感：拿是铁钳一合一探、一下抓起；
    握是攥在手心里一直不放（maintain=维持、sustain=支撑）。
  tags: [principle, rule, 手感辨析, 拿, 握, cept, ten]

- id: p18
  title: 握 vs 放：握是攥着不松，放是撒手
  type: principle
  source_chapter: tane / pos 段（字幕 L661-L666）
  source_quote: |
    "握是攥着不松，放是撒手。"
  summary: |
    区分握(ten)与放(pos/pon)的手感：握是持续抓住不放；
    放是撒手让对象落下、从而有了位置（propose 把想法放到面前）。
  tags: [principle, rule, 手感辨析, 握, 放, ten, pos]

- id: p19
  title: 放 vs 伸：放是放下不动，伸是往外撑开
  type: principle
  source_chapter: pos / tend 段（字幕 L705-L710）
  source_quote: |
    "放是放下不动，伸是往外撑开。"
  summary: |
    区分放(pos)与伸(tend)的手感：放是撒手后静止；
    伸是像绳子一拉把帐篷撑起来、往外延展（extend 延长）。
  tags: [principle, rule, 手感辨析, 放, 伸, pos, tend]

- id: p20
  title: 伸 vs 站：伸是往外撑，站是立柱不动
  type: principle
  source_chapter: tend / sist 段（字幕 L743-L746）
  source_quote: |
    "伸是往外撑，站是力柱不动。"
  summary: |
    区分伸(tend)与站(sist/st)的手感：伸是向外撑开、延展；
    站是像立柱一样立着不动（persist 一直站到最后=坚持）。
  tags: [principle, rule, 手感辨析, 伸, 站, tend, sist]

- id: p21
  title: 走 vs 迈：走是一路往前，迈是一步一阶台阶
  type: principle
  source_chapter: cede / gress 段（字幕 L827-L833）
  source_quote: |
    "走是一路往前，迈是一步一击台阶。"
  summary: |
    区分走(ced/cess)与迈(gress/grad)的手感：走是货车压着一路往前走；
    迈是一步一阶台阶地往上跨（progress 进步、graduate 迈上最后一阶）。
  tags: [principle, rule, 手感辨析, 走, 迈, cede, gress]

- id: p22
  title: 迈 vs 来：迈是自己往上走，来是从远处到这
  type: principle
  source_chapter: gress / ven 段（字幕 L866-L872）
  source_quote: |
    "迈是自己往上走，来是从远处到这。"
  summary: |
    区分迈(gress)与来(ven/vent)的手感：迈是自己一步步向上跨；
    来是从远处向说话者这里移动，城门一开车一辆辆来。
  tags: [principle, rule, 手感辨析, 迈, 来, gress, ven]

- id: p23
  title: 来 vs 跑：来是到了就停，跑是一刻不停
  type: principle
  source_chapter: ven / cur 段（字幕 L909-L915）
  source_quote: |
    "来是到了就停，跑是一刻不停。"
  summary: |
    区分来(ven)与跑(cur/curs)的手感：来是抵达后停下；
    跑是持续流动不停（current 水流/当前的、occur 跑进脑子里=想到）。
  tags: [principle, rule, 手感辨析, 来, 跑, ven, cur]

- id: p24
  title: 看的动作定义：走、迈、来、跑，最后停下来看
  type: principle
  source_chapter: spect 段（字幕 L945-L952）
  source_quote: |
    "看：一路走、迈、来、跑，最后停下来看。走过去了又回头再看一眼，就是 respect 尊重。"
  summary: |
    看(spect/spec)作为动作的收束：其它动作都在"动"，看是停下来用眼睛观察；
    回过头再看一眼=尊重(respect)，从下面打量=suspect，穿过窗框看=perspective。
  tags: [principle, rule, 手感辨析, 看, spect]
```

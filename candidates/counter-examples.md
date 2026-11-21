# 反例 / 陷阱候选（counter-example-extractor 产出）

> 说明：本字幕几乎没有"千万不要…""很多人以为…"式的字面警告。以下绝大多数是**作者在引入新词根时，用"X 是……Y 是……"句式把它和上一个近义根做对照**而暗示的常见混淆点——即"作者通过对比暗示的常见混淆点"，属**推断**，非作者明说的失败模式。凡属推断均在 summary 中标注。source_quote 保留语音转写原貌（含同音错字），语义还原写在 summary 里。

```yaml
- id: x01
  title: ject(扔) 与 port(扛/带) 混淆——"一下离手" vs "一路扛着走"
  type: counter-example
  source_chapter: 字幕 L47-L54（ject 收尾 → port 开篇）
  source_quote: |
    "jet 一扔 一喷 喷射 / port 扔 / 扔是一下离手 / 扔是一路扛着走"
  summary: |
    【推断】作者在引入 port 时立刻拿刚讲完的 ject 做对照。字幕第二个"扔"是同音错字，
    按语义应为"扛/带(port)=一路扛着走"。整句意为"ject 是一下离手，port 是一路扛着走"。
    这是对比暗示的混淆点，不是字面警告。
  failure_mode: |
    只记中文"扔/带"，把 ject（一下离手、投出即不管）和 port（一路扛着走）当成同一动作，
    导致 reject/inject 与 import/export 的动作想象错位。
  mechanism: |
    中文一个"扔/带"字覆盖多个英文动作，学习者用中文标签当锚点，丢失了"动作过程的手感"
    这一区分维度；作者的解法是给每个根一个独立的身体意象（投石机甩石头 vs 人扛货一路走）。
  warning_signs:
    - 说不清 ject 和 port 的动作差别
    - 把 import 想成"往里扔一下"
    - 把 support 想成"扔住"
  bound_to:
    - "近义动作手感辨析"
    - "拆词核心模型"
  tags: [counter-example, near-synonym-confusion, ject, port, inferred]

- id: x02
  title: fer(带) 与 mit(送) 混淆——"跟着走" vs "放手让它去"
  type: counter-example
  source_chapter: 字幕 L88-L128（fer 段 → mit 段）
  source_quote: |
    "for 带 也是承载 传托着货 一路带过去 ... mit 送 也写成miss ... 带是跟着走 送是放手让它去"
  summary: |
    【显式对比，非字面警告】作者明说"带是跟着走，送是放手让它去"，这是全书最清楚的
    X是…Y是… 防混淆句式之一。fer 与 mit 是用户点名的"带vs送"区别。
  failure_mode: |
    把 fer（带，跟着走）和 mit（送，放手让它去）混用，误以为 offer（提供）与 emit（排放）
    都是"拿走/给出去"的同一动作，refer（带回出处）与 transmit（送过去）也分不开。
  mechanism: |
    "带"和"送"在中文里都含"使某物转移"义，差异在施动者是否继续伴随；
    只用中文释义无法编码"是否放手"这一维度，必须靠动作画面区分。
  warning_signs:
    - 分不清 refer（带回出处）与 emit（往外送/排放）
    - 把 submit 想成"带着走"而不是"从下面递上去/把自己交下去"
    - 把 promise 的"送出去"说成"带过去"
  bound_to:
    - "近义动作手感辨析"
    - "拆词核心模型"
  tags: [counter-example, near-synonym-confusion, fer, mit, explicit-contrast]

- id: x03
  title: mit(送) 与 duc(引) 混淆——"送出去就不管" vs "一路领着走"
  type: counter-example
  source_chapter: 字幕 L164-L168（duct 开篇）
  source_quote: |
    "duct ... 也写成duce / 送出去就不管了 / 引是一路领着走"
  summary: |
    【显式对比，非字面警告】作者在讲 duct 时用前一根 mit 做对照："送出去就不管了，引是一路领着走"。
    这是用户点名的"带vs送vs引"三者中的"送vs引"一环。
  failure_mode: |
    把 duc（引，一路领着走）当成 mit（送，放手不管），于是 educate 被想成"把人送出去"
    而不是"把藏在里面的本事引出来"；produce/conduct 的"一路引"感丢失。
  mechanism: |
    两个根都涉及"使某物移动离开原地"，区别在施动者是否全程牵引；中文"送/引"差异细微，
    字幕把 duc 误写成"你"，更说明只能靠动作意象而非汉字标签来记。
  warning_signs:
    - 把 produce 想成"送出去"而不是"水往前引/装甲一路冒出来"
    - 说不出 conduct（导电/带领）的"一路引"感
    - 把 introduce 想成"送进来"
  bound_to:
    - "近义动作手感辨析"
    - "拆词核心模型"
  tags: [counter-example, near-synonym-confusion, mit, duc, explicit-contrast]

- id: x04
  title: fact(做) 与 struct(垒/建) 混淆——"一锤一锤" vs "一块一块往上垒"
  type: counter-example
  source_chapter: 字幕 L195-L236（fact → struct）
  source_quote: |
    "fact 做 铁锤一下一下 把东西做出来 ... struct 键 做是一锤一锤 键是一块一块往上垒"
  summary: |
    【推断】"做是一锤一锤，建(字幕'键')是一块一块往上垒"。作者用对比暗示 fact/struct 易混。
  failure_mode: |
    把 struct（垒/建）当成 fact（做），construct 只记成"做"，丢失"一块块垒起来"的意象，
    destroy（反过来往下拆）也随之失去对照；instruct/obstruct 的根感模糊。
  mechanism: |
    fact 与 struct 中文都可译"做/造"，区别在动作方式（锤击成型 vs 逐块堆叠）；
    中文释义抹平了这种过程差异，只有动作画面能承载。
  warning_signs:
    - 分不清 factory 和 structure 的词根
    - 把 destroy 记成"不好好做"
    - 把 obstruct 想成"做路障"
  bound_to:
    - "近义动作手感辨析"
    - "词族批量记忆法"
  tags: [counter-example, near-synonym-confusion, fact, struct, inferred]

- id: x05
  title: struct(结构) 与 form(型) 混淆——"垒出来" vs "倒进模子"
  type: counter-example
  source_chapter: 字幕 L262-L275（structure → form）
  source_quote: |
    "structure 建起来的样子 结构 ... form 型 累出来的是结构 倒进模子 出来的是型"
  summary: |
    【推断】"垒(字幕'累')出来的是结构，倒进模子出来的是型"。显式对比 struct/form。
  failure_mode: |
    把 form（型/模子）与 struct（结构/垒）混为一谈，transform/reform/conform/uniform 的
    "型"意象被错记成"结构"，platform/formula 的"模子"义也丢失。
  mechanism: |
    两者都表示"做出来的形状"，区别在"逐块垒" vs "倒进模子一次成型"；
    中文"结构/型"不能承载这一区分。
  warning_signs:
    - 把 reform 想成"重新搭结构"而不是"重新塑形"
    - 说不出 uniform"大家都是一个型"的模子意象
  bound_to:
    - "近义动作手感辨析"
    - "拆词核心模型"
  tags: [counter-example, near-synonym-confusion, struct, form, inferred]

- id: x06
  title: form(型) 与 press(压) 混淆——动作意象过渡处的弱信号
  type: counter-example
  source_chapter: 字幕 L271-L306（form → press）
  source_quote: |
    "form 型 ... 倒模子 ... press 压 倒模子靠油 压是硬按下去 印刷机一压 字就上了纸"
  summary: |
    【推断，低置信度】字幕在 form→press 过渡处留有"倒模子…压是硬按下去"的对照痕迹，
    推测作者用"倒模子(成型)" vs "硬按下去(压)"区分 form/press。转写残缺("靠油"疑为错字)，
    证据较弱，仅作候选保留。
  failure_mode: |
    把 press（压/硬按下去）和 form（倒模子成型）当成同一种"使物体成形"的动作，
    express/impress/depress 的"压"感被"型"感覆盖。
  mechanism: |
    两者都是"对物体施力改变形状"，区别在"倒进模子" vs "外部硬按"；一字之差的动作起点不同。
  warning_signs:
    - 把 express 想成"做出一个型"而不是"把里面的东西往外压出来"
    - 把 impress 想成"成型"而不是"往里一压留下印子"
  bound_to:
    - "近义动作手感辨析"
  tags: [counter-example, near-synonym-confusion, form, press, inferred, low-confidence]

- id: x07
  title: press(压) 与 plic/plex(折) 混淆——"往下按" vs "叠起来"
  type: counter-example
  source_chapter: 字幕 L303-L345（press → plic，用户点名的"压vs折"）
  source_quote: |
    "press 压 ... 压是硬按下去 ... click 折 也写成ply 压是往下按 折是叠起来"
  summary: |
    【显式对比，非字面警告】"压是往下按，折是叠起来"。这是用户点名的"压vs折"区别，
    作者用对照防止把 plic 的根义记成 press。
  failure_mode: |
    把 plic/plex（折）当 press（压），complicated 被想成"压得很复杂"而非"一层层折在一起打不开"；
    implicit/explicit/reply/imply 的"折在里面 / 摊开 / 折回去"意象整体丢失。
  mechanism: |
    两者都是"对物体施力使其变形"，区别在"往下按" vs "折叠叠加"；
    中文"压/折"差异需靠动作区分，字幕把 plic 误写成"click"更凸显不能靠标签。
  warning_signs:
    - 把 explicit 记成"压出来"而不是"摊开在外面"
    - 把 imply 的"折在里面"说成"压在里面"
    - 把 multiply 想成"压多次"而不是"一折再折"
  bound_to:
    - "近义动作手感辨析"
    - "拆词核心模型"
  tags: [counter-example, near-synonym-confusion, press, plic, explicit-contrast]

- id: x08
  title: tract(拉) 与 pand(挂) 混淆——"往这边拽" vs "吊着不落地"
  type: counter-example
  source_chapter: 字幕 L379-L421（tract → pand）
  source_quote: |
    "拉 脚盘一圈圈转 绳子绷紧 把十块一路拖过来 ... pand 挂 拉是往这边拽 挂是吊着不落地"
  summary: |
    【推断】"拉是往这边拽，挂是吊着不落地"。显式对比暗示 tract/pand 易混。
  failure_mode: |
    把 pand（挂/吊）当 tract（拉/拽），depend 被想成"拉着你"而非"挂在别人下面、靠着它才不吊"；
    suspend/pending/expend 的"悬吊/秤"意象丢失。
  mechanism: |
    两者都涉及"力作用使物体位置改变"，区别在"往这边拖拽" vs "悬吊不落地"；
    中文"拉/挂"需靠身体感区分。
  warning_signs:
    - 把 suspend 想成"拉住"而不是"从底下吊着、悬在半空"
    - 把 expensive 的"秤出去的多"记成"拉出去的多"
  bound_to:
    - "近义动作手感辨析"
  tags: [counter-example, near-synonym-confusion, tract, pand, inferred]

- id: x09
  title: pand(挂) 与 vert(转) 混淆——"吊着不动" vs "绕轴打转"
  type: counter-example
  source_chapter: 字幕 L468-L472（vert 开篇）
  source_quote: |
    "vert 转 挂是吊着不动 转 是绕着肘打转"
  summary: |
    【推断】"挂是吊着不动，转是绕着(轴)打转"。显式对比暗示 pand/vert 易混。
  failure_mode: |
    把 vert（转）与 pand（挂）混，reverse/convert/divert/universe 的"转"意象被错记成"挂"。
  mechanism: |
    两者都描述物体相对静止/运动的状态，区别在"吊着不动" vs "绕轴旋转"；
    中文需靠动作画面区分，字幕把 vert 写成"转"、pand 写成"挂"恰是好的标签，但学习者常只记中文。
  warning_signs:
    - 把 universe 想成"挂着的一切"而不是"绕一个中心转成一个整体"
    - 把 advertise 的"目光转过来朝着它"记成"挂广告"
  bound_to:
    - "近义动作手感辨析"
  tags: [counter-example, near-synonym-confusion, pand, vert, inferred]

- id: x10
  title: vert(转) 与 rupt(破) 混淆——"绕着转" vs "一下崩开"
  type: counter-example
  source_chapter: 字幕 L509-L514（rupt 开篇）
  source_quote: |
    "rupt 破 转 是绕着转 破 是一下崩开"
  summary: |
    【推断】"转是绕着转，破是一下崩开"。显式对比暗示 vert/rupt 易混。
  failure_mode: |
    把 rupt（破/崩开）当 vert（转），interrupt 被想成"转过去"而非"在中间一下打断"；
    erupt/bankrupt/disrupt/corrupt 的"崩"感丢失。
  mechanism: |
    两者都含"物体状态改变"，区别在"绕轴旋转" vs "一下崩裂"；中文"转/破"差异靠动作区分。
  warning_signs:
    - 把 bankrupt 想成"转成破产"而不是"长凳被砸成两半"
    - 把 corrupt 想成"转坏了"而不是"整个坏透了"
  bound_to:
    - "近义动作手感辨析"
  tags: [counter-example, near-synonym-confusion, vert, rupt, inferred]

- id: x11
  title: rupt(破) 与 clud(关) 混淆——"崩开" vs "合上"
  type: counter-example
  source_chapter: 字幕 L548-L551（clud 开篇）
  source_quote: |
    "clud 关 破是崩开 关是和尚 两扇大门一合"
  summary: |
    【推断】"破是崩开，关是合(字幕'和尚'为'合上'同音错字)"。显式对比暗示 rupt/clud 易混。
  failure_mode: |
    把 clud（关）当 rupt（破），include/exclude/conclude/disclose/exclusive 的"关门"意象被记成"破开"。
  mechanism: |
    两者中文都可表"使物体分开/闭合的状态变化"，区别在"崩开" vs "合拢"；
    中文释义易混，需靠"两扇大门一合"的画面固化。
  warning_signs:
    - 把 exclude 想成"破出去"而不是"关在外面"
    - 把 conclude 记成"破到此为止"而不是"门一扇扇全关上"
  bound_to:
    - "近义动作手感辨析"
  tags: [counter-example, near-synonym-confusion, rupt, clud, inferred]

- id: x12
  title: cept(拿) 与 ten(握) 混淆——"一下抓起" vs "攥着不松"
  type: counter-example
  source_chapter: 字幕 L583-L629（cept → ten）
  source_quote: |
    "cept 拿 铁钳往下一探 一合 把铜币拿了起来 ... tane 握 拿是一下抓起 握是钻着不松"
  summary: |
    【推断】"拿是一下抓起，握是钻(攥)着不松"。显式对比暗示 cept/ten 易混。
  failure_mode: |
    把 ten（握/攥着不松）当 cept（拿/一下抓起），maintain/contain/retain/sustain/detain 的
    "持续握持"意象丢失，被错记成"拿一次"。
  mechanism: |
    两者都是"手获取物体"，区别在"一下抓起即放" vs "持续攥住不松"；
    中文"拿/握"差异需靠动作过程区分。
  warning_signs:
    - 把 retain 想成"再拿一次"而不是"往回握住"
    - 把 sustain 的"从下面一直拖住"记成"拿住"
  bound_to:
    - "近义动作手感辨析"
    - "词族批量记忆法"
  tags: [counter-example, near-synonym-confusion, cept, ten, inferred]

- id: x13
  title: ten(握) 与 pos(放) 混淆——"攥着不松" vs "撒手"
  type: counter-example
  source_chapter: 字幕 L661-L666（pos 开篇）
  source_quote: |
    "pos 放 握 是钻着不松 放 是撒手"
  summary: |
    【推断】"握是钻(攥)着不松，放是撒手"。显式对比暗示 ten/pos 易混——两者恰是相反动作，
    却被放在相邻位置讲解，正是易混信号。
  failure_mode: |
    把 pos（放/撒手）与 ten（握/不松）混，deposit（放下去/存款）被想成"握住"；
    propose/expose/postpone/compose/oppose 的"放"感被"拿"感覆盖。
  mechanism: |
    两者是手的相反动作，中文"放/握"反义明显，但学习者常只记"手与物接触"的笼统意象而混；
    作者用"旗子一落就有了位置"给 pos 独立画面。
  warning_signs:
    - 把 expose 想成"握住给别人看"而不是"放到外面谁都看得见"
    - 把 oppose 的"对着放"记成"对着握"
  bound_to:
    - "近义动作手感辨析"
  tags: [counter-example, near-synonym-confusion, ten, pos, inferred]

- id: x14
  title: pos(放) 与 tend(伸) 混淆——"放下不动" vs "往外撑开"
  type: counter-example
  source_chapter: 字幕 L705-L708（tend 开篇）
  source_quote: |
    "tend 深 放是放下不动 深是往外撑开"
  summary: |
    【推断】"放是放下不动，伸(字幕'深')是往外撑开"。显式对比暗示 pos/tend 易混。
  failure_mode: |
    把 tend（伸/撑开）当 pos（放/不动），extend/attend/pretend/intend/tension/tendency 的
    "往外伸"意象丢失；pretend 被想成"放个假的"而不是"把假布景伸在前面"。
  mechanism: |
    两者都涉及"物体位置/状态改变"，区别在"放下静止" vs "向外撑开延展"；
    中文"放/伸"需靠动作区分。
  warning_signs:
    - 把 pretend 想成"放个假的"
    - 把 tension 的"绷紧/风景(紧张)"记成"放下"
    - 说不出 tendency"一直往一边伸"的方向感
  bound_to:
    - "近义动作手感辨析"
  tags: [counter-example, near-synonym-confusion, pos, tend, inferred]

- id: x15
  title: tend(伸) 与 sist(站) 混淆——"往外撑" vs "立住不动"
  type: counter-example
  source_chapter: 字幕 L743-L746（sist 开篇）
  source_quote: |
    "sist 站 深是往外撑 站是力助不动"
  summary: |
    【推断】"伸(深)是往外撑，站是着(力)立(字幕'力助')不动"。显式对比暗示 tend/sist 易混。
  failure_mode: |
    把 sist（站/立住不动）当 tend（伸/撑开），resist/persist/assist/consist/exist/substitute/distant 的
    "顶住不动/站住"意象丢失。
  mechanism: |
    两者都描述"力量的施加与位置状态"，区别在"向外撑开" vs "立住不动"；
    中文"伸/站"差异靠动作区分。
  warning_signs:
    - 把 assist 想成"伸过去"而不是"站到旁边帮忙"
    - 把 consist 的"站到一起"记成"伸到一起"
    - 把 resist 的"顶着往回站住一步不退"记成"往外撑"
  bound_to:
    - "近义动作手感辨析"
  tags: [counter-example, near-synonym-confusion, tend, sist, inferred]

- id: x16
  title: gress(走) 与 grad(迈台阶) 混淆——"一路往前" vs "一步一击台阶"
  type: counter-example
  source_chapter: 字幕 L827-L833（gress 开篇）
  source_quote: |
    "gress 脉 也写成 grad greed 走是一路往前 脉是一步一击台阶"
  summary: |
    【推断】"走(gress/ced)是一路往前，迈(字幕'脉'/grad)是一步一击(级)台阶"。显式对比暗示 gress/grad 易混。
  failure_mode: |
    把 gress（走/一路往前）与 grad（迈台阶/一级级）混，progress/graduate/grade/gradual/degree/aggressive 的
    "一级级"意象丢失；aggressive 被想成"一路走"而不是"冲着对方迈过去"。
  mechanism: |
    两者都表示"移动前进"，区别在"连续走" vs "逐台阶迈"；中文"走/迈"需靠动作节奏区分。
  warning_signs:
    - 把 gradual 想成"一直走"而不是"一级一级"
    - 把 degree 的"一击一击的刻度"记成"一路走"
  bound_to:
    - "近义动作手感辨析"
  tags: [counter-example, near-synonym-confusion, gress, grad, inferred]

- id: x17
  title: gress/迈 与 ven(来) 混淆——"自己往上走" vs "从远处到这"
  type: counter-example
  source_chapter: 字幕 L866-L872（ven / then 开篇）
  source_quote: |
    "then 来 也写成 vent 脉是自己往上走 来 是从远处到这"
  summary: |
    【推断】"迈(脉/gress)是自己往上走，来(ven)是从远处到这"。显式对比暗示 gress/ven 易混。
  failure_mode: |
    把 ven（来/从远处到近处）与 gress（自己一路往前/往上）混，invent/prevent/revenue/convene/adventure/convenient/avenue 的
    "到来"意象丢失；prevent 被想成"提前走"而不是"抢先一步来挡在前面"。
  mechanism: |
    两者都表示"移动接近"，区别在运动方向和参照点（自己走 vs 从远处到来）；
    中文"来/走"需靠方向感区分。
  warning_signs:
    - 把 prevent 想成"提前走"
    - 把 revenue 的"钱花出去又回来了"记成"钱走回来"
    - 把 convenient 的"来的正合适"记成"走到合适"
  bound_to:
    - "近义动作手感辨析"
  tags: [counter-example, near-synonym-confusion, gress, ven, inferred]

- id: x18
  title: ven(来) 与 cur(跑) 混淆——"到了就停" vs "一刻不停"
  type: counter-example
  source_chapter: 字幕 L909-L914（cur 开篇）
  source_quote: |
    "cur 跑 水跑起来 就是流 来是到了就停 跑是一刻不停"
  summary: |
    【推断】"来是到了就停，跑(cur)是一刻不停"。显式对比暗示 ven/cur 易混。
  failure_mode: |
    把 cur（跑/一刻不停）当 ven（来/到了就停），current/currency/recur/occur/excursion/course 的
    "持续流动"意象丢失；occur 被想成"来到"而不是"迎面跑到你跟前"。
  mechanism: |
    两者都表示"移动"，区别在"到点即停" vs "持续不停"；中文"来/跑"需靠动作持续性区分。
  warning_signs:
    - 把 occur 想成"来到"而不是"迎面跑到跟前"
    - 把 currency 的"流通的东西"记成"来来的东西"
    - 把 recur 的"又跑回来"记成"又回来"
  bound_to:
    - "近义动作手感辨析"
  tags: [counter-example, near-synonym-confusion, ven, cur, inferred]

- id: x19
  title: 同一词根动作感漂移——"一个根=一个固定中文动作"的隐含陷阱
  type: counter-example
  source_chapter: 字幕 L583-L625（cept/cap 词族；参照 BOOK_OVERVIEW 批判节）
  source_quote: |
    "cept 拿 铁钳往下一探 一合 把铜币拿了起来 ... perceive 一把抓住 察觉 ... capture 抓住 捕获
     capable 拿得住 有能力的 ... participate 拿一份 参与"
  summary: |
    【推断，来自字幕内证 + 全局批判】同一个 cap/cept 根，字幕给出的中文标签从"拿"漂移到
    "抓住/拿得住/拿一份/容纳"。作者默认"一个根配一个具象动作"，但同一根在不同词里动作感会漂移，
    这是方法论本身暗藏的误读风险，非作者明说的警告。
  failure_mode: |
    学习者把"一个根=一个固定动作"绝对化，遇到 cap/cept 在 perceive/capable/participate 中的语义漂移时，
    强行套用"拿"的画面，反而产生牵强的理解；同理 object(物体/反对)、effect(效果/影响) 的动作感很勉强。
  mechanism: |
    作者的方法是教学助记法而非严格词源学；词根在历史中发生语义漂移，"动作画面"只是后人重包装的入口，
    把助记意象当成词的真实义项来源，会在不透明词上失效。
  warning_signs:
    - 给 object/effect 硬编"扔出去"的故事却讲不通
    - 发现同一根需要两三个不同中文动词才能解释
    - 拆出来的动作感和词典释义对不上
  bound_to:
    - "拆词核心模型"
    - "生词现场拆解流程"
    - "词族批量记忆法"
  tags: [counter-example, root-sense-drift, method-limit, inferred]
```

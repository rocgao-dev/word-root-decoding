# 案例提取候选池（case-extractor 产出）

> 来源：3602a2da_VID_1178.txt（1035 行视频字幕）。语音转写同音错字按语义还原（磁=词、磁根=词根、前坠=前缀、意=词缀、rat=re、bin=in、x=ex、then=down 等）。
> 本文件只做候选提取，不做筛选（宁错杀）。每条为代表案例组，非 191 词穷举。

```yaml
- id: c01
  title: ject（扔）词族——开篇最完整的「一根推多词」演示
  type: case
  source_chapter: 字幕行 10–50（ject 扔 / 投石机一甩）
  source_quote: |
    "扔，投石机一甩，石头离手，飞出去就不管了。re(往回)：别人递过来你又扔回去，就是 reject，拒绝；in(向里)扔进身体，inject，注射；ex(向外)扔出来，eject，弹出；pro(向前)把计划往前扔出去就是 project，项目；把光往前扔上幕布是投影；object 迎面扔来打不着，物体、反对；adjective 扔在名词旁边，形容词；trajectory 扔出的线，轨迹。"
  summary: |
    遇到什么问题：reject/inject/eject/project/object 等一串以 ject 开头的词，孤立死记记不住。
    怎么用方法：先定动作根 ject=扔（画面：投石机一甩、石头离手、飞出去就不管了），再逐个叠加方向前缀，读「动作被方向修饰后的结果」。
    得出什么词义：re(回)扔回去=拒绝；in(里)扔进身体=注射；ex(外)扔出来=弹出；pro(前)往前扔=项目/投影；ob(迎面)扔来打不着=物体/反对；ad(旁边)扔在名词旁=形容词；tra(线)扔出的线=轨迹。
  bound_to:
    - "拆词核心模型：词 = 动作(词根) + 方向(前缀)"
    - "词族批量记忆：一个动作根配不同方向生成一串词"
  outcome: |
    一个根当场推出 7 个词，作为全片第一个演示确立了「词=动作+方向」模型，后续 24 根均照此套路展开。
  tags: [case, ject, 词族, 开篇演示, 核心模型]

- id: c02
  title: port（扛）词族与「扔 vs 扛」手感区分
  type: case
  source_chapter: 字幕行 51–86（port 扛 / 扔是一下离手，扛是一路扛着走）
  source_quote: |
    "port：扔是一下离手，扛是一路扛着走。im(往里)import 进口；x(往外)export 出口；sub(从下面拖着)support 支持；rat(往回)把消息一路带回来就是 report 报告；transport 跨过去，运输；portable 扛得动，便携；passport 过港口用的，护照；portfolio 随身扛的，作品集。"
  summary: |
    遇到什么问题：ject 和 port 都像「扔/带」，近义动作如何区分？十几个 port 词如何批量记？
    怎么用方法：先用「手感」划清边界——"扔是一下离手，扛是一路扛着走"，port 定为扛着走；再叠加方向前缀读义。
    得出什么词义：im(里)=进口；ex(外)=出口；sub(下)从下面拖住=支持；re(回)一路带回来=报告；trans(跨)=运输；portable=便携；passport=护照。
  bound_to:
    - "近义动作手感辨析：扔(一下离手) vs 扛(一路扛着走)"
    - "词族批量记忆：一个动作根配不同方向生成一串词"
  outcome: |
    用「手感」把两个近义根彻底分开，并一口气带出 8 个 port 词，证明方法可从单根扩展到成族记忆。
  tags: [case, port, 手感辨析, 词族]

- id: c03
  title: fer / mit / duc（带·送·引）三根手感辨析
  type: case
  source_chapter: 字幕行 87–194（fer 带 / mit 送 / duct 引）
  source_quote: |
    "带是跟着走，送是放手让它去。fer(带)：ob(朝着)把东西带到你面前就是 offer 提供；this(分开)两条船往两边带就是 differ 不同；sub(下面)在底下扛住重担就是 suffer 遭受。mit(送)：sub(下面)从下面递上去 submit 提交；pro(向前)先送出去，以后再办，promise 承诺；per(穿过)放它过去 permit 允许。duc(引)：送出去就不管了，引是一路领着走；pro(向前)水往前引 produce 生产；e(向外)把藏在里面的本事引出来 educate 教育；con(一起)电线把电引过去 conduct 导电。"
  summary: |
    遇到什么问题：带(fer)、送(mit)、引(duc) 三个近义根极易混，offer/promise/produce 等词释义牵强。
    怎么用方法：不靠中文翻译，靠动作过程的身体感——"带是跟着走（人跟着货），送是放手让它去，引是一路领着走（像领人走路）"；再配方向。
    得出什么词义：fer：ob→提供、dis→不同、sub→遭受/受苦、re→更喜欢/参考、trans→转移；mit：sub→提交/服从、pro→承诺、per→允许、ad→准入、trans→传送、e→排放、dis→解散、mission→使命；duc：pro→生产/产品、e→教育、con→导电/进行、intro→介绍、aqueduct→渡槽。
  bound_to:
    - "近义动作手感辨析：带 vs 送 vs 引"
    - "词族批量记忆：一个动作根配不同方向生成一串词"
  outcome: |
    三根各带一词族，用「跟着走/放手去/领着走」三分手感，把最容易混的一组根拆开，同时覆盖约 25 个高频词。
  tags: [case, fer, mit, duct, 手感辨析, 词族]

- id: c04
  title: fact（做）/ struct（垒）词族与「做 vs 垒」手感区分
  type: case
  source_chapter: 字幕行 195–270（fact 做 / struct 垒）
  source_quote: |
    "fact：做，铁锤一下一下把东西做出来。x(向外)做出来的结果 effect 效果；per(到底)从头做到尾一点不差 perfect 完美；manu 是手，用手做 manufacture 制造；factory 做东西的地方，工厂；defect 做出来少了一块，缺陷。struct：做是一锤一锤，垒是一块一块往上垒；con(一起)一块块垒起来 construct 建造；反过来往下拆 destroy 摧毁；in(向里)照着图纸一步步往里搭 instruct 指导，说明书叫 instruction。"
  summary: |
    遇到什么问题：fact=做 与 struct=垒 都是「造东西」，effect/perfect/manufacture 与 construct/destroy 分不清。
    怎么用方法：抓手感差异——"做是一锤一锤（敲打成形），垒是一块一块往上垒（堆叠）"；struct 反向即"往下拆"。再配方向前缀。
    得出什么词义：fact：ex→效果、ad→影响(affect)、per→完美、manu+fact→制造、defect→缺陷、efficient→高效、artificial→人造；struct：con→建造、de→摧毁、in→指导/说明书、instrument→工具/乐器、structure→结构、obstruct→阻碍、infrastructure→基础设施。
  bound_to:
    - "近义动作手感辨析：做(一锤一锤) vs 垒(一块块往上垒)"
    - "词族批量记忆：一个动作根配不同方向生成一串词"
  outcome: |
    用「敲打 vs 堆叠」区分两个高频「造」根，并借"往下拆"顺势带出 destroy，展示反向前缀的推导力。
  tags: [case, fact, struct, 手感辨析, 词族]

- id: c05
  title: press（压）/ plic（折）词族与「压 vs 折」手感区分
  type: case
  source_chapter: 字幕行 303–378（press 压 / click-plic 折）
  source_quote: |
    "press：倒模子靠油，压是硬按下去，印刷机一压字就上了纸。x(向外)把里面的东西往外压出来就是 express 表达；in(向里)往里一压留下一个印子就是 impress 给人留下印象；then(向下)一直往下压，压得人低落 depress 沮丧；compress 压缩；suppress 抑制。click(折，也写成 ply)：压是往下按，折是叠起来；com(一起)一层层折在一起打都打不开 complicated 复杂；in(向里)折在里面 implicit 含蓄；ex(向外)摊开在外面 explicit 明确。"
  summary: |
    遇到什么问题：press 与 plic/ply 都是「使形变」，express/impress 与 complicated/explicit 如何记牢？
    怎么用方法：先分手感——"压是往下按（硬按下去），折是叠起来（一层层）"，并用"印刷机一压字就上纸"坐实 press 的画面；再读方向。
    得出什么词义：press：ex→表达、in→留下印象、down→沮丧、compress→压缩、suppress→抑制、repress→克制、espresso→浓缩咖啡；plic：com→复杂、in→含蓄、ex→明确、re→回复、im→暗示、multi→倍增、du→复制、dis→展示。
  bound_to:
    - "近义动作手感辨析：压(往下按) vs 折(叠起来)"
    - "词族批量记忆：一个动作根配不同方向生成一串词"
  outcome: |
    用一组生活意象（印刷机、叠纸、浓缩咖啡）把压/折两族十几个抽象词具象化，印证「动作画面优于抽象释义」。
  tags: [case, press, plic, 手感辨析, 词族]

- id: c06
  title: tract（拉）/ pend（挂）词族与「拉 vs 挂」手感区分
  type: case
  source_chapter: 字幕行 379–467（拉/tract / pand-pend 挂）
  source_quote: |
    "拉：脚盘一圈圈转，绳子绷紧，把石块一路拖过来。at(朝着)拉过来 attract 吸引；diss(分开)拉到一边 distract 使分心；com(一起)两头往中间一拉 contract 收缩，把双方拉到一起盖上印就是合同；abs(离开)从一大堆具体的东西里把要点拉出来 abstract 抽象的。pand(挂)：拉是往这边拽，挂是吊着不落地；d(向下)挂在别人下面靠着它才不吊 depend 依靠；前面加 in 不挂在谁下面 independent 独立；sus(在下面)从底下吊着 suspend 悬挂/暂停。"
  summary: |
    遇到什么问题：拉(tract)与挂(pend)方向感相近，contract/abstract/depend/expensive 等词义跳跃。
    怎么用方法：分手感——"拉是往这边拽（绳子绷紧拖过来），挂是吊着不落地（秤上、秤出去）"；再叠加方向，注意 abstract 是从具体里"拉出要点"、contract 是"拉到一起盖章成合同"。
    得出什么词义：tract：at→吸引、dis→分心、con→收缩/合同、abs→抽象的、ex→提取、sub→减去、tractor→拖拉机；pend：de→依靠、in→独立、sus→悬挂/暂停、ex(秤出去的多)→昂贵的、spend→花费、pending→待定、appendix→附录、compensate→补偿。
  bound_to:
    - "近义动作手感辨析：拉(往这边拽) vs 挂(吊着不落地)"
    - "词族批量记忆：抽象词由具象动作+方向推导"
  outcome: |
    把 contract"合同"、abstract"抽象"、expensive"昂贵"这类语义漂移词还原为可想象的动作，扩展了方法的适用边界。
  tags: [case, tract, pend, 手感辨析, 词族, 语义漂移]

- id: c07
  title: vert（转）/ rupt（破）词族与「转 vs 破」手感区分
  type: case
  source_chapter: 字幕行 468–547（vert 转 / rupt 破 / root 路线）
  source_quote: |
    "vert：挂是吊着不动，转是绕着轴打转，水车一转整条水道都动起来。ray(往回)转过头沿路往回走 reverse 倒转/相反的；add(朝着)让你的目光转过来朝着它 advertise 做广告；unit(一)万物绕着一个中心转成一个整体 universe 宇宙；convert 整个转过去，转换；diverse 转向四面八方，多样的。rupt：转是绕着转，破是一下崩开，石头裂开一道缝；意(向外)从里面破开冲出来 erupt 爆发/火山喷发；inter(中间)在中间一下打断 interrupt 打断；bankrupt 放债人的长凳被砸成两半，破产。"
  summary: |
    遇到什么问题：转(vert/vers)与破(rupt)都是「变化」，universe/diverse/erupt/bankrupt 记不牢。
    怎么用方法：分手感——"转是绕着轴打转（水车），破是一下崩开（石头裂缝）"；rupt 一词用"放债人的长凳被砸成两半"的具象故事钉住 bankrupt。再配方向。
    得出什么词义：vert：re→倒转/相反、ad→做广告、un→宇宙、con→转换、di→改道、version→版本、diverse→多样的、versatile→多才多艺；rupt：ex→爆发/火山喷发、inter→打断、bank→破产、dis→扰乱、cor→腐败、ab→突然的、route→路线。
  bound_to:
    - "近义动作手感辨析：转(绕轴打转) vs 破(一下崩开)"
    - "词族批量记忆：用具象小故事钉住语义漂移词"
  outcome: |
    "长凳砸成两半=破产"等故事化意象成为最强记忆锚点，展示方法处理难词（bankrupt/erupt）的能力。
  tags: [case, vert, rupt, 手感辨析, 词族, 故事化意象]

- id: c08
  title: spect（看）词族——respect / suspect / retrospect 等「看」的方向链
  type: case
  source_chapter: 字幕行 945–996（spect 看）
  source_quote: |
    "看：一路走、迈、来、跑，最后停下来看。ray(回)走过去了又回头再看一眼，就是 respect 尊重；so(从下面)从下往上打量就是 suspect 怀疑；per(穿过)穿过窗框看出去 perspective 视角，画画里叫透视；inspect 往里看，检查；expect 往外看，盼着期待；prospect 往前看，前景；aspect 朝一面看，方面；spectator 看的人，观众；retro(往后)往回看一眼，就是 retrospect 回顾。"
  summary: |
    遇到什么问题：respect/suspect/perspective/prospect/retrospect 等一堆"看"词方向各异，难以区分。
    怎么用方法：先立根 spect=看，并铺一段动作链"走、迈、来、跑，最后停下来看"做画面铺垫；再读前缀方向——回看/下看/穿看/里看/外看/前看/后看。
    得出什么词义：re(回)→尊重；sub(下)→怀疑；per(穿)→视角/透视；in→检查；ex→期待；pro→前景；a(朝一面)→方面；spectator→观众；retro(后)→回顾。
  bound_to:
    - "词族批量记忆：一个动作根配不同方向生成一串词"
    - "拆词核心模型：前缀=空间/逻辑方向"
  outcome: |
    一个"看"根串起 9 个词，并把"前缀一律当方向"的简化用法展示到极致（retrospect 回顾为用户点名的代表例）。
  tags: [case, spect, 词族, 方向前缀, 代表案例]

- id: c09
  title: 结尾三道自测题——intercept / deport / convene 现场迁移验证
  type: case
  source_chapter: 字幕行 1000–1024（最后三道题，都是没讲过的词）
  source_quote: |
    "最后三道题，都是没讲过的词，你自己拆，答案先打在弹幕里。inter(中间)+sept(拿)：半路拿走 intercept 拦截；de(离开)+port(搬)：搬走 deport 驱逐出境；con(一起)+vane(来)：来到一起 convane 召集、开会。"
  summary: |
    遇到什么问题：三个从未讲过的生词 intercept/deport/convene，能否不靠死记现场推出词义？
    怎么用方法：完整套用"先找动作 → 再看方向 → 组合词义"流程——先在词里定位已学的动作根（cept 拿、port 搬、vent 来），再读前缀方向（inter 中间、de 离开、con 一起）。
    得出什么词义：inter(中间)+cept(拿)=半路拿走=拦截；de(离开)+port(搬)=搬走=驱逐出境；con(一起)+vent(来)=来到一起=召集/开会。
  bound_to:
    - "生词现场拆解流程：先找动作 → 再看方向 → 组合词义"
    - "方法可迁移性验证：用未学过的词当场套用"
  outcome: |
    三题全部当场拆出，作为方法论有效的收尾证据；作者称学习者已"把 191 个词从头拆到尾、一个都没死记，记住的是 25 个动作"，下次遇生词仍可现场推导。
  tags: [case, 自测题, 迁移验证, intercept, deport, convene, 收尾]

- id: c10
  title: pos（放）/ tend（撑开）词族——「求婚」「帐篷」等生活场景释义
  type: case
  source_chapter: 字幕行 661–742（pos 放 / tend 撑开）
  source_quote: |
    "pos：握是攥着不松，放是撒手，旗子一落就有了位置。pro(向前)把想法放到面前就是 propose 提议；把戒指放到面前就是求婚；x(向外)放到外面谁都看得见 expose 暴露；post(往后)往后放一放 postpone 推迟。tend：放是放下不动，深是往外撑开，绳子一拉帐篷就撑起来了；x(向外)越撑越长 extend 延长；at(朝着)把注意力伸过去 attend 出席/照料；pre(前面)把一块假布景撑在前面 pretend 假装。"
  summary: |
    遇到什么问题：放(pos)与伸(tend)手感相近，propose/expose/attend/pretend 等词抽象难记。
    怎么用方法：分手感——"放是撒手（旗子一落有了位置），深/伸是往外撑开（绳子一拉帐篷撑起来）"；再用生活场景落义，如"把戒指放到面前=求婚"。
    得出什么词义：pos：pro→提议/求婚、ex→暴露、post→推迟、position→位置、com→组成、im→强加、op→反对、deposit→存款；tend：ex→延长、at→出席/照料、pre→假装、intend→打算、tension→紧张、tendency→趋势、tent→帐篷。
  bound_to:
    - "近义动作手感辨析：放(撒手) vs 伸(往外撑开)"
    - "词族批量记忆：用生活场景为抽象词落义"
  outcome: |
    "求婚""帐篷"两个生活画面分别钉住 propose 与 tend 的核心手感，展示方法用已知生活经验解释抽象词的贴近性。
  tags: [case, pos, tend, 手感辨析, 生活场景, 词族]
```

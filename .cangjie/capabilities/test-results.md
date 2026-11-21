# 阶段 4 压力测试结果 — word-root-decoding

- **测试方式**: 独立 sub-agent 盲测（未参与蒸馏、看不到 type/expected_behavior/notes，只拿到 skill name + description + 4 张卡的 description + 10 条纯 prompt）
- **测试时间**: 2026-11-21
- **总通过率**: 10/10 = 100% → 接受，无需回炉

## 逐条判卷

| # | 类型 | prompt 摘要 | 盲测 would_trigger / card | 预期 | 判定 |
|---|---|---|---|---|---|
| 1 | should_trigger | reject 为什么是拒绝 | yes / word-decoding-core | 激活并拆 re+ject | ✅ |
| 2 | should_trigger | 生词怎么现场推断 | yes / word-decode-flow | 激活走 flow 流程 | ✅ |
| 3 | should_trigger | ject vs port 区别 | yes / root-feel-discrimination | 激活手感辨析 | ✅ |
| 4 | should_trigger | 按词根批量记 spect 词族 | yes / word-family-scaling | 激活词族扩展 | ✅ |
| 5 | should_not_trigger | 查 phenomenon 释义音标 | no / none | 不激活（纯查词+非系统词） | ✅ |
| 6 | should_not_trigger | Python 的 prefix 参数 | no / none | 不激活（编程语境） | ✅ |
| 7 | should_not_trigger | 英语词 Word 文档排版 | no / none | 不激活（任务无关） | ✅ |
| 8 | edge_case | effect 怎么拆（拆不动） | yes / core，且指出 fect 存疑牵强 | 可激活但须判停/标注存疑 | ✅ |
| 9 | edge_case | telephone / tele 怎么拆 | no，指出希腊根排除 | 超范围不硬拆 | ✅ |
| 10 | edge_case | photo/tele/geo 总结 | no | 超范围不硬套 | ✅ |

## 关键结论
- **触发精度**: 4 条正向全部精准命中预期卡片，4 张卡的 description 区分度良好，无互相抢调用。
- **诱饵零误触发**: 3 条 should_not_trigger 全部正确忍住（含 1 条关键词 prefix 跨领域诱饵）。
- **边界处理**: 3 条 edge 全部正确识别希腊词根/语义漂移词的边界，其中 effect 用例盲测agent主动标注"存疑牵强"，与 B 段判停条件一致。
- **4 张卡路由**: 每张卡都被独立命中一次，验证了 single 入口内部路由表的有效性。

## 判定
100% 通过，达到接受阈值（100% → 直接接受）。无需回炉重做阶段 2。

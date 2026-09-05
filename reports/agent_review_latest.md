# C2-A 只读交易员治理 Agent 评审

> **PAPER_ONLY · 只读治理 · 不生成信号 · 不下单 · 不构成交易指令**

- 证据状态 / 公开发布决定：可用 / `FAIL`
- 私有源评审决定：`FAIL`
- 首要阻断：`STRICT_REPORT_READY`
- 硬门槛通过：`2 / 18`
- 数据 / 因果 / 对账：`DATA_NOT_READY / False / True`
- 策略版本 / 参数：`v1.3-causal / 不可用`
- 权限边界：Agent 只读审查研究、因果、对账与风险证据；不参与确定性信号计算，不修改账本，也不能提交订单。
- 公开证据边界：完整源报告只留在私有链；本公开包没有外部签名锚，不能独立授权 `REVIEW_REQUIRED`。

## 未通过的硬门槛

- `STRICT_REPORT_READY`
- `PARAMETER_SPACE_720`
- `RESEARCH_DESIGN`
- `CONTROL_SUITE`
- `EMBARGO_SENSITIVITY`
- `STRICT_DATA`
- `CAUSALITY_AUDIT`
- `OOS_INDEPENDENT_DAYS`
- `OOS_TRADE_COUNT`
- `PROFITABLE_OUTER_FOLD_RATE`
- `NET_EXCESS_LCB95`
- `WHITE_REALITY_CHECK`
- `STRESS_MATRIX_27`
- `TWO_X_COST_NONNEGATIVE`
- `TOP3_PROFIT_CONCENTRATION`
- `FORWARD_PAPER_DAYS`

公开 JSON 已移除源报告路径和生成时间，仅保留白名单证据状态、版本指纹与决定。
完整研究证据只存在于私有链，因此公开 `decision / promotion_gate` 永远为 `FAIL`。
完整机器可读摘要见 `../data/agent_review_latest.json`。

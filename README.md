# C2-A v1.3 PAPER_ONLY 结果

本仓库只发布经过白名单脱敏的自动运行状态。**不连接券商、不支持实盘、不构成收益承诺。**

## 当前阶段

当前为 `SHADOW_ONLY_ROOT_DISK`：仅验证分钟数据可用性与因果时间，不创建模拟账户，不生成信号、订单、持仓或收益。

部署完成后的入口：

- 最新 Shadow 状态：`status/shadow/README.md`
- 结构化状态：`status/shadow/latest.json`
- 每日不可变证据：`status/shadow/daily/`

正式 PAPER 阶段需要独立持久卷、严格数据源和两个真实交易日验收，并需再次人工确认。公开仓库届时仍只展示账户级收益汇总；股票代码、具体持仓和逐笔交易不会公开。

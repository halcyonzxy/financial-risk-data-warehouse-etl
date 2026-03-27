# 📊 Financial Risk Data Warehouse ETL  
企业级金融风控数仓 ETL 项目 | ODS–DWD–DWS 分层架构

---

## 🚀 Project Overview

本项目是企业级金融风控数仓 ETL 全流程解决方案，基于 ODS → DWD → DWS 标准数仓分层架构构建，专为期货 / 信贷类风控场景量身设计。
项目从真实业务需求出发，完成数据模型重构、数据清洗逻辑、统一指标口径、全链路数据监控体系建设，达到可直接上线的生产级标准。

---

## ⭐ Key Features

- 标准数仓分层（ODS → DWD → DWS）
- 全表主键约束（保证数据唯一性）
- ETL 幂等性（支持重复执行 / 补数据）
- 真实业务指标（PnL / 持仓 / 风险敞口）
- 数据质量监控（缺失 / 异常 / 重复）
- 风控体系（信用风险 / 市场风险 / 持仓风险）
- 无硬编码，口径可追溯，可审计

---

## 🏗️ Architecture

### ODS
- 客户信息
- 交易流水
- 市场指标

### DWD
- 去重 / 清洗 / 标准化
- 异常数据分流

### DWS
- 指标聚合
- 风控输出
- 数据质量报告

---

## ⚙️ Core Tables

- dws_business_indicators：客户 - 品种日频业务指标表
- 持仓量、成交量、真实盈亏、信用等级、风险敞口
- dws_risk_monitoring：业务风险监控表
- 客户信用风险、市场指标超标风险、大额持仓风险
- dws_data_quality_summary：数据质量异常明细表
- 缺失客户 ID、金额不一致、交易量异常、重复交易
- dwd_futures_trade_exceptions：交易异常明细清单

---

## 🛠️ Tech Stack

- MySQL 8.0+
- SQL（窗口函数）

---

## ⚡ Quick Start

```sql
USE XXX;
```

---



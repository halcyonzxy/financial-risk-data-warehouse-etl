# 📊 Financial Risk Data Warehouse ETL  
企业级金融风控数仓 ETL 项目 | ODS–DWD–DWS 分层架构

---

## 🚀 Project Overview

本项目构建了一套企业级金融风控数据仓库 ETL 全流程解决方案，基于 ODS → DWD → DWS 分层架构，面向期货 / 信贷风控场景。

---

## ⭐ Key Features

- 标准数仓分层（ODS → DWD → DWS）
- 全表主键约束（保证数据唯一性）
- ETL 幂等性（支持重复执行 / 补数据）
- 真实业务指标（PnL / 持仓 / 风险敞口）
- 数据质量监控（缺失 / 异常 / 重复）
- 风控体系（信用风险 / 市场风险 / 持仓风险）
- 无硬编码，口径可追溯

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

- dws_business_indicators
- dws_risk_monitoring
- dws_data_quality_summary
- dwd_futures_trade_exceptions

---

## 🛠️ Tech Stack

- MySQL 8.0+
- SQL（窗口函数）

---

## ⚡ Quick Start

```sql
CREATE DATABASE risk_dw;
SOURCE project_main.sql;
```

---

## 🎯 Use Cases

- 金融风控
- 数据仓库建设
- ETL 面试项目


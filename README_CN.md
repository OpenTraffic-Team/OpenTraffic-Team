<div align="right">

**中文** | [**English**](README.md)

</div>

<div align="center">

# 🚦 OpenTraffic

### 智能交通开源基础设施社区

为未来城市交通构建一体化的 **感知 · 决策 · 控制 · 部署基础设施**。

</div>
<div align="center">

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg?style=for-the-badge)](LICENSE)
[![HuggingFace](https://img.shields.io/badge/🤗%20HuggingFace-Models-FFD21E?style=for-the-badge)](https://huggingface.co/OpenTraffic)
[![X](https://img.shields.io/badge/X-Follow-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/OpenTraffic_CN)
[![WeChat](https://img.shields.io/badge/WeChat%20Group-07C160?style=for-the-badge&logo=wechat&logoColor=white)](https://github.com/OpenTraffic-Team/OpenTraffic-TSC-Engine/blob/main/pic/wechat.jpg)

</div>

---

# 🌍 概述

OpenTraffic 是面向智能交通系统的开源基础设施项目，专注于构建：

* 🚗 交通感知
* 🚦 信号控制
* 🧠 强化学习与智能决策 (RL / Agent)
* ⚙️ 边缘计算与系统部署 (Ops)

基于**分层 Agent 架构，感知与控制双栈并行**。

---

# ⚙️ 核心平台

## 🧩 OpenTraffic-Ops (平台层)
👉 [GitHub 仓库](https://github.com/OpenTraffic-Team/opentraffic-ops)
统一的系统运行时底座，负责全局调度与基础设施能力。

* Agent 生命周期管理（启动 / 停止 / 调度）
* 模型与服务注册
* 任务编排与运行时管理
* 数据流与消息系统
* 边云协同执行

---

# 🚦 交通控制栈

## 🤖 opentraffic-tsc-agent

👉 [GitHub 仓库](https://github.com/OpenTraffic-Team/opentraffic-tsc-agent)

* 多路口协同控制
* Agent 决策编排
* 在线 / 离线推理
* 与 Ops 系统交互

---

## 🛠 opentraffic-tsc-skills

👉 [GitHub 仓库](https://github.com/OpenTraffic-Team/opentraffic-tsc-skills)

* 相位切换策略
* 排队长度 / 交通流量计算
* 奖励 / 代价设计
* 安全约束与动作规则

---

## 🧠 opentraffic-tsc-engine

👉 [GitHub 仓库](https://github.com/OpenTraffic-Team/opentraffic-tsc-engine)

* 强化学习 / 规则 / 混合控制模型
* 状态与动作空间定义
* 信号控制策略训练与推理
* 多阶段控制算法

---

# 👁️ 交通感知栈

## 🤖 opentraffic-perception-agent

👉 [GitHub 仓库](https://github.com/OpenTraffic-Team/opentraffic-perception-agent)

* 多模型协同调度
* 场景级感知任务执行
* 结构化交通状态输出
* Ops 通信

---

## 🛠 opentraffic-perception-skills

👉 [GitHub 仓库](https://github.com/OpenTraffic-Team/opentraffic-perception-skills)

* 目标追踪与 ID 管理
* 轨迹重建
* 交通流量 / 速度统计
* 事件检测（拥堵 / 事故）

---

## 🧠 opentraffic-perception-engine

👉 [GitHub 仓库](https://github.com/OpenTraffic-Team/opentraffic-perception-engine)

* 检测 / 跟踪 / 分类模型
* 多相机融合推理
* 边缘轻量模型 (TIR 等)
* 统一推理接口

---

# 🔁 数据流

## 🚦 控制管线

```text
OpenTraffic-Ops
   ↓
opentraffic-tsc-agent
   ↓
opentraffic-tsc-skills
   ↓
opentraffic-tsc-engine
```

## 👁️ 感知管线

```text
OpenTraffic-Ops
   ↓
opentraffic-perception-agent
   ↓
opentraffic-perception-skills
   ↓
opentraffic-perception-engine
```

---

# 🧠 设计理念

* 分层解耦 (Ops / Agent / Skills / Engine)
* 感知与控制对称架构
* 小模型优先 (边缘友好的引擎层)
* Agent 负责智能编排，不涉底层计算
* Ops 统一系统运行底座

---

# 🚀 亮点

* 🧠 基于 Agent 的交通智能
* ⚡ 实时边缘部署
* 🔄 基于强化学习的信号优化
* 👁️ 多相机感知融合
* 🧩 模块化插件架构

---

# 📦 仓库

### 💻 OPS
* [https://github.com/OpenTraffic-Team/opentraffic-ops](https://github.com/OpenTraffic-Team/opentraffic-ops)

### 🚦 控制
* [https://github.com/OpenTraffic-Team/opentraffic-tsc-agent](https://github.com/OpenTraffic-Team/opentraffic-tsc-agent)
* [https://github.com/OpenTraffic-Team/opentraffic-tsc-skills](https://github.com/OpenTraffic-Team/opentraffic-tsc-skills)
* [https://github.com/OpenTraffic-Team/opentraffic-tsc-engine](https://github.com/OpenTraffic-Team/opentraffic-tsc-engine)

### 👁️ 感知
* [https://github.com/OpenTraffic-Team/opentraffic-perception-agent](https://github.com/OpenTraffic-Team/opentraffic-perception-agent)
* [https://github.com/OpenTraffic-Team/opentraffic-perception-skills](https://github.com/OpenTraffic-Team/opentraffic-perception-skills)
* [https://github.com/OpenTraffic-Team/opentraffic-perception-engine](https://github.com/OpenTraffic-Team/opentraffic-perception-engine)

---

# 🌐 社区

OpenTraffic 欢迎以下领域的贡献者：

* 🚗 智能交通算法研究者
* 🧠 强化学习开发者
* 👁️ 计算机视觉工程师
* ⚙️ 边缘计算与系统工程师
* 🚦 智慧交通行业从业者

---

# 📬 联系我们

如需合作或贡献，请联系 OpenTraffic 团队。

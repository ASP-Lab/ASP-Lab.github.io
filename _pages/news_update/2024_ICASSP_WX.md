---
layout: archive
title: "ASP 课题组论文《Distributed-Robust Source Localization in Wireless Acoustic Sensor Networks》被 ICASSP 2025 接收"
permalink: /news_update/2024_ICASSP_WX
author_profile: false
---

{% include base_path %}

======

近日，王旭同学论文 **《Distributed-Robust Source Localization in Wireless Acoustic Sensor Networks》** 成功被 **IEEE ICASSP 2025** 接收。ICASSP 是全球信号处理领域最具影响力的顶级会议，本次论文的录用充分展示了团队在 **分布式声学定位（Distributed Acoustic Localization）** 与 **无线声学传感器网络（WASN）** 方向的最新研究成果。

声源定位（Source Localization）是 WASN 中的重要任务，但实际网络中普遍存在 **噪声干扰、节点异构、同步偏差、节点数量不均、网络拓扑稀疏** 等问题，使得定位系统在分布式场景下容易出现漂移、精度下降及鲁棒性不足。

为此，论文提出了一种 **分布式鲁棒声源定位框架（Distributed-Robust Source Localization, DR-SL）**，结合 TDOA 空间特征、网格投票机制和分布式协作策略，在无需集中式计算的条件下实现高精度、强鲁棒性的定位能力。

---

##  **方法主要创新点**

- **1. TDOA 曲线–网格投票机制（Curve-to-Grid Voting）**  
  通过构建节点内部多麦克风对的 TDOA 曲线，并判断曲线是否穿过空间网格块来构成概率投票，提升定位对噪声与混响的鲁棒性。

- **2. 分布式更新策略（Fully Distributed Update）**  
  每个节点仅需与邻居节点进行局部信息交换，无需全局参数同步，大幅降低通信量。

- **3. 鲁棒一致性融合（Robust Consensus Fusion）**  
  针对节点质量不一致与环境噪声干扰，通过鲁棒一致性策略抑制异常节点对整体定位结果的破坏。

- **4. 多源场景可扩展性（Scalable to Multi-Source）**  
  框架可自然拓展到多个声源场景，无需额外训练或模型复杂度提升。

基于大量仿真与真实 WASN 数据的实验结果表明：**F-D-R-SSL 算法在噪声、混响和网络稀疏条件下均显著优于传统 SRP-PHAT、TDOA-Grid 方法及部分分布式定位算法。**

---

##  **图示说明**


<div style="text-align: center;">
  <img src="/images/news_update/2024_ICASSP_wx1.png" alt="网格划分与TDOA曲线" style="width: 80%; max-width: 650px;">
</div>

<center><em>图 1  网格划分示意：展示第 m 个节点中由多麦克风对构成的 TDOA 曲线</em></center>

---


<div style="text-align: center;">
  <img src="/images/news_update/2024_ICASSP_wx2.png" alt="F-D-R-SSL流程" style="width: 80%; max-width: 650px;">
</div>

<center><em>图 2  F-D-R-SSL 算法网格划分插图，红色五角星表示真实声源位置。</em></center>

<br />
<br />

---

该论文由 **内蒙古大学 ASP 课题组** 独立完成，作者包括：  
**王旭、斯琴图雅、呼德研究员（通讯作者）**
研究得到国家自然科学基金及相关科研项目的支持。

---
layout: archive
title: "ASP 课题组论文《Robust Self-Localization of Wireless Acoustic Sensor Networks in the Presence of TDoA Outliers》发表于 IEEE Transactions on Mobile Computing"
permalink: /news_update/2026_TMC_WX
author_profile: false
---

{% include base_path %}

======

近日，计算机学院（软件学院）、人工智能学院 ASP 课题组论文 **《Robust Self-Localization of Wireless Acoustic Sensor Networks in the Presence of TDoA Outliers》** 发表在国际顶级期刊 **IEEE Transactions on Mobile Computing**。该刊是传感网络与移动计算领域的国际旗舰期刊，也是 **CCF-A 类期刊**，最新影响因子为 **9.2**。本次成果发表充分展示了团队在 **无线声学传感器网络（WASN）** 与 **节点自定位（Self-Localization）** 方向的最新研究进展。

与传统麦克风阵列相比，声传感器网络（也称声物联网）具有 **拓扑结构灵活、空间覆盖范围大、支持分布式计算** 等显著优势，因此被认为是下一代智能声信号处理的重要平台。然而，在实际复杂环境中，到达时间差（Time Difference of Arrival, TDoA）观测往往会受到异常值（outliers）、噪声和混响等因素的影响，从而严重降低节点自定位的精度与稳定性。

为此，论文针对 **TDoA 异常值存在情况下的 WASN 节点自定位问题**，对异常观测的产生概率进行了数学建模，并在此基础上提出了 **集中式** 与 **分布式** 两种鲁棒节点自定位方法，用以提升复杂声学环境下的定位精度与系统稳定性。

---

##  **方法主要创新点**

- **1. TDoA 异常值概率建模（TDoA Outlier Probability Modeling）**  
  针对复杂环境中常见的 TDoA 异常观测问题，论文从概率建模角度刻画了异常值的产生机制，为后续鲁棒定位算法设计提供了理论基础。

- **2. 集中式鲁棒自定位方法（Centralized Robust Self-Localization）**  
  在全局观测条件下，利用异常值建模结果构建新的鲁棒几何优化框架，从而有效减弱异常 TDoA 对节点位置估计的影响。

- **3. 分布式鲁棒自定位方法（Distributed Robust Self-Localization）**  
  结合 WASN 的分布式计算特点，提出无需集中式处理的节点协作定位策略，使各节点在局部信息交互下实现稳定的自定位估计。

- **4. 强鲁棒性与高精度（Robustness and Accuracy）**  
  所提方法在存在 TDoA 异常值、复杂噪声和混响条件下仍能保持较高定位精度，为实际部署中的 WASN 自校准提供了有效方案。

实验结果表明：**在复杂声学环境下，所提集中式与分布式方法均能显著提升节点自定位性能，节点定位误差可稳定控制在 10 cm 以内。**

---

##  **图示说明**

<div style="text-align: center;">
  <img src="/images/news_update/2026_TMC_wx1.png" alt="WASN节点自定位系统框图" style="width: 80%; max-width: 650px;">
</div>

<center><em>图 1  无线声学传感器网络节点自定位系统示意图。</em></center>

---

<div style="text-align: center;">
  <img src="/images/news_update/2026_TMC_wx2.png" alt="实验结果展示" style="width: 80%; max-width: 650px;">
</div>

<center><em>图 2  所提方法在复杂声学环境下的部分实验结果展示。</em></center>
---

<div style="text-align: center;">
  <img src="/images/news_update/2026_TMC_wx3.png" alt="实际环境中的实验" style="width: 80%; max-width: 650px;">
</div>

<center><em>图 3  所提方法在实际环境中的实验展示。</em></center>

<br />
<br />

---

该论文由 **内蒙古大学 ASP 课题组** 独立完成，作者包括：  
**呼德研究员（通讯作者）、王旭（2024级博士研究生）**

研究得到国家自然科学基金青年基金、地区基金，内蒙古自治区本级引进高层次人才科研支持、内蒙古大学“骏马计划”高层次人才引进等项目的支持。

论文链接：[https://ieeexplore.ieee.org/document/11450502](https://ieeexplore.ieee.org/document/11450502)

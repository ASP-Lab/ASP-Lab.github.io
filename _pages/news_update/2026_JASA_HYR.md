---
layout: archive
title: "ASP 课题组论文《Active Noise Control Incorporating External Wireless Acoustic Sensors》发表于声学顶级期刊 JASA"
permalink: /news_update/2026_JASA_HYR
author_profile: false
---

{% include base_path %}

======

近日，计算机学院（软件学院）、人工智能学院 ASP 课题组在 **主动噪声控制（Active Noise Control, ANC）与无线声学传感器网络（Wireless Acoustic Sensor Networks, WASNs）** 方向取得重要研究进展，相关论文 **《Active Noise Control Incorporating External Wireless Acoustic Sensors》** 被国际声学顶级期刊 **The Journal of the Acoustical Society of America（JASA）** 录用。

JASA 由美国声学学会（Acoustical Society of America, ASA）出版，自 1929 年创刊以来，一直是国际声学领域具有重要影响力的旗舰学术期刊，涵盖物理声学、工程声学、语音与听觉、噪声控制等多个研究方向。**值得一提的是，该成果是内蒙古自治区首篇由区内单位作为第一单位在 JASA 发表的研究论文。**

传统主动噪声控制系统通常依赖部署在本地的参考麦克风获取噪声信息，其降噪性能受到本地传感器数量、部署位置以及空间覆盖范围等因素的限制。随着无线声学传感器网络以及智能终端设备的发展，分布在声学空间中的外部麦克风能够提供更加丰富的噪声观测信息，为进一步提升主动噪声控制性能提供了新的可能。

为此，论文构建了一种 **外部无线声传感器辅助的主动噪声控制框架**，将分布于外部空间的无线声学传感器引入本地 ANC 系统，在充分利用外部声学信息的同时，重点解决由无线通信延迟和额外传感器引起的实时性与计算复杂度问题。

---

## **方法主要创新点**

* **1. 外部无线声传感器辅助 ANC（External Wireless Acoustic Sensor-assisted ANC）**
  构建了一种融合本地参考麦克风与外部无线声传感器的主动噪声控制框架，利用空间中更加丰富的声学观测信息辅助本地 ANC 系统，从而突破传统系统仅依赖本地参考信号的限制。

* **2. 面向无线通信延迟的控制滤波（Communication Delay-aware Control Filtering）**
  针对外部声传感器数据通过无线网络传输所产生的通信延迟问题，论文推导了 **考虑通信延迟的控制滤波器闭式解**，并进一步给出了相应的自适应实现，使系统能够有效利用存在传输延迟的外部声学信息。

* **3. 外部声传感器贡献度分析与选择（Sensor Contribution Analysis and Selection）**
  针对引入大量外部声传感器可能造成的额外计算负担，从理论上分析不同外部声传感器对本地 ANC 降噪性能的贡献，并据此选择少量贡献较大的传感器参与噪声控制，在降低系统复杂度的同时尽可能保持降噪性能。

* **4. 面向实际智能终端的可扩展 ANC 框架（Scalable ANC Framework）**
  所提出的方法为利用智能手机、智能音箱及其他分布式智能终端中的麦克风辅助主动噪声控制提供了新的技术思路，有助于进一步扩大 ANC 系统的空间感知范围与实际应用能力。

仿真与实际环境实验均验证了所提方法的有效性。实验结果表明：**通过合理利用外部无线声传感器提供的声学信息，并进一步考虑无线通信延迟与传感器选择问题，可以有效提升主动噪声控制系统的性能，同时兼顾系统的实时性与计算效率。**

---

<div style="text-align: center;">
  <img src="/images/news_update/2026_JASA_HYR.png" style="width: 80%; max-width: 650px;">
</div>

<br />
<br />

---

该论文由 **内蒙古大学** 与 **中国科学院声学研究所** 合作完成，论文第一单位为 **内蒙古大学**。作者包括：
**呼德研究员、何艳榕（2025级博士研究生）、赵清颖讲师、李军锋研究员**。

该研究获得国家自然科学基金杰出青年项目、青年项目、地区项目，以及内蒙古自治区自然科学基金青年项目、内蒙古大学“骏马计划”高层次人才引进等项目的支持。

论文链接：https://doi.org/10.1121/10.0044566

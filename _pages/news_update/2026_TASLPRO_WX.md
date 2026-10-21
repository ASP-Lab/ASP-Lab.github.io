---
layout: archive
title: "ASP 课题组论文《From Theoretical to Practical Source Placement for Active Geometry Calibration of Distributed Microphone Arrays》被 IEEE/ACM Transactions on Audio, Speech, and Language Processing 录用"
permalink: /news_update/2026_TASLPRO_WX
author_profile: false
---

{% include base_path %}

======

近日，计算机学院（软件学院）、人工智能学院 ASP 课题组在 **分布式麦克风阵列几何校准（Geometry Calibration of Distributed Microphone Arrays）** 方向取得最新研究进展，相关论文 **《From Theoretical to Practical Source Placement for Active Geometry Calibration of Distributed Microphone Arrays》** 研究了主动几何校准中的最优声源布放问题，提出了一种从理论最优分析到实际迭代校准的完整解决方案。

分布式麦克风阵列（Distributed Microphone Arrays, DMAs）具有空间覆盖范围广、部署灵活等优势，被广泛应用于声源定位、波束形成和声学事件监测等任务。然而，这些应用通常需要已知麦克风的空间位置，因此，**准确获取阵列几何结构是实现高性能空间声学处理的重要前提**。

现有主动几何校准方法通常利用多个已知位置的校准声源估计麦克风坐标，但校准声源往往采用随机布放方式，未充分考虑声源空间位置对几何校准精度的影响。这可能导致较高的定位误差，限制系统的校准性能。因此，**如何通过合理布置校准声源来提高分布式麦克风阵列的几何校准精度**，是本文重点解决的问题。

为此，论文提出了一种 **从理论到实际的主动几何校准声源优化布放方法**。该方法利用位置可控的移动机器人作为校准声源，首先从理论上分析不同声源位置对阵列几何校准精度的影响，并推导同步与异步场景下的最优 Cramér–Rao 下界（Optimal Cramér–Rao Lower Bound, oCRLB）及其对应的最优几何条件。在此基础上，针对不同阵列配置设计声源位置优化方法，并进一步考虑实际麦克风位置未知的问题，提出迭代式声源布放策略，逐步提高阵列几何校准精度。

---

## **方法主要创新点**

* **1. 基于移动机器人的主动几何校准（Robot-assisted Active Geometry Calibration）**  
  不同于传统随机布放校准声源的方法，本文利用位置可控的移动机器人作为校准声源，通过主动调整机器人的发声位置，获取更加有利于阵列几何校准的声学观测信息，从而提升麦克风位置估计精度。

* **2. 同步与异步场景下的最优 CRLB 分析（Optimal CRLB Analysis）**  
  针对同步和异步分布式麦克风阵列，分别推导基于到达时间（Time of Arrival, ToA）观测的 **最优 Cramér–Rao 下界（oCRLB）**，并进一步分析实现理论最优校准精度所需的声源几何条件，为校准声源的合理布置提供理论依据。

* **3. 最优声源位置求解（Optimal Source Placement）**  
  根据不同麦克风阵列配置及其几何特点，分别设计 **闭式声源布放方案与数值优化方法**，使校准声源的位置能够满足或尽可能接近理论最优几何条件，从而降低阵列几何校准误差。

* **4. 面向实际未知阵列的迭代式校准（Iterative Source Placement）**  
  考虑到实际应用中麦克风位置通常未知，无法直接依据真实阵列几何结构计算最优声源位置，本文进一步提出 **迭代式声源布放策略**，通过交替进行麦克风阵列几何估计与校准声源位置优化，逐步改善声源布放方案并提高几何校准精度，实现从理论最优设计到实际系统部署的有效衔接。

仿真与真实录音实验均验证了所提方法的有效性。实验结果表明，**相比传统随机声源布放方式，所提出的最优声源布放策略能够有效降低分布式麦克风阵列的几何校准误差**，并在不同声学条件下表现出良好的性能。

特别是在真实录音实验中，所提方法在多种几何校准算法下均取得了更低的均方误差（MSE），验证了声源位置优化对于提高实际阵列校准精度的有效性。

上述结果表明，该研究不仅从理论上揭示了 **校准声源空间分布与麦克风阵列几何校准精度之间的关系**，还通过迭代优化解决了实际麦克风位置未知条件下的声源布放问题，为 **分布式麦克风阵列的高精度几何校准与实际部署** 提供了新的技术思路。

---

## **图示说明**

<div style="text-align: center;">
  <img src="/images/news_update/2026_TASLPRO_WX1.png" alt="分布式麦克风阵列主动几何校准系统框架" style="width: 80%; max-width: 650px;">
</div>

<center><em>图 1  基于移动机器人的分布式麦克风阵列主动几何校准系统框架。</em></center>

---

<div style="text-align: center;">
  <img src="/images/news_update/2026_TASLPRO_WX2.png" alt="真实环境中的几何校准实验" style="width: 80%; max-width: 650px;">
</div>

<center><em>图 2  分布式麦克风阵列主动几何校准的真实环境实验设置。</em></center>

---

<div style="text-align: center;">
  <img src="/images/news_update/2026_TASLPRO_WX3.png" alt="最优声源布放方法实验结果" style="width: 80%; max-width: 650px;">
</div>

<center><em>图 3  所提方法与传统随机声源布放方法的部分实验结果对比。</em></center>

<br />
<br />

---

该论文作者包括：  
**呼德、王旭、斯琴图雅、李军峰**。

该研究围绕分布式麦克风阵列的 **主动几何校准与最优声源布放** 展开，通过将理论最优几何分析与实际迭代优化相结合，为复杂声学环境下的阵列自校准提供了新的解决方案。


---
layout: archive
title: "我组四篇论文被 INTERSPEECH 2026 录用"
permalink: /news_update/2026_INTERSPEECH
author_profile: false
---

{% include base_path %}

======

近日，我课题组共有 **四篇论文** 被国际语音大会 **INTERSPEECH 2026** 录用。四项工作分别面向 HRTF 个性化建模、开放式助听器双耳语音增强、分布式麦克风阵列几何校准以及声源定位等关键声学任务，展示了我组在 **空间音频、智能助听、声传感器网络与声源定位** 等方向的最新研究进展。

---

# **1. SA-HRTF: A Sound-Assisted Approach to Personalized HRTF Modeling**

**作者：** 赵清颖、陈思远、呼德（通讯作者）

头相关传输函数（Head-Related Transfer Functions, HRTFs）是实现沉浸式双耳音频渲染的关键技术，但高密度个性化 HRTF 测量通常耗时且成本较高。针对稀疏测量条件下个性化 HRTF 难以准确重建的问题，本文提出一种 **声音辅助的个性化 HRTF 建模方法 SA-HRTF**，利用双耳声音信号提供额外的听觉感知信息：

* **声音辅助 HRTF 个性化**：突破仅依赖已有 HRTF 数据进行个性化建模的传统方式，引入双耳声音信息辅助 HRTF 预测；
* **双路径网络架构**：主路径从现有 HRTF 数据库中学习结构特征并生成初始估计，辅助路径从声音信号中提取与听觉感知相关的互补特征；
* **双路径特征融合**：通过融合模块整合 HRTF 先验与声音辅助信息，获得更加准确的个性化 HRTF；
* **稀疏测量下的高精度重建**：实验结果表明，该方法能够有效提升个性化 HRTF 的重建性能，为降低个体 HRTF 测量成本提供了新的解决思路。

<div style="text-align: center;">
  <img src="/images/news_update/2026_INTERSPEECH/SA_HRTF_framework.png" alt="SA-HRTF 模型框架示意图" style="width: 80%; max-width: 600px;">
</div>
<center>图1 SA-HRTF 声音辅助个性化 HRTF 建模框架</center>

---

# **2. ABSE-NET: A Lightweight Neural Model for Active Binaural Speech Enhancement in Open-Fit Hearing Aids**

**作者：** 呼德（通讯作者）、杜学、赵清颖、斯琴图雅

开放式助听器具有良好的佩戴舒适性，但其开放结构会使外部声音直接泄漏进入耳道，从而影响双耳语音增强效果。针对这一问题，本文提出一种 **主动双耳语音增强网络 ABSE-NET**，将主动噪声控制（ANC）与双耳语音增强（BSE）进行联合设计：

* **BSE 与 ANC 联合建模**：同时实现目标语音增强与开放式助听器中的声学泄漏抑制，提升复杂声学环境下的听觉体验；
* **BMVDR + 轻量级神经网络级联架构**：首先利用双耳最小方差无失真响应（BMVDR）波束形成器进行初步语音增强，再利用轻量级神经网络进一步消除声学泄漏并补偿语音失真；
* **时频依赖与注意力建模**：在编码器–解码器网络中设计频率–时间依赖学习模块与卷积注意力模块，充分挖掘语音在时间和频率维度上的关联信息；
* **面向实际助听设备部署**：与传统 BSE-ANC 方法相比，ABSE-NET 在实际部署过程中无需耳内麦克风，在降低系统部署复杂度的同时取得了优于现有方法的客观语音增强性能。

<div style="text-align: center;">
  <img src="/images/news_update/2026_INTERSPEECH/ABSE_NET_framework.png" alt="ABSE-NET 模型框架示意图" style="width: 80%; max-width: 600px;">
</div>
<center>图2 ABSE-NET 主动双耳语音增强总体框架</center>

---

# **3. Optimal Source Placement for TDoA-based Geometry Calibration of Distributed Microphone Arrays**

**作者：** 王旭、斯琴图雅（通讯作者）、赵清颖、呼德

分布式麦克风阵列（Distributed Microphone Arrays, DMAs）的几何位置是声源定位、语音增强等空间音频任务的重要先验信息。然而，现有几何校准方法通常随机布置校准声源，其位置并不一定能够提供最有效的几何信息，进而影响阵列校准精度。针对这一问题，本文研究了 **基于 TDoA 的 DMA 几何校准中的最优声源布置问题**：

* **从“校准算法”进一步拓展到“校准源位置优化”**：利用移动机器人作为多个校准声源，通过主动优化其空间位置提升麦克风阵列几何校准精度；
* **基于 TDoA 的 CRLB 理论分析**：针对存在时间偏移的到达时间差（TDoA）观测，推导几何校准问题的 Cramér-Rao 下界（CRLB），量化不同声源位置对校准精度的影响；
* **最优校准源位置求解**：在有限房间空间约束下，以最小化 CRLB 为目标寻找更加有利于阵列几何校准的声源位置；
* **多阶段高效求解策略**：针对计算资源受限或实时性要求较高的应用场景，进一步提出多阶段求解方法，在降低计算开销的同时保持较好的校准性能。

<div style="text-align: center;">
  <img src="/images/news_update/2026_INTERSPEECH/Optimal_Source_Placement.png" alt="最优校准声源位置示意图" style="width: 80%; max-width: 600px;">
</div>
<center>图3 分布式麦克风阵列几何校准中的最优声源布置示意图</center>

---

# **4. G2C-NET: A Grid-to-Continuous Neural Network for Sound Source Localization in Distributed Microphone Arrays**

**作者：** 岳致远、呼德（通讯作者）

基于网格的声源定位方法能够将连续坐标回归转化为空间分类，在复杂声学环境下具有较好的稳定性，但同时存在 **网格分辨率与计算复杂度之间的固有矛盾**：粗网格容易产生明显的量化误差，而增加网格密度又会显著提升计算成本。针对这一问题，本文提出一种 **从网格到连续坐标的声源定位网络 G2C-NET**，在不增加网格密度的情况下实现亚网格级连续位置估计：

* **全局似然估计（GLE）**：通过自适应麦克风对特征聚合器，根据不同麦克风对声学信息的可靠性动态分配权重，抑制噪声与混响造成的不可靠空间特征；
* **连续位置估计（CPE）**：不再直接将峰值网格中心作为最终定位结果，而是利用峰值网格及其局部邻域的空间似然进行加权，实现从离散网格到连续坐标的映射；
* **空间分布与坐标联合监督**：联合使用空间分布损失与坐标回归损失，使网络同时学习全局空间结构和细粒度连续位置；
* **兼顾精度、鲁棒性与计算效率**：在相同网格分辨率下，G2C-NET 在模拟数据上取得 **25.52 cm RMSE 和 78.63% 的 30 cm 定位准确率**，在真实数据上取得 **23.35 cm RMSE 和 81.15% 的定位准确率**，并能够适应 4–7 个麦克风节点，在强混响及节点数量较少的情况下仍保持较好的定位性能。

<div style="text-align: center;">
  <img src="/images/news_update/2026_INTERSPEECH/G2C_NET_framework.png" alt="G2C-NET 网络框架示意图" style="width: 80%; max-width: 600px;">
</div>
<center>图4 G2C-NET 从空间网格到连续声源坐标的定位框架</center>

---

四篇论文的录用展示了我组在 **空间音频、智能助听、分布式声学感知与声源定位** 等方向的持续研究进展。其中，相关工作既关注 HRTF 个性化、开放式助听器语音增强等面向听觉感知与实际应用的问题，也围绕分布式麦克风阵列的几何校准与高精度声源定位开展了深入探索。

未来，我们将继续面向 **智能声学与语音信号处理** 中的关键问题开展研究，推动空间音频、无线声学传感器网络、智能助听与声学感知技术在真实复杂环境中的进一步应用。

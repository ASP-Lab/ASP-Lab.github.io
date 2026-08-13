---

layout: archive
title: "ASP 课题组论文《Low-Rate Voice Activity Detector Over Wireless Acoustic Sensor Networks》被 IEEE Transactions on Audio, Speech and Language Processing 录用"
permalink: /news_update/2026_TASLPRO_LSJ
author_profile: false
---------------------

{% include base_path %}

======

近日，计算机学院（软件学院）、人工智能学院 ASP 课题组论文 **《Low-Rate Voice Activity Detector Over Wireless Acoustic Sensor Networks》** 被 语音信号处理顶级期刊 **IEEE Transactions on Audio, Speech and Language Processing** 录用。该工作面向 **无线声学传感器网络（Wireless Acoustic Sensor Networks, WASNs）中的语音活动检测（Voice Activity Detection, VAD）**，针对多节点音频数据传输带来的高通信开销问题，提出了一种兼顾检测性能与通信效率的 **低码率语音活动检测方法（Low-Rate VAD）**。

语音活动检测是语音增强、关键词唤醒、自动语音识别以及说话人日志等语音处理系统中的重要前端技术。相比单麦克风或传统麦克风阵列，WASN 通过将多个声学节点分布在空间中的不同位置，可以获取更加丰富的空间声学信息，在远场、噪声和混响等复杂环境下具有明显优势。

然而，传统 WASN 通常需要多个节点持续向融合中心传输音频信号或高维声学特征。随着节点数量增加，**无线通信量和节点能量消耗将迅速增长**，成为制约大规模 WASN 实际部署的重要因素。因此，如何在尽可能减少节点通信数据量的同时保持较高的 VAD 检测性能，是本文重点解决的问题。

为此，论文提出了一种 **面向无线声学传感器网络的 Low-Rate VAD 框架**。该方法将声学特征提取与压缩过程部署在各个节点本地，通过量化编码将连续高维特征转换为少量离散信息进行无线传输，并根据不同节点对于 VAD 任务的重要程度自适应调整传输码率；融合中心则进一步完成多节点信息聚合与时间建模，最终得到语音活动检测结果。

---

## **方法主要创新点**

* **1. 面向 WASN 的低码率 VAD 框架（Low-Rate VAD over WASNs）**
  不再要求各个无线节点持续向融合中心传输完整音频数据，而是在节点本地完成声学表示学习与信息压缩，仅传输与 VAD 任务高度相关的紧凑信息，从而显著降低无线通信负担。

* **2. 基于残差向量量化的特征压缩（Residual Vector Quantization）**
  各节点首先从本地音频中学习紧凑的声学表示，并进一步利用 **残差向量量化** 将连续特征编码为少量离散码字，在尽可能保留语音活动信息的同时大幅压缩需要传输的数据量。

* **3. 自适应节点码率分配（Adaptive Rate Allocation）**
  考虑到不同位置的声学节点对当前语音活动检测任务具有不同贡献，模型根据节点的重要程度 **自适应分配传输码率**，使重要节点传输更多有效信息，而贡献较低的节点采用更低码率，从而进一步提高整体通信效率。

* **4. 多节点自适应融合与时间建模（Channel Aggregation and Temporal Modeling）**
  在融合中心对来自不同节点的量化特征进行自适应聚合，并进一步建模语音活动在时间维度上的连续变化，在低通信码率条件下充分利用 WASN 的多节点空间信息。

实验结果表明，所提出的 Low-Rate VAD 在不同网络规模以及真实录音场景下均表现出良好的检测性能。**在包含 20 个声学节点的 WASN 中，该方法的 VAD F1 值达到 96.94%，同时每个节点每帧仅需传输不超过 84 bit 的数据。**

上述结果表明，Low-Rate VAD 能够在保持较高语音活动检测性能的同时，大幅减少节点与融合中心之间的数据传输量，为 **低通信开销、低能耗、大规模无线声学传感器网络** 中的智能语音感知提供了新的解决思路。

---

## **图示说明**

<div style="text-align: center;">
  <img src="/images/news_update/2026_LowRate_VAD1.png" alt="Low-Rate VAD总体框架" style="width: 80%; max-width: 650px;">
</div>

<center><em>图 1  面向无线声学传感器网络的 Low-Rate VAD 总体框架。</em></center>

---

<div style="text-align: center;">
  <img src="/images/news_update/2026_LowRate_VAD2.png" style="width: 80%; max-width: 650px;">
</div>

<center><em>图 2  Low-Rate VAD 的部分实验结果。</em></center>

<br />
<br />

---

该论文由 **内蒙古大学 ASP 课题组** 与相关科研团队合作完成，作者包括：
**呼德研究员、李少杰、赵清颖、李军锋**。

该研究围绕无线声学传感器网络中的 **低通信开销智能语音感知** 展开，为在资源受限的无线节点上部署高性能语音前端算法提供了新的技术思路。


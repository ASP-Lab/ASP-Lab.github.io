---
layout: archive
title: "我组三篇论文被 EUSIPCO 2025 录用 / 接收"
permalink: /news_update/2025_EUSIPCO
author_profile: false
---

{% include base_path %}

======

我课题组共有三篇研究成果被国际著名学术会议 **European Signal Processing Conference（EUSIPCO 2025）** 接收。相关工作覆盖 **语音活动与重叠语音检测、前馈主动噪声控制（ANC）参考麦克风选择、输入/输出通道联合优化** 等方向，体现了团队在声学信号处理、多麦克风网络系统以及资源高效化建模方面的最新探索。

---

# **1. A Lightweight Cross-Domain Front-End Feature Extractor for Multichannel Voice Activity and Overlapped Speech Detection**

**作者**：Shaojie Li, Qintuya Si, **De Hu**  

### **研究背景**  
在远场语音、多麦克风场景中，语音活动检测（VAD）与重叠语音检测（OSD）是语音增强、会议分析、语音识别等系统的关键前端模块。然而，传统 VAD/OSD 特征往往在跨通道建模能力不足，或对噪声／混响敏感；同时高维多通道特征会带来额外计算成本。

### **方法概述**  
本文提出一种 **轻量级跨域前端特征提取器（Lightweight Cross-Domain Feature Extractor, L-CD-FE）**，通过在 **时域与频域（cross-domain）联合建模** 的方式，有效融合空间差异与语音结构信息。

核心特点包括：

- 设计跨通道一致性的多麦克风特征结构，使系统在 **麦克风数量变化** 时仍可稳定运行；
- 在保证检测性能的前提下显著降低特征计算复杂度；
- 同时面向 VAD 与 OSD 等多类语音检测任务。

### **意义**  
该方法适用于会议系统、智能音箱、远场识别、智慧办公等多通道语音场景，为 **低复杂度、多通道语音检测前端** 提供了可扩展方案。

<div style="text-align: center;">  
  <img src="/images/news_update/2025_eusipco/VAD_feature_extractor_framework.png" style="width: 80%; max-width: 600px;">  
</div>  
<center>图1 轻量级跨域前端特征提取器（L-CD-FE）结构示意图</center>

---

# **2. Reference Microphones Selection for Feedforward Active Noise Control Exploiting Microphone Networks**

**作者**：Yanrong He（内蒙古大学硕士研究生）、**De Hu**  

### **研究背景**  
传统前馈主动噪声控制（ANC）系统通常依赖在噪声源附近部署一个或多个参考麦克风（Reference Microphones, RM）采集噪声信号。然而现实中噪声源位置常常未知且随时间变化，使参考信号不再“干净”，从而导致控制性能下降。

### **本文贡献**

本文提出一种 **基于麦克风网络（microphone network）** 的新型 ANC 框架，通过利用高空间分辨率的麦克风网络来采集噪声，并从中 **选择最具贡献度的子网络作为最佳参考麦克风集**。

主要创新包括：

- 将参考麦克风选择建模为一个 **布尔优化问题**，以最小化输出噪声功率；
- 相比暴力穷举搜索，该方法在计算量显著减少的情况下仍能达到 **接近最优的降噪性能**；
- 在噪声源位置时变、声场复杂的情况下仍保持稳健性。

### **应用价值**  
适用于大型空间（会议室、航空舱室、厂房）、可移动噪声场景等实际 ANC 系统，为 **多麦克风网络驱动的智能降噪系统** 提供了重要技术基础。

<div style="text-align: center;">  
  <img src="/images/news_update/2025_eusipco/ANC_ref_mic_selection.png" style="width: 80%; max-width: 600px;">  
</div>  
<center>图2 基于麦克风网络的参考麦克风选择框架示意图</center>

---

# **3. Joint Input and Output Channel Selection for Multi-channel Feedforward Active Noise Control**

**作者**：Yanrong He（内蒙古大学硕士研究生）、**De Hu**  
**通讯作者**：De Hu

### **研究背景**  
多通道前馈 ANC 系统利用多个参考麦克风和多个扬声器，可比单通道系统获得更优降噪效果。然而通道数增加会导致滤波器规模和计算量迅速上升，影响实时性和系统稳定性。

### **本文贡献**

本文首次提出 **输入通道（参考麦克风）与输出通道（扬声器／次级源）联合选择（J-IO-CS）方法**，通过统一建模方式同时优化输入与输出资源配置。

主要创新点包括：

- 基于空间滤波器的 **组稀疏性（group sparsity）** 构建新的通道选择模型；
- 将原始非凸优化问题，通过交换目标与约束并使用 **l₁,₂ 范数** 转化为一个凸可解问题；
- 引入可调参数保证优化后的模型与原始目标保持理论等价性；
- 在降低通道数量的同时保持优良噪声控制性能，大幅提升 ANC 系统实时效率。

### **意义**  
这是多通道前馈 ANC 中 **首次同时实现输入与输出通道联合选择**，相比仅选择参考麦克风的现有方法具有更高的计算效率与系统可扩展性。

<div style="text-align: center;">  
  <img src="/images/news_update/2025_eusipco/ANC_input_output_selection.png" style="width: 80%; max-width: 600px;">  
</div>  
<center>图3 多通道前馈 ANC 输入/输出通道联合选择（J-IO-CS）框架示意图</center>

---

这三项工作集中展现了我课题组在：

- 多通道语音检测前端设计  
- 麦克风网络驱动的主动噪声控制  
- 多通道信号系统的结构优化与稀疏建模  

等方向的系统性研究进展。

我们将继续在 **智能声学系统、空间音频、主动控制与多传感器网络** 等方向深入探索，为声学信号处理领域提供更高效、更可扩展的解决方案。

如论文链接、海报或会议页面公开，可在本页下方补充下载入口。


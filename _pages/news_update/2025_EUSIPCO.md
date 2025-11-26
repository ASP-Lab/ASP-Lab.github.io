---
layout: archive
title: "我组三篇论文被 EUSIPCO 2025 录用 / 接收"
permalink: /news_update/2025_EUSIPCO
author_profile: false
---

{% include base_path %}

======

我课题组有三篇研究成果被国际著名学术会议 **EUSIPCO 2025** 接收 / 录用，涵盖声学主动降噪、语音活动检测与麦克风网络选择等方向，体现了团队在声学信号处理与多通道语音 / 噪声控制领域的广泛探索。

---

# **1. A Lightweight Cross-Domain Front-End Feature Extractor for Multichannel Voice Activity and Overlapped Speech Detection**

**作者**：Shaojie Li, Qintuya Si, **De Hu** 

**研究背景与意义**：在远场、多通道语音场景中，语音活动检测 (VAD) 与重叠语音 (overlapped speech) 检测是语音增强、语音识别、语音分析等系统的重要前端。传统特征提取与检测方法在多通道与空间复杂条件下往往计算复杂或对噪声／混响敏感。

**方法亮点**：

- 提出一种 **轻量级、跨域 (cross-domain)** 的前端特征提取器，可在多通道输入下高效提取用于 VAD / 重叠语音检测的空间 + 频谱特征。  
- 特征提取器设计考虑 **通道数可变、多通道信号一致建模**，兼顾实时性与检测性能。  
- 相较于传统单通道或简单拼接多通道特征的方法，该设计在保留多通道空间信息的同时，不会带来过高计算/存储负担。

**意义 / 应用场景**：该方法适用于多麦克风远场语音捕捉系统（会议室、远场语音识别、智能音箱、会议转写等），为高效、低复杂度的 VAD / 重叠语音检测提供可行方案。
 
<div style="text-align: center;">  
  <img src="/images/news_update/2025_eusipco/VAD_feature_extractor_framework.png" alt="Cross-Domain Front-End Feature Extractor 结构示意图" style="width: 80%; max-width: 600px;">  
</div>  
<center>图1 一种轻量级跨域特征提取(L-CD-FE)体系示意图 </center>

---

# **2. Reference Microphones Selection for Feedforward Active Noise Control Exploiting Microphone Networks**

**作者**：Yanrong He, **De Hu** 

**研究背景与意义**：在多通道前馈 (feedforward) 主动噪声控制 (ANC) 系统中，当系统中存在大量麦克风 (microphone network) 时，如何正确选择参考麦克风 (reference microphones) 对系统稳定性与降噪效果至关重要。盲目使用全部麦克风可能导致过高计算复杂度、延迟增加或因声源位置变化引入性能不稳定。

**方法与贡献**：

- 利用麦克风网络结构和空间 / 时延 /声源分布信息，提出一种参考麦克风选择策略 (microphone-network-aware selection)，为 feedforward ANC 系统挑选最合适的参考通道。  
- 该策略考虑麦克风与噪声源、控制点之间的几何和传播约束，以保证因果性 (causality) 与有效性。  
- 实验／仿真显示，该选择策略能在变化的噪声环境下保持较好的降噪效果，同时减少麦克风使用数量，提高系统效率与稳定性。

**意义 / 应用**：该研究对大规模麦克风网络 / ANC 系统尤为重要，如智能空间降噪系统、车载 / 飞机 /工业环境中的主动降噪、多通道耳机 /头戴系统等。

<div style="text-align: center;">  
  <img src="/images/news_update/2025_eusipco/ANC_ref_mic_selection.png" alt="Feedforward ANC 参考麦克风选择示意图" style="width: 80%; max-width: 600px;">  
</div>  
<center>图2 参考麦克风选择机制示意图</center>

---

# **3. Joint Input and Output Channel Selection for Multi-channel Feedforward Active Noise Control**

**作者**：Yanrong He, **De Hu**

**研究背景**：在多通道前馈 ANC 系统中，不仅参考 (reference) 通道 (input) 的选择重要，系统输出通道 (output, 即 secondary sources / 控制扬声器/路径) 的选择也同样关键。输入通道与输出通道组合若不合理，将影响控制效果、系统稳定性与资源使用效率。

**方法与贡献**：

- 提出一种 **联合输入 (input) 与输出 (output) 通道选择机制**，针对 feedforward 多通道 ANC 同时决定哪些参考麦克风 (input channel) 和哪些控制通道 (output channel) 应被激活使用。  
- 该机制考虑声源分布、麦克风／扬声器网络结构、传播路径与系统资源限制，从而优化整体系统性能 / 资源消耗平衡。  
- 初步仿真 /评估表明，该联合选择策略在降低系统复杂度、减少资源使用量的同时，仍能维持良好噪声抑制效果。

**意义 / 应用**：对于实际部署多通道 ANC 的系统（如大空间降噪、复杂环境、多扬声器控制系统等）具有重要价值 —— 在资源受限、系统复杂的场景下还能保证稳定降噪效果。

<div style="text-align: center;">  
  <img src="/images/news_update/2025_eusipco/ANC_input_output_selection.png" alt="Multi-channel Feedforward ANC 通道选择示意图" style="width: 80%; max-width: 600px;">  
</div>  
<center>图3 输入/输出通道联合选择 框架示意图</center>

---

这三项工作集中体现了我组在 **多通道语音检测、多通道 / 多麦克风网络噪声控制、系统资源效率优化** 等方面的前沿探索。未来我们将继续深入，用更系统、更高性能的方法推进智能声学系统研究。

论文链接 / 下载地址：如有公开 PDF / 会议页面，请在图示下方或“论文链接”部分补充。  

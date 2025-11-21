---
layout: archive
title: "胡俊升同学关于个性化空间音频（HRTF）方面的研究《Graph Neural Field with Spatial-Correlation Augmentation for HRTF Personalization》发表于人工智能顶级会议《AAAI 2026》"
permalink: /news_update/2025_AAAI_Hjs
author_profile: false

---

{% include base_path %}


======
近日，胡俊升同学相关论文《Graph Neural Field with Spatial-Correlation Augmentation for HRTF Personalization》被人工智能国际顶级会议 **AAAI Conference on Artificial Intelligence（AAAI 2026）** 录用。AAAI 是人工智能领域最具影响力的国际旗舰会议之一，在中国计算机学会（CCF）会议分类中被列为 **A 类会议**。

在虚拟现实 / 增强现实（VR/AR）等设备中，为用户提供沉浸式 3D 空间音频体验，高质量的头相关传递函数（Head Related Transfer Function, HRTF）至关重要。然而，HRTF 的精确测量费时、昂贵，且与用户的头部尺寸、耳廓结构、躯干形状等人体差异强相关。因此，如何为新用户快速生成高精度、个性化的 HRTF 是一个重要挑战。

为解决这一问题，论文提出了一种 **空间相关性增强的图神经场模型（Graph Neural Field with Spatial-Correlation Augmentation, GraphNF-SCA）**，整体框架包含三个核心部分：(i) **HRTF 个性化模块**、(ii) **HRTF 上采样模块**、(iii) **微调阶段**。  
在个性化模块中，模型通过带有编码器-解码器结构的图神经网络进行目标用户 HRTF 的预测；在上采样模块中，另一图神经网络实现对 HRTF 的空间插值，充分学习其在空间位置上的相关性；最后，通过微调阶段进一步增强个性化 HRTF 的空间一致性。  
与现有方法相比，GraphNF-SCA 能够有效挖掘 HRTF 数据固有的空间相关特征，从而显著提升个性化 HRTF 的生成质量。实验表明，该方法在多个公开 HRTF 数据集上均取得了最优表现。


<div style="text-align: center;">
  <img src="/images/news_update/HRTF_GraphNF_framework.png" alt="GraphNF-SCA 模型框架示意图" style="width: 80%; max-width: 600px;">
</div>

<center> 图1 Network architecture for GNN-based HRTF-P module </center>
<br />
<br />

<div style="text-align: center;">
  <img src="/images/news_update/HRTF_experiment_results.png" alt="AAAI_results" style="width: 80%; max-width: 600px;">
</div>

<center>图2 部分实验结果展示</center>



内蒙古大学为论文唯一完成单位，作者包括：呼德研究员（通讯作者）、胡俊升（硕士研究生）、姜翠翠（硕士研究生）。该研究得到了国家自然科学基金项目、内蒙古自治区高层次人才支持计划、内蒙古大学高层次人才“骏马计划”等项目的支持。

 
论文链接：[https://www.arxiv.org/abs/2511.10697](https://www.arxiv.org/abs/2511.10697)

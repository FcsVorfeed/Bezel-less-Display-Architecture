# 单体无边框显示系统技术白皮书 / Bezel-less Visual Elimination Solution for Standalone Display Devices

- **核心构思与作者 / Core Concept & Author:** 张烁 / Shuo Zhang
- **联合署名与所属机构 / Co-authored & Affiliated Institution:** 上海魔法少女网络科技有限公司 / Shanghai Magical Battle Syou Jyo Network Technology Co., Ltd.
- **发布日期 / Publication Date:** 2026年5月7日 / May 7, 2026

---

## ⚠️ 开源与防御性公开声明 / Open Source and Defensive Publication Declaration

本白皮书及其包含的所有技术方案、算法逻辑与架构设计，由张烁与上海魔法少女网络科技有限公司共同作为**现有技术 (Prior Art)** 予以防御性公开。本文档遵循 CC BY-SA 4.0 (署名-相同方式共享4.0国际) 协议开放。任何个人或组织均可自由查阅、使用并在遵守协议的前提下进行商业化探索，旨在打破显示设备工业的技术壁垒，防止上述构思被任意第三方进行过度专利垄断。

This whitepaper and all technical solutions, algorithm logic, and architectural designs contained herein are defensively published as **Prior Art** by Shuo Zhang and Shanghai Magical Battle Syou Jyo Network Technology Co., Ltd. This document is licensed under the CC BY-SA 4.0 (Attribution-ShareAlike 4.0 International) license. Any individual or organization is free to access, use, and explore commercialization under the premise of compliance with this license. The purpose is to break the technical barriers in the display device industry and prevent the aforementioned concepts from being over-monopolized by any third-party patents.

---

## 💡 摘要 / Abstract

本技术方案提出了一种低成本、高适用性的单体显示设备“0边框”视觉消除系统。针对现有纯光学无边框方案会导致边缘画面严重畸变的缺陷，本系统采用软硬件协同的混合架构：
* **物理层面：** 引入环状光学折射透镜遮蔽物理边框；
* **计算层面：** 通过 GPU 或 SOC 底层实时运行多模态视觉算法，包括逆向畸变映射、全局过扫描 (Overscan)，以及基于高斯模糊与运动补偿的边缘像素推演。

该方案不仅实现了单体显示设备的 1:1 无损无边框观感，更为多屏幕无缝拼接阵列提供了底层的帧生成补偿策略。

This technical solution proposes a low-cost, highly applicable "zero-bezel" visual elimination system for standalone display devices. Addressing the severe edge distortion defects caused by existing pure optical bezel-less solutions, this system adopts a hybrid hardware-software collaborative architecture. 
* **Physical Level:** A ring-shaped optical refraction lens is introduced to obscure the physical bezel.
* **Computational Level:** Multimodal visual algorithms—including inverse distortion mapping, global overscan, and edge pixel extrapolation based on Gaussian blur and motion compensation—are executed in real-time at the GPU or SOC driver layer.

This solution not only achieves a 1:1 lossless bezel-less visual experience for standalone displays but also provides a foundational frame generation compensation strategy for seamless multi-screen splicing arrays.

---

## 📁 包含文件 / Included Files

* `单体无边框显示系统技术白皮书.pdf` (中文完整版技术文档)
* `Bezel-less Display Whitepaper.pdf` (English Version Technical Document)

请查阅上述 PDF 文件以获取完整的技术细节、算法架构图以及渲染管线流程图。
Please refer to the PDF files above for complete technical details, algorithm architecture diagrams, and rendering pipeline flowcharts.

---

## ⚖️ 授权协议 / License

本项目遵循 [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/) 协议开放。
This work is licensed under a Creative Commons Attribution-ShareAlike 4.0 International License.

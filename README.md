# 图像匹配与分割项目集合

> 全面的计算机视觉项目集合 - 包含 10+ 个开源项目和自研工具

---

## 📁 项目结构

### 🎯 自研项目

| 项目 | 说明 |
|------|------|
| **[Image-Matching-Tools](file:///D:/A_Python/P1/Image-Matching-Tools/)** | 专业图像匹配工具库（6 种算法集成） |
| **[Image-Matching-Learning](file:///D:/A_Python/P1/Image-Matching-Learning/)** | 学习示例库（6 个算法的详细示例） |
| **图像匹配算法/** | 基础 Demo 代码（SIFT, SURF, ORB 等） |

### 📦 第三方开源项目

| 项目 | 会议/来源 | 说明 |
|------|----------|------|
| **[LightGlue](file:///D:/A_Python/P1/LightGlue-main/)** | ICCV 2023 | 轻量级特征匹配 |
| **[RoMa](file:///D:/A_Python/P1/RoMa-main/)** | CVPR 2024 | 鲁棒稠密特征匹配 |
| **[GIM](file:///D:/A_Python/P1/gim-main/)** | ICLR 2024 Spotlight | 通用图像匹配框架 |
| **[OmniGlue](file:///D:/A_Python/P1/omniglue-onnx-main/)** | CVPR 2024 | Google 通用特征匹配 |
| **[DeDoDe](file:///D:/A_Python/P1/DeDoDe-main/)** | 3DV 2024 | 检测器 + 描述子联合训练 |
| **[EfficientSAM](file:///D:/A_Python/P1/EfficientSAM-main/)** | - | 高效 Segment Anything |
| **[accelerated_features](file:///D:/A_Python/P1/accelerated_features-main/)** | - | XFeat 轻量级特征 |
| **[A2PM-MESA](file:///D:/A_Python/P1/A2PM-MESA-main/)** | - | 多视角立体匹配 |
| **[image-matching-webui](file:///D:/A_Python/P1/image-matching-webui-main/)** | - | Web 界面工具 |

---

## 🚀 快速开始

### 使用自研工具库

```bash
cd Image-Matching-Tools
pip install -e .
```

```python
from imtools import ImageMatcher

# 创建匹配器
matcher = ImageMatcher(algorithm='sift')

# 匹配图片
result = matcher.match('image1.jpg', 'image2.jpg')
result.show()
```

### 运行学习示例

```bash
cd Image-Matching-Learning
pip install -r requirements.txt
python 01-sift-matching.py
```

---

## 📊 算法对比

| 算法 | 速度 | 精度 | 专利 | 推荐场景 |
|------|------|------|------|---------|
| **SIFT** | ⭐⭐ | ⭐⭐⭐⭐⭐ | 已过期 | 高精度匹配 |
| **SURF** | ⭐⭐⭐ | ⭐⭐⭐⭐ | 需许可 | 快速匹配 |
| **ORB** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | 无 | 实时应用 |
| **AKAZE** | ⭐⭐⭐⭐ | ⭐⭐⭐⭐ | 无 | 平衡选择 |
| **LightGlue** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | 无 | 最佳选择 |

---

## ⚠️ 第三方开源项目声明

本目录包含多个优秀的开源图像匹配与分割项目。这些项目的版权归原作者所有。

### 1. LightGlue (ICCV 2023)
- **作者**: Philipp Lindenberger et al. (ETH Zurich, Microsoft Research)
- **论文**: [LightGlue: Local Feature Matching at Light Speed](https://arxiv.org/pdf/2306.13643.pdf)
- **官方仓库**: [cvg/LightGlue](https://github.com/cvg/LightGlue)
- **许可证**: Apache-2.0
- **特点**: 轻量级特征匹配，自适应剪枝，速度快

### 2. EfficientSAM
- **作者**: Yunyang Xiong et al. (Salesforce)
- **论文**: EfficientSAM: Leveraged Masked Image Pretraining for Efficient Segment Anything
- **官方仓库**: [yformer/EfficientSAM](https://github.com/yformer/EfficientSAM)
- **许可证**: Apache-2.0
- **特点**: 高效版 Segment Anything

### 3. DeDoDe
- **作者**: Johan Edstedt et al. (Linköping University)
- **论文**: DeDoDe: Detect, Describe, and Dense Match
- **官方仓库**: [Parskatt/DeDoDe](https://github.com/Parskatt/DeDoDe)
- **许可证**: Apache-2.0
- **特点**: 检测器和描述子联合训练

### 4. RoMa (CVPR 2024)
- **作者**: Johan Edstedt et al. (Linköping University)
- **论文**: Robust Dense Feature Matching
- **官方仓库**: [Parskatt/RoMa](https://github.com/Parskatt/RoMa)
- **许可证**: Apache-2.0
- **特点**: 鲁棒稠密特征匹配

### 5. GIM (ICLR 2024 Spotlight)
- **作者**: Xuelun Shen et al. (Xiamen University, Intel Labs)
- **论文**: Learning Generalizable Image Matcher From Internet Videos
- **官方仓库**: [xuelunshen/gim](https://github.com/xuelunshen/gim)
- **许可证**: Apache-2.0
- **特点**: 从互联网视频学习通用匹配器

### 6. OmniGlue (CVPR 2024)
- **作者**: Hanwen Jiang et al. (Google Research, UT Austin)
- **论文**: OmniGlue: Generalizable Feature Matching with Foundation Model Guidance
- **官方仓库**: [google-research/omniglue](https://github.com/google-research/omniglue)
- **许可证**: Apache-2.0
- **特点**: Google 通用特征匹配，ONNX 格式

### 7. Image Matching WebUI
- **作者**: Vincentqyw
- **官方仓库**: [Vincentqyw/image-matching-webui](https://github.com/Vincentqyw/image-matching-webui)
- **许可证**: Apache-2.0
- **特点**: 图像匹配 Web 界面，支持多种算法

### 8. Accelerated Features
- **作者**: Guilherme Potje et al. (UFMG)
- **论文**: XFeat: Accelerated Features for Lightweight Image Matching
- **官方仓库**: [verlab/accelerated_features](https://github.com/verlab/accelerated_features)
- **许可证**: MIT
- **特点**: XFeat 等轻量级特征提取

---

## 📥 权值文件说明

部分项目包含预训练权值文件（.pth, .pt, .ckpt），这些文件较大：

- **DeDoDe**: 3 个权值文件 (~187MB)
- **EfficientSAM**: 权值文件 (~200MB)
- **GIM**: 3 个权值文件 (~170MB)

如果 GitHub 下载慢，可从官方仓库下载：
- [EfficientSAM 权值](https://github.com/yformer/EfficientSAM)
- [DeDoDe 权值](https://github.com/Parskatt/DeDoDe)
- [GIM 权值](https://github.com/xuelunshen/gim)

---

## ⚖️ 版权与使用条款

1. **自研项目** - Image-Matching-Tools 和 Image-Matching-Learning 为原创代码。
2. **第三方项目** - 版权归原作者所有，请支持原作者并给官方仓库 star。
3. **使用限制** - 本仓库仅用于学习和研究目的，请遵循各项目的开源许可证。

---

## 📧 联系方式

- **GitHub**: [@chai1110](https://github.com/chai1110)
- **Email**: chai011379@gmail.com

---

<div align="center">

**如果这个项目对你有帮助，请给一个 ⭐ Star！**

</div>

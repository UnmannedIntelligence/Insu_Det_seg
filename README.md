
# Detection of Missing Insulators in High-Voltage Transmission Lines Using UAV Images

### Repository Overview

This repository provides the experimental resources for our manuscript submitted to *Drones (MDPI)*. It contains source code, experimental data, and aerial inspection videos used for the insulator missing defect detection study.

⚠️ **Note:** At present, only experimental videos are available. The source code and datasets will be uploaded after the manuscript is accepted.





## Abstract

Insulators are essential components in high-voltage transmission lines and require regular inspection to ensure reliable power delivery. Traditional manual inspection methods are inefficient and labor-intensive, highlighting the need for intelligent and automated solutions.

In this study, we propose a missing insulator detection method that integrates Unmanned Aerial Vehicle (UAV) imaging with deep learning techniques.

- Firstly, an improved Faster Region-Based Convolutional Neural Network (Faster R-CNN) is employed to detect and localize insulators in aerial images. Small-sized insulators unsuitable for defect detection are filtered out.
- Secondly, localized insulators are segmented using an improved U-Net to reduce background interference. A bounding-box regression approach is adopted to obtain the minimum enclosing rectangles, and the insulators are aligned vertically.
- Adaptive thresholding is then applied to extract binary images of the insulators, which are further transformed into defect curves for identifying missing insulators.
- To address the limited availability of labeled samples, a transfer learning-based strategy is adopted to improve model generalization.

A dataset of glass insulators was collected using a DJI M300 UAV equipped with an H20T camera along a 330-kV overhead transmission line. The proposed method achieved a detection accuracy of **99.85%**, with improved localization and robustness compared to existing approaches.

Field experiments conducted in real-world scenarios further verify the effectiveness and adaptability of the proposed method.


## Citation

If you find this repository useful in your research, please cite our paper once it is published in *Drones (MDPI)*:

```text
@article{Drones2025ZhangInsuDet,
  author = {Yulong Zhang, Xianghong Xue, Lingxia Mu, Jing Xin, Yichi Yang, Youmin Zhang},
  title = {Detection of Missing Insulators in High-Voltage Transmission Lines Using UAV Images},
  journal = {Drones},
  year = {2026},
  volume = {...},
  pages = {...},
  doi = {...}
}
```

---

## Contact

For questions or collaborations, please contact:

**Yulong Zhang** · [yulong.zhang@stu.xaut.edu.cn](mailto:yulong.zhang@stu.xaut.edu.cn)

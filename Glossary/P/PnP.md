---
type: acronym
full_name: Perspective-n-Point
category:
  - 3D Vision
aliases:
  - Perspective-n-Point
  - n 点透视问题
---

# PnP

**Full Name:** Perspective-n-Point

**中文：** n 点透视问题

## Definition

PnP 是一个几何位姿估计问题。给定相机内参和 $n$ 组 3D 点与 2D 像素的对应关系，求物体或世界坐标系到相机坐标系的旋转 $R$ 和平移 $t$，共 6 个自由度。

## Explanation

许多求解方法会减小[[Reprojection Error|重投影误差]]，让 3D 点的预测投影更接近观测像素。以 OpenCV 的 `solvePnP` 为例，输出满足 $X_c = RX_w + t$。若要得到相机在世界坐标系中的位置，需取逆变换，得到 $-R^\top t$。[OpenCV 文档](https://docs.opencv.org/4.13.0/d5/d1f/calib3d_solvePnP.html)

## Related

- [[Camera Intrinsics]]
- [[6D Pose Estimation]]
- [[Reprojection Error]]
- [[RANSAC]]

## Common Use

常用于相机定位和物体位姿估计。例如，用 CAD 模型上的 3D 角点及其在图像中的 2D 位置，估计物体相对于相机的位姿。

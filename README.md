# Pose-Invariant Face Recognition with VGG16 and ResNet50 on FRMDB

![Face Recognition](https://img.icons8.com/ios/50/000000/face-id.png) ![Deep Learning](https://img.icons8.com/ios-filled/50/000000/neural-network.png) ![CNN](https://img.icons8.com/ios-filled/50/000000/artificial-intelligence.png)

## Overview

This project aims to address a common challenge in **Face Recognition** technology: identifying faces from various angles, particularly in real-world environments like security camera footage. While traditional systems work well with clear, front-facing images, recognizing faces in different poses remains a complex problem.

To solve this, we compare two popular deep learning models:

- **VGG16** ![VGG16](https://img.icons8.com/color/48/000000/vgg16.png)
- **ResNet50** ![ResNet50](https://img.icons8.com/color/48/000000/resnet50.png)

We evaluate these models using a specialized dataset called **FRMDB** (Face Recognition from Mugshots DataBase).

---

## Key Points

1. **Pose-Invariant Face Recognition (PIFR)** is crucial in real-world scenarios, especially for video footage from security cameras.
   
2. Current systems excel in recognizing clear, front-facing images (e.g., for **smartphone unlocking** or **passport verification**) but struggle with different angles or "in-the-wild" conditions.

3. **FRMDB** provides a unique dataset with mugshots from multiple angles, not just the standard front and right-profile views used in police databases.

4. We compare the performance of **VGG16** and **ResNet50**, two widely used **Convolutional Neural Networks (CNNs)**, in recognizing faces from different subsets of mugshots.

5. **Experiment Expansion**: We've expanded our testing beyond previous research, including more identities and additional security camera footage for a more comprehensive evaluation.

---

## Results

By analyzing the performance of VGG16 and ResNet50 on different angles of mugshots, we aim to find the most effective model for **Pose-Invariant Face Recognition** in security applications.

- **VGG16** is known for its simplicity and strong performance on large datasets.
- **ResNet50** introduces residual connections that help with deeper network learning and is highly effective in feature extraction.

---

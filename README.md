# Pose-Invariant Face Recognition Using VGG16 and ResNet50 on FRMDB

![Face Recognition](https://img.icons8.com/ios/50/000000/face-id.png) ![Deep Learning](https://img.icons8.com/ios-filled/50/000000/neural-network.png) ![CNN](https://img.icons8.com/ios-filled/50/000000/artificial-intelligence.png)

## Reseach Paper Link

![Evaluating Deep Neural Networks for Face Recognition with Different Subsets of Mugshots From the Photo-Signaling Procedure](https://ieeexplore.ieee.org/abstract/document/10405736)

## Overview

This project focuses on addressing a key challenge in **Face Recognition**—recognizing faces from different angles (Pose-Invariant Face Recognition or PIFR). The models commonly excel with front-facing images but struggle in real-world conditions, such as security footage where faces are seen from various perspectives.

### Key Facts:
- **Dataset**: We used the **Face Recognition from Mugshots DataBase (FRMDB)**, a specialized dataset that contains mugshots captured from multiple angles.
- **CNN Models**: We evaluated two popular Convolutional Neural Networks (CNNs):
  - **VGG16**: A 16-layer model pre-trained on the VGGFace dataset.
  - **ResNet50**: A 50-layer model that uses residual connections and is pre-trained on VGGFace2.
  
## Experimental Setup

### Mugshots Dataset:

- **Subjects**: The FRMDB dataset includes 39 subjects from previous work and 28 new subjects.
- **Mugshots**: Each subject has **28 mugshots** taken from multiple horizontal and vertical angles.
- **Security Footage**: 
  - **Low-resolution**: 5 videos per subject.
  - **High-resolution**: 3 videos per new subject, 1920 x 1080 pixels.
  
We evaluated face recognition by testing multiple **subsets of mugshots**, including:
  - **Test F**: Only the frontal image.
  - **Test F-L1-R1**: Frontal, left, and right nearest-to-frontal images.
  - **Test 1**: Frontal and right profile image, mimicking traditional police photo-signaling.
  - **Test 6**: The full set of 28 mugshots.

### Evaluation Metrics:
We calculated accuracy based on the model's ability to identify the correct person in:
- **Top-1**: The most similar mugshot or identity.
- **Top-3, Top-5, Top-10**: The person is found within the top 3, 5, or 10 ranked results.

## Results

### VGG16 vs. ResNet50 Performance:

1. **Top-1 Accuracy**:
   - **VGG16**: Achieved **55.7% accuracy** on the new high-resolution dataset (Test 6).
   - **ResNet50**: Reached **62.2% accuracy**, outperforming VGG16.
   
2. **Top-3 Accuracy**:
   - **VGG16**: **75.7%** when using the full set of mugshots (Test 6).
   - **ResNet50**: **75.1%**, slightly lower than VGG16.

3. **Top-10 Accuracy**:
   - **VGG16**: Achieved **95% accuracy** on the new subjects.
   - **ResNet50**: Maintained an accuracy of **92.0%**, showing consistent performance.

### Summary of Findings:
- Both VGG16 and ResNet50 performed best when using the **full set of 28 mugshots**, improving accuracy significantly compared to subsets with fewer angles.
- ResNet50 outperformed VGG16 in **Top-1 accuracy** across both low- and high-resolution footage, indicating better feature extraction capabilities in more challenging conditions.
- Using only frontal and profile images (as in **Test 1**) resulted in the **lowest accuracy**, confirming that diverse angles improve the robustness of face recognition models.

---

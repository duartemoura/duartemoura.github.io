---
title: "Post-Hoc Interpretability of Lung Cancer Nodule Classification"
excerpt: "Exploring gradient-based methods for medical imaging explainability in CT scans. <br/><img src='/images/xai.png' width='500' height='300'>"
collection: portfolio
---

This project laid the groundwork for my research in **explainable AI (XAI)** for medical imaging. Using a **ResNet** model built with **PyTorch Lightning**, I classified lung cancer nodules from **32×32 grayscale CT slices** and evaluated interpretability through gradient-based methods.

---

### Model Training & Performance

**Training Metrics**  
Key training metrics showing model convergence and generalization:

![Train Metrics](/images/training_metrics.png)

**Confusion Matrix**  
Model performance visualized through classification outcomes:

![Confusion Matrix](/images/confusion_matrix.png)

---

### Post-Hoc Interpretability

To understand model decision-making, I applied several **gradient-based XAI techniques** to visualize which image regions influenced predictions. The focus layer for all methods was **Layer 2 (Basic Block Conv2)**.

---

## Grad-CAM

**Misclassification Example**  
A misclassified nodule with incorrect attention focus:

![Misclassification](/images/miscalssification.png)

**Good Interpretation**  
Model highlights the relevant nodule region:

![Good XAI](/images/goodxai.png)

**Bad Interpretation**  
Model focuses on irrelevant areas:

![Bad XAI](/images/badxai.png)

---

## HiRes-CAM

**Misclassification Example**  
Incorrect focus under HiRes-CAM:

![Misclassification - HiRes-CAM](/images/mishires.png)

**Good Interpretation**  
Refined attribution highlighting the lesion:

![Good XAI - HiRes-CAM](/images/goodhires.png)

**Bad Interpretation**  
Attribution is noisy or distracts from the target:

![Bad XAI - HiRes-CAM](/images/badhires.png)

---

## Score-CAM

**Misclassification Example**  
Failure case visualized with Score-CAM:

![Misclassification - Score-CAM](/images/miscore.png)

**Good Interpretation**  
Accurate localization of the nodule:

![Good XAI - Score-CAM](/images/goodscore.png)

**Bad Interpretation**  
Focus deviates significantly from the target:

![Bad XAI - Score-CAM](/images/badscore.png)

---

### Conclusion

This project highlights the strengths and limitations of **post-hoc interpretability methods** in the context of medical imaging. While techniques like Grad-CAM, HiRes-CAM, and Score-CAM provide valuable insights, their outputs can vary in reliability—emphasizing the need for robust and clinically trustworthy XAI in sensitive domains like cancer diagnosis.

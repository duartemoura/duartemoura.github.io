---
title: "LSTM - Time Series Classification Kaggle"
excerpt: "Exploring advanced LSTM architectures with attention mechanisms for effective time series classification on Kaggle. Winner of the competition. <br/><img src='/images/lstm.png' width='500' height='300'>"
collection: portfolio
---

In this project, we designed and implemented a pipeline to tackle the challenges of Time Series Classification (TSC), leveraging deep learning techniques. The final model was an LSTM with masking and attention mechanisms, optimized for handling imbalanced datasets and complex temporal dependencies.

### Key Highlights

#### 1. Data Preprocessing and Feature Engineering
- **Handling Missing Values:** Interpolation with a linear method preserved temporal continuity.
- **Feature Engineering:** Introduced rolling statistics (mean, standard deviation) for richer temporal insights, creating a 3D representation per sample.

#### 2. Data Augmentation
- Used `tsaug` to balance class distributions, outperforming traditional methods like SMOTE for time-series data.

#### 3. Model Architecture
- **Bidirectional LSTM with Attention:** Focused on relevant time steps to enhance classification accuracy.
- **Masking & Padding:** Ensured the model efficiently processed variable-length sequences.

#### 4. Results and Challenges
- **High Accuracy:** Achieved robust performance despite initial class imbalance.
- **Overfitting Mitigation:** Explored model simplification techniques, balancing complexity and performance.

![Training Loss Chart](/images/loss.png)

#### 5. Future Work
- Investigate dimensionality reduction with autoencoders.
- Leverage variational autoencoders (VAEs) to synthesize realistic minority class samples.

You can view additional the full report here: [Time Series Classification Project](/files/Kaggle_report-1.pdf).

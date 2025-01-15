---
title: "Calibration CNNs"
excerpt: "Implementation of the paper On calibration of Modern Neural Networks using bird and cat images of the CIFAR-10 dataset <br/><img src='/images/birds_cats.png' width='500' height='300'>"
collection: portfolio
---

In this project, I delve into the calibration of Convolutional Neural Networks (CNNs) to ensure that their predicted probabilities accurately reflect true correctness likelihoods. This involves implementing techniques such as Expected Calibration Error (ECE) and Temperature Scaling, as discussed in the paper "On Calibration of Modern Neural Networks". The experiments utilize the CIFAR-10 dataset to evaluate and enhance the calibration of CNN models, aiming to align predicted confidences with actual accuracies.

<div style="text-align: center;">
  <img src="/images/LENET_combined_reliability.png" alt="Combined Reliability Diagram" width="600">
  <p><em>Combined Reliability Diagram illustrating the empirical probability versus mean predicted probability for varying temperature values (T). The dashed line represents perfect calibration.</em></p>
</div>


You can explore the project's code and detailed report here: [Calibration of CNNs](https://github.com/duartemoura/calibrating_nn)
---
layout: page
title: Traffic Optimization with Deep Reinforcement Learning
description: Using Amazon SageMaker to train a Reinforcement Learning model for traffic signal optimization in SUMO simulations.
img: assets/img/sumo.png
importance: 1
category: aws
related_publications: false
---

In this project, we employed a Deep Q-Network (DQN) agent to optimize traffic flow within the SUMO (Simulation of Urban MObility) environment. Our work is based on the foundational model from [Andrea Vidali's repository](https://github.com/AndreaVidali/Deep-QLearning-Agent-for-Traffic-Signal-Control/tree/master). Expanding on this base, we implemented a comprehensive solution using AWS infrastructure, encompassing data preprocessing, model training, and deployment.

The DQN agent was trained using Amazon SageMaker, taking advantage of its powerful machine learning capabilities. To simulate real-world scenarios, we replicated data ingestion from IoT devices and applied advanced preprocessing techniques with AWS analytics services. This robust setup empowered the reinforcement learning model to make data-driven decisions, ultimately improving traffic signal management and reducing congestion.

Our project focuses specifically on optimizing the timing of traffic light state changes, transitioning from fixed schedules to a dynamic, adaptive system. This approach ensures more efficient traffic flow and reduces delays in urban environments.

<div style="text-align: center;">
  <img src="/assets/img/wsa.png" alt="Optimized Traffic Simulation" width="600">
  <p><em>Architecture of the pipeline.</em></p>
</div>

This project was proudly selected to be showcased at AWS Re:Invent 2024, highlighting its innovation and real-world impact.

Explore the full workshop for step-by-step guidance: [Traffic Optimization with Deep RL](https://catalog.us-east-1.prod.workshops.aws/workshops/4cfe9329-1004-4583-8393-0ce6d194b973/en-US/2-introduction)

<div style="text-align: center;">
  <img src="/assets/img/final_model_cars.gif" alt="Optimized Traffic Flow" width="600">
  <p><em>Simulation Comparison: Optimized traffic (right) vs. default settings (left).</em></p>
</div>

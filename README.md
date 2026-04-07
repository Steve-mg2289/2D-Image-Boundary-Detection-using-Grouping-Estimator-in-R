## 📌 Project Description

This project implements and compares two methods for estimating boundaries in two-dimensional (2D) image data using **R**: the classical **Probit Maximum Likelihood Estimator (MLE)** and a **Grouping Estimator**, based on the research paper *“An Analysis of Two-Dimensional Image Data Using a Grouping Estimator” (2022)*.

In many real-world image analysis problems, it is essential to divide a space into two regions (e.g., object vs. background). While traditional statistical models like probit regression assume a specific distribution of errors, they can produce biased results when this assumption is incorrect. To address this limitation, this project explores the grouping estimator—a semiparametric approach that does not rely on distributional assumptions.

The project simulates 2D image data under different conditions (normal, Cauchy, and heteroscedastic noise) and evaluates how well each method estimates the true boundary between regions. The grouping estimator works by partitioning the data into grids, computing summary statistics within each group, and then applying a probit model on the aggregated data.

### 🎯 Objectives

* Simulate high-resolution 2D image data with stochastic noise
* Implement and compare:

  * Probit regression (MLE)
  * Grouping estimator
* Analyze the impact of distribution misspecification
* Visualize and compare estimated boundaries
* Reproduce key findings from the research paper

### 🔍 Key Insight

The grouping estimator reduces the resolution of the data through aggregation, making it more robust to noise and model misspecification. This project demonstrates that, under non-ideal conditions, the grouping estimator can outperform traditional methods in estimating boundaries.

### 🛠️ Tools & Technologies

* R (base + packages like `dplyr`, `ggplot2`)
* Statistical modeling (GLM – probit link)
* Simulation and Monte Carlo experiments

### 📊 Expected Outcome

A reproducible R-based workflow that shows how grouping-based methods can improve boundary estimation in noisy 2D image data, along with visual and quantitative comparisons between methods.

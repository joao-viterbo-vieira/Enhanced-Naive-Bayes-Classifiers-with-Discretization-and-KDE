# Enhanced Naive Bayes Classifiers with Discretization and KDE

This project explores advanced methods to improve Naive Bayes classifiers by incorporating discretization techniques and Kernel Density Estimation (KDE). Completed as part of the **Machine Learning and Data Mining** course in the Master’s program in Data Science and Engineering, the project achieved a grade of **19.2/20**.

---

## Project Overview

### Objectives

- To evaluate the effectiveness of discretization techniques, such as equal width and equal depth binning, in enhancing Multinomial and Gaussian Naive Bayes classifiers.
- To assess the potential of KDE Naive Bayes as a flexible and robust alternative for handling continuous features.
- To compare the performance of these models using rigorous metrics such as **ROC curves** and cross-validation.

### Key Highlights

- Discretization improves the performance of Multinomial Naive Bayes classifiers by simplifying continuous features, reducing noise, and better capturing feature relationships.
- Discretization leads to worse performance in Gaussian Naive Bayes, as the assumption of normality conflicts with discretized data.
- KDE Naive Bayes surpasses Gaussian Naive Bayes by effectively capturing complex and multimodal distributions in continuous data.

---

## Notebook Contents

### 1. Data Preparation

- **1.1 Load Dataset**: Initial exploration and loading of datasets.
- **1.2 Preprocessing**:
  - Handling missing values.
  - Encoding categorical data for compatibility with Naive Bayes models.

### 2. Enhancing Naive Bayes Classifiers

#### 2.1 Multinomial Naive Bayes (MNB)

- Applied discretization techniques:
  - **Equal Width Discretization**: Divides the range of a continuous variable into equal-width intervals.
  - **Equal Depth Discretization**: Divides the data into bins with equal frequencies.
- Evaluated performance improvements through cross-validation and ROC analysis.

#### 2.2 Gaussian Naive Bayes (GNB)

- Tested with the same discretization techniques to analyze their impact on a continuous data model.
- Found that discretization led to worse results due to GNB’s reliance on normality for continuous features.

#### 2.3 KDE Naive Bayes

- Introduced KDE Naive Bayes to handle continuous features without discretization.
- Leveraged kernel density functions to approximate feature distributions by smoothing data points, enabling KDE Naive Bayes to handle complex and multimodal distributions.
- Compared KDE Naive Bayes with Gaussian Naive Bayes through 10-fold cross-validation and hyperparameter tuning.

### 3. Results and Insights

- **Performance Metrics**:
  - ROC Curves: Evaluated classifier performance across thresholds.
  - Cross-Validation: Assessed robustness and generalization.
- **Comparative Analysis**:
  - Discretization improved Multinomial Naive Bayes but worsened Gaussian Naive Bayes.
  - KDE Naive Bayes outperformed Gaussian Naive Bayes in continuous data scenarios.

### 4. Conclusions and Recommendations

- Discretization boosts the performance of Multinomial Naive Bayes.
- KDE Naive Bayes is a robust alternative for continuous data, offering better adaptability compared to Gaussian Naive Bayes.
- Recommendations for future work include exploring hybrid approaches and applying these methods to diverse datasets.

---

## Key Takeaways

- **Discretization Techniques**:
  - Equal width and equal depth binning enhance the compatibility and effectiveness of Multinomial Naive Bayes.
- **KDE Naive Bayes**:
  - Offers a flexible and robust alternative to Gaussian Naive Bayes by better modeling continuous features.
- **Systematic Evaluation**:
  - Rigorous testing using cross-validation and ROC analysis highlights the practical advantages of these methods.

---

## Future Work

- Explore hybrid models combining discretization with KDE techniques.
- Apply these methods to larger, more diverse datasets to test scalability and robustness.
- Investigate the integration of other feature engineering techniques for further performance improvements.

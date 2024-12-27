# Enhanced Naive Bayes Classifiers with Discretization and KDE

This project explores advanced techniques to improve the performance of Naive Bayes classifiers. By incorporating discretization methods and introducing Kernel Density Estimation (KDE), the project evaluates the impact of these enhancements on classification accuracy and robustness. Completed as part of the **Machine Learning and Data Mining** course in the Master’s program in Data Science and Engineering, this project achieved a grade of **19.2/20**.

---

## Project Overview

### Objectives

- To evaluate the effectiveness of discretization techniques, such as equal width and equal depth binning, in enhancing Multinomial and Gaussian Naive Bayes classifiers.
- To assess the potential of KDE Naive Bayes as a flexible and robust alternative for handling continuous features.
- To compare the performance of these models using rigorous metrics such as **ROC curves** and cross-validation.

### Key Highlights

- Discretization improves the performance of Naive Bayes classifiers by transforming continuous features into discrete intervals, which simplifies the data structure and reduces noise, making the classifiers more efficient and effective in capturing feature relationships.
- KDE Naive Bayes surpasses Gaussian Naive Bayes in capturing complex feature distributions, offering improved adaptability for continuous data.
- Systematic evaluation demonstrates the trade-offs and advantages of these techniques across different scenarios.

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
- Conducted detailed comparisons of accuracy and ROC curves.

#### 2.3 KDE Naive Bayes

- Introduced KDE Naive Bayes to handle continuous features without discretization.
- Leveraged kernel density functions to better approximate feature distributions by smoothing data points and creating a non-parametric estimate of the probability density function. This approach allows KDE Naive Bayes to capture complex and multimodal distributions that Gaussian Naive Bayes, with its assumption of normality, may fail to model effectively.
- Compared KDE Naive Bayes with Gaussian Naive Bayes through 10-fold cross-validation and hyperparameter tuning.

### 3. Results and Insights

- **Performance Metrics**:
  - ROC Curves: Evaluated classifier performance across thresholds.
  - Cross-Validation: Assessed robustness and generalization.
- **Comparative Analysis**:
  - Demonstrated the advantages of discretization for both Multinomial and Gaussian Naive Bayes models.
  - Highlighted the superiority of KDE Naive Bayes in scenarios with complex data distributions.

### 4. Conclusions and Recommendations

- Discretization significantly boosts the performance of Naive Bayes classifiers, especially for categorical data.
- KDE Naive Bayes is a robust choice for continuous data, outperforming Gaussian Naive Bayes in various cases.
- Recommendations for future work include exploring hybrid approaches and applying these methods to real-world datasets.

---

## Key Takeaways

- **Discretization Techniques**:
  - Equal width and equal depth binning enhance the compatibility and effectiveness of Naive Bayes models.
- **KDE Naive Bayes**:
  - Offers a flexible and robust alternative to Gaussian Naive Bayes by better modeling continuous features.
- **Systematic Evaluation**:
  - Rigorous testing using cross-validation and ROC analysis highlights the practical advantages of these methods.

---

## Future Work

- Explore hybrid models combining discretization with KDE techniques.
- Apply these methods to larger, more diverse datasets to test scalability and robustness.
- Investigate the integration of other feature engineering techniques for further performance improvements.

---


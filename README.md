## Abstract

The idea is to predict if a customer will accept the coupon or not by learning algorithms from the scratch (except neural networks) using Python. 
Logistic regression, Neural Networks, SVM, and Naive Bayes are implemented, tuned, and measured by performance metrics such as accuracy, time consumption, 
and peak memory usage. Meanwhile, the tradeoff between overfitting and underfitting is considered to ensure output robustness. 
The result shows that Neural Networks achieve the best test accuracy of ~74% and Hard-Margin SVM takes the least time and memory. 
This project can serve as a reference for corporations to distribute coupons to target customers with higher acceptance demand, thus boosting their revenues.

[Dataset](https://archive.ics.uci.edu/ml/datasets/in-vehicle+coupon+recommendation): 12684 records, 26 attributes

See **Data Preprocessing, Model implemeantation** in Machine_Learning_Models.ipynb

For hyperparameter tuning, we adopted the following strategies, 
<img src="https://user-images.githubusercontent.com/49282511/208027821-bcd40a5b-40d4-4ce4-a324-04b2dca90872.png"  width="60%" height="45%">

Model Performance Comparison

- Accuracy
<img src="https://user-images.githubusercontent.com/49282511/208027758-df8d39a7-9d1f-4c5a-a658-800fac7a5f05.png"  width="52.5%" height="40%">

- Process Time & Peak Memory Usage among the best tuned models

| Models | Process Time(s) | Peak Memory Usage(MB) |
|:---| :----: | ---: |
| Logistic Regression | 50 | 13.5 |
| Gaussian Naive Bayes | 339 | 13.9|
| Hard SVM | 136 | 4.5 |
| Nueral Network | 884 | 14 |


## Future Work
- Neural network is overfitting, consider the bias-variance tradeoff when conducting hyperparameters tuning. 
- The current hyperparameter tuning way may be unstable for the greedy strategy. Do research on optimized tuning style.
- Continue with soft-SVM using SMO with powerful GPU for accelarated training process.

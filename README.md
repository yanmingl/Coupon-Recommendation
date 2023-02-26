## Abstract

The objective of this project is to develop machine learning models using Python to predict whether customers will accept a coupon or not. To achieve this goal, we implemented Logistic Regression, Support Vector Machines (SVM), Naive Bayes, and Neural Networks. These models were carefully tuned and evaluated based on performance metrics such as accuracy, time consumption, and peak memory usage. Moreover, we considered the tradeoff between overfitting and underfitting to ensure the robustness of our output.

Our results indicate that Neural Networks achieved the best test accuracy of approximately 74%, while Hard-Margin SVM exhibited the least time and memory consumption. Our findings can serve as a useful reference for businesses looking to distribute coupons to target customers with higher acceptance rates, leading to increased revenues.

Overall, this project demonstrates the effectiveness of various machine learning algorithms in predicting customer behavior. By leveraging these models, businesses can make informed decisions about their marketing strategies, ultimately leading to improved profitability.

## Method
### [Dataset](https://archive.ics.uci.edu/ml/datasets/in-vehicle+coupon+recommendation)
12684 records, 26 attributes

### Code
See **Data Preprocessing, Model implemeantation** in `Code.ipynb`

### Hyperparameter Tuning Strategy
<img src="https://user-images.githubusercontent.com/49282511/208027821-bcd40a5b-40d4-4ce4-a324-04b2dca90872.png"  width="70%" height="45%">

## Model Performance Comparison

- Accuracy
<img src="https://user-images.githubusercontent.com/49282511/208027758-df8d39a7-9d1f-4c5a-a658-800fac7a5f05.png"  width="70%" height="40%">

- Process Time & Peak Memory Usage among the best tuned models

| Models | Process Time(s) | Peak Memory Usage(MB) |
|:---| :----: | ---: |
| Logistic Regression | 50 | 13.5 |
| Gaussian Naive Bayes | 339 | 13.9|
| Hard SVM | 136 | 4.5 |
| Nueral Network | 884 | 14 |


## Future Work
- It has come to our attention that the neural network model is overfitting the data. As such, we need to consider the bias-variance tradeoff when conducting hyperparameter tuning to improve the model's generalization performance.

- The current hyperparameter tuning method may be unstable due to its greedy strategy. We plan to conduct research on an optimized tuning style that can yield better results.

- We will continue with the soft-SVM model using Sequential Minimal Optimization (SMO) and a powerful GPU to accelerate the training process. This approach can help us overcome the challenges of dealing with large datasets and complex decision boundaries. We expect this model to yield better results than the neural network model, given its ability to handle high-dimensional data with less overfitting.

By doing so, we hope to provide businesses with more reliable predictions and better guidance for their coupon distribution strategies.

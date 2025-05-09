<H1>Breast Cancer Recurrence Prediction</H1>
This project explores data preprocessing, visualization, and classification models to predict breast cancer recurrence using a dataset of patient records. The workflow includes cleaning the data, one-hot-encoding, and applying machine learning models (K-Nearest Neighbors and Logistic Regression) for binary classification.

<H2>Dataset</H2>
The dataset (cancer.csv) contains anonymized patient records with the following features:

- class: Target variable (recurrence-events or no-recurrence-events)
- age, menopause, tumor-size, inv-nodes, node-caps, deg-malig, breast, breast-quad, irradiat
Size: 386 samples, 10 features

<H2>Results Summary</H2>

| Model                   | Accuracy | Notes                                                      |
| ----------------------- | -------- | ---------------------------------------------------------- |
| KNN (k=3)               | 59%      | Weak performance, especially on the minority class         |
| KNN (Grid Search, k=13) | **72%**  | Best overall accuracy, but low recall for recurrence cases |
| Logistic Regression     | 65%      | Better balance, but weak performance on minority class     |

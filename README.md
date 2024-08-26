# Churn Prediction with Logistic Regression

This project demonstrates the use of Logistic Regression to predict customer churn based on various features. The dataset is sourced from IBM's Developer Skills Network and is used to build and evaluate a classification model.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Features](#features)
- [Modeling](#modeling)
- [Evaluation](#evaluation)
- [How to Use](#how-to-use)
- [Contributing](#contributing)
- [Acknowledgments](#acknowledgments)
- [License](#license)

## Introduction

Customer churn is a critical metric for businesses to monitor, as it indicates the loss of customers over time. This project uses a Logistic Regression model to predict the likelihood of a customer churning based on various factors such as tenure, age, income, and more.

## Dataset

The dataset used in this project contains the following features:

- **tenure**: Number of months the customer has stayed with the company
- **age**: Customer's age in years
- **address**: Number of years the customer has lived at their current address
- **income**: Annual income of the customer
- **ed**: Level of education of the customer
- **employ**: Number of years the customer has been employed
- **equip**: Binary feature indicating whether the customer has the equipment
- **churn**: Target variable indicating if the customer churned (1) or not (0)

## Features

The features are normalized using `StandardScaler` to ensure that the Logistic Regression model performs optimally.

## Modeling

The Logistic Regression model is built using the following steps:

1. **Data Preparation**: The dataset is loaded, and the relevant features are selected.
2. **Feature Normalization**: The features are normalized to have a mean of 0 and a standard deviation of 1.
3. **Train-Test Split**: The dataset is split into training and testing sets with a ratio of 80:20.
4. **Model Training**: The Logistic Regression model is trained using the training set.
5. **Prediction**: The model is used to predict the churn status of customers in the test set.

## Evaluation

The model's performance is evaluated using the following metrics:

- **Jaccard Index**: A similarity measure between the predicted and actual labels.
- **Confusion Matrix**: A matrix showing the true positive, true negative, false positive, and false negative counts.
- **Classification Report**: A detailed report showing precision, recall, F1-score, and support for each class.
- **Log Loss**: A metric to evaluate the accuracy of probabilistic predictions.

The confusion matrix is also visualized to provide a clearer understanding of the model's performance.

## How to Use

1. Clone this repository to your local machine.
2. Ensure that you have the required libraries installed:
    - `requests`
    - `pandas`
    - `numpy`
    - `matplotlib`
    - `scikit-learn`
3. Run the script to download the dataset, preprocess the data, train the model, and evaluate its performance.

```bash
git clone https://github.com/idaraabasiudoh/churn-prediction.git
cd churn-prediction
python churn_prediction.py
```

## Contributing

Contributions are welcome! If you would like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-branch-name`
3. Make your changes and commit them: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature-branch-name`
5. Submit a Pull Request.

Please ensure your code adheres to the project’s coding standards and includes appropriate tests.

## Acknowledgments

I would like to thank the IBM Developer Skills Network for providing the dataset and resources that made this project possible. Special thanks to the course instructors of the IBM Machine Learning course on Coursera for their valuable insights and guidance throughout the project.

## License

This project is licensed under the MIT License. You are free to use, modify, and distribute this software in compliance with the License. See the [LICENSE](LICENSE) file for more details.

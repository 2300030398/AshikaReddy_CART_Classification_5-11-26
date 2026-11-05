# CART Classification Using the Tennis Dataset

## Project Overview
This project implements a **CART (Classification and Regression Trees) classification model** using the classic Tennis dataset. The model predicts whether a person will play tennis based on weather conditions such as Outlook, Temperature, Humidity, and Wind.

CART uses binary splits and Gini impurity to select the best features for classification.

## Dataset
The Tennis dataset contains 14 records with the following features:

| Feature | Description |
|---|---|
| Outlook | Weather condition: Sunny, Overcast, Rain |
| Temperature | Temperature: Hot, Mild, Cool |
| Humidity | Humidity: High, Normal |
| Wind | Wind condition: Weak, Strong |
| PlayTennis | Target: Yes or No |

## Technologies Used
- Python
- Pandas
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Implementation Steps
1. Import the required libraries.
2. Create and load the Tennis dataset.
3. Convert categorical values into numerical values using LabelEncoder.
4. Separate input features (`X`) and target (`y`).
5. Split the dataset into training and testing data.
6. Train the CART classification model using `DecisionTreeClassifier`.
7. Predict the test results.
8. Evaluate the model using accuracy, confusion matrix, and classification report.
9. Visualize the decision tree.

## Model
```python
from sklearn.tree import DecisionTreeClassifier

cart_model = DecisionTreeClassifier(
    criterion="gini",
    random_state=42
)

cart_model.fit(X_train, y_train)
```

## Evaluation Metrics
The model is evaluated using:
- **Accuracy:** Overall correct predictions.
- **Confusion Matrix:** Correct and incorrect predictions by class.
- **Precision:** How many predicted positive cases are actually positive.
- **Recall:** How many actual positive cases are correctly identified.
- **F1-score:** Balance between precision and recall.



## Conclusion
This project demonstrates how CART classification works using the Tennis dataset. It shows how a decision tree learns from weather conditions and predicts whether tennis should be played.

The dataset is small, so the results are intended for learning and practice rather than real-world performance evaluation.

# Classifier Comparison on Digits Dataset

This project demonstrates how to train and compare several simple classifiers on the **Digits dataset** provided by `scikit-learn`. It is designed as an educational exercise for understanding basic classification models, data splitting, scaling, and performance evaluation.

---

## Dataset

We use the `load_digits()` dataset which contains images of handwritten digits (0-9), represented as 64 features (8x8 pixels).

- **Samples:** 1797
- **Features:** 64
- **Task:** Multi-class classification (10 classes: digits 0 to 9)

---

## Classifiers Compared

We trained and evaluated the following models:

1. **DecisionTreeClassifier**  
2. **KNeighborsClassifier**  
3. **LogisticRegression**

All classifiers were trained on the same dataset using an 80%/20% train/test split.

---

## Data Preparation

- The dataset was split into:
  - **80% Training set**  
  - **20% Testing set**
- **Feature scaling** was applied using `StandardScaler` (important for KNN and Logistic Regression).
- Each model was evaluated by calculating its accuracy on both training and testing sets.

---

## Results Summary

| Classifier         | Train Accuracy | Test Accuracy |
|---------------------|----------------|----------------|
| Decision Tree       | Very High (Perfect on training) | Lower on testing |
| K-Nearest Neighbors | High           | High           |
| Logistic Regression | High           | High           |

### Key observations:

- **Decision Tree:** Overfitting occurred. The model perfectly memorized the training data but generalized poorly on unseen data.
- **K-Nearest Neighbors:** Performed well, showing good generalization due to its nature and proper scaling.
- **Logistic Regression:** Delivered stable and strong performance, proving to be a very reliable baseline model.

---

## Technologies Used

- Python 3.x
- scikit-learn
- Jupyter Notebook
- pandas

---

## How to Run

1. Clone this repository or download the provided `.ipynb` notebook file.
2. Open `classifier_comparison_extended.ipynb` in **Jupyter Notebook** or **Google Colab**.
3. Run all cells to reproduce the results.

---

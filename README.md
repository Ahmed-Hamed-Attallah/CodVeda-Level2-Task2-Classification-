# Iris Flower Classification 🌸

A machine learning project to classify iris flowers into three species based on their sepal and petal measurements using Logistic Regression, Random Forest, and Support Vector Machines (SVM).

## 📖 Project Overview

This project implements and compares three classic machine learning algorithms on the famous Iris dataset. The goal is to predict the species of an iris flower (`setosa`, `versicolor`, or `virginica`) from four numerical features: sepal length, sepal width, petal length, and petal width.

The models evaluated are:
- **Logistic Regression**
- **Random Forest Classifier**
- **Support Vector Classifier (SVM)**

## 📊 Dataset

The dataset used is the **Iris dataset**, a classic benchmark in pattern recognition. It contains 150 samples with 4 features each:

**Features:**
- `sepal_length` (cm)
- `sepal_width` (cm)
- `petal_length` (cm)
- `petal_width` (cm)

**Target:**
- `species` (`setosa`, `versicolor`, `virginica`)

### Jupyter Notebook
Alternatively, you can open and run the `Classification with Logistic Regression.ipynb` Jupyter Notebook to execute the code step-by-step.

### What the code does:
1.  **Loads and Preprocesses Data:** Handles label encoding and feature scaling.
2.  **Splits the Data:** 80% for training, 20% for testing.
3.  **Trains Models:** Fits Logistic Regression, Random Forest, and SVM models.
4.  **Evaluates Performance:** Calculates accuracy, precision, recall, and plots a confusion matrix and multi-class ROC curves.

## 📈 Results

### Model Performance Summary
| Model | Accuracy | Precision | Recall |
| :--- | :---: | :---: | :---: |
| **Logistic Regression** | 93.3% | 0.933 | 0.933 |
| **Random Forest** | 93.3% | 0.933 | 0.933 |
| **Support Vector Machine (SVM)** | **96.7%** | **0.970** | **0.967** |

### Key Findings
- The **SVM model performed best** on the test set.
- All models achieved a **Micro-Average AUC score of 0.99 or 1.00**, indicating excellent overall classification performance.
- The primary source of error is misclassifying between the `versicolor` and `virginica` species, which are more similar to each other than to `setosa`.

**Confusion Matrix (Logistic Regression):**
| | Predicted: 0 | Predicted: 1 | Predicted: 2 |
| :--- | :---: | :---: | :---: |
| **Actual: 0** | 10 | 0 | 0 |
| **Actual: 1** | 0 | 9 | 1 |
| **Actual: 2** | 0 | 0 | 10 |


## 🔮 Future Work

- Hyperparameter tuning using GridSearchCV for each model.
- Experimenting with other algorithms (e.g., K-Nearest Neighbors, Gradient Boosting).
- Implementing k-Fold Cross-Validation for more robust performance metrics.
- Deploying the best model as a simple web application with Flask or Streamlit.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- The Iris dataset is a classic dataset originally published by R.A. Fisher.
- Built with Python's amazing data science ecosystem.

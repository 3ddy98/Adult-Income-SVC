Here’s a sample README for your GitHub repository, highlighting the main functionality of the code:

---

# Income Classification using Machine Learning

This repository contains code to classify income level (<=50K or >50K) using various machine learning models, including **Support Vector Machines (SVM)** and **Random Forest Classifier (RFC)**. The project demonstrates data preprocessing, feature encoding, model training, and evaluation.

## Features

- **Data Loading and Preprocessing**: Loads data from `adult.data` and `features.csv` and applies ordinal encoding to categorical variables.
- **Exploratory Data Analysis**: Examines the dataset to handle missing values and checks the distribution of numerical features.
- **Modeling**: Uses `SVM` and `Random Forest` classifiers, with hyperparameter tuning for `SVM` using `GridSearchCV`.
- **Model Evaluation**: Evaluates model performance using metrics such as accuracy and AUC, and plots ROC curves to compare SVM and RFC.

## Requirements

This project requires the following Python libraries:
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`

Install the necessary packages using:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

## Usage

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/income-classification.git
   ```

2. Run the main code file to preprocess data, train models, and evaluate results:
   ```python
   python main.py
   ```

3. Visualize performance metrics:
   - **Scatter Plot of SVM Results**: Plots SVM scores for different `C` values.
   - **AUC Curve for SVM vs RFC**: Compares the ROC curves of SVM and RFC.

## Key Results

- **Best SVM Parameters**: The best `C` value found via Grid Search was `4.0` with a `rbf` kernel.
- **Model Performance**:
  - **SVM**: Accuracy on test set - ~85%
  - **RFC**: Performance similar to SVM in ROC/AUC comparison.

## Visualization

- **Feature Pair Plot**: Visualizes relationships between features using Seaborn pair plots.
- **ROC Curve**: Displays ROC curves comparing SVM and RFC classifiers.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

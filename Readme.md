# Student Score Prediction

This project predicts student performance using various machine learning approaches, exploring how feature selection, scaling, and polynomial transformations impact model performance.

## **Dataset**
- [Students Performance Dataset](https://www.kaggle.com/datasets/rabieelkharoua/students-performance-dataset)
- Contains a mix of categorical and numerical features, including:
  - Age
  - Study Time Weekly
  - Absences
  - GPA 
  - GradeClass (target)


## **Exploratory Data Analysis (EDA)**
- **No null or duplicate values** were found.
- Dataset includes both **categorical** and **numerical** features.
- Visualizations:
  - **Correlation Heatmap** to show relationships between features.
  - **Histogram Plots** for distribution analysis of numerical variables.

## **Data Preprocessing**
- **Scaling** applied to numerical features (MinMaxScaler / StandardScaler).
- **Categorical features** encoded appropriately (Label/One-Hot Encoding).
- Created train-test splits for model evaluation.

## **Model Training**
Several models were tested:

1. **Linear Regression** (baseline)
2. **Linear Regression with Selected Features** (dropping less important ones)
3. **Polynomial Regression (without scaling)**
4. **Polynomial Regression (with scaling)**

## **Results**
- Model performance evaluated using:
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
  - Mean Absolute Error (MAE)
  - R² Score

**Best Result**:  
- Achieved by **Polynomial Regression with Scaling**, indicating that feature scaling significantly improved performance for higher-order features.

## **Usage**
Clone the repository:
```bash
git clone https://github.com/ubadakhan/class-grade-prediction.git
cd class grade prediction

python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
pip install -r requirements.txt

jupyter notebook main.ipynb

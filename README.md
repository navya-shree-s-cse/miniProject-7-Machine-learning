# miniProject-7-Machine-learning
# QuickCart Stockout Risk Prediction
### Minor Project – 07

## 1. Project Overview
QuickCart Stockout Risk Prediction is a Machine Learning project that predicts the risk of products going out of stock across different stores.

The project helps identify products with high stockout risk so that businesses can manage inventory efficiently, avoid lost sales and improve stock availability.

## 2. Problem Statement
QuickCart has 12 stores, 60 products and 15 suppliers. Running out of stock results in lost sales, while ordering excess products increases storage costs.

This project predicts the stockout risk for each product, store and day using Machine Learning techniques.

## 3. Objectives
- Analyze daily inventory data.
- Identify stockout risk levels.
- Study the impact of festivals on stock availability.
- Analyze supplier reliability.
- Compare different Machine Learning models.
- Predict stockout risk accurately.
- Help businesses make better inventory decisions.

## 4. Dataset Description

The project uses five CSV files:

| Dataset | Number of Rows |
|---|---:|
| dim_stores.csv | 12 |
| dim_skus.csv | 60 |
| dim_suppliers.csv | 15 |
| dim_events.csv | 30 |
| fact_inventory_daily.csv | 21,600 |

**Target Variable:** `stockout_risk`

It contains three categories:
- Safe
- At-Risk
- Imminent

## 5. Technologies Used
- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Machine Learning

## 6. Project Workflow
1. Import required libraries.
2. Load all five CSV datasets.
3. Check dataset size and missing values.
4. Clean and preprocess the data.
5. Merge datasets into one combined dataset.
6. Perform Exploratory Data Analysis (EDA).
7. Analyze festival effects and supplier reliability.
8. Create new features for prediction.
9. Split data into training and testing sets.
10. Apply data preprocessing.
11. Train Machine Learning models.
12. Compare model performance.
13. Generate predictions and visualize results.

## 7. Machine Learning Algorithms

Three models are used:

1. **Dummy Classifier:** Baseline model for comparison.
2. **Logistic Regression:** Classification model with balanced class weights.
3. **Random Forest Classifier:** Ensemble learning model used to predict stockout risk.

## 8. Evaluation Metrics
The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

Special importance is given to **Imminent Recall**, because missing an actual stockout is costly.

## 9. Key Findings
- Safe is the largest stockout-risk category.
- Imminent is the smallest category.
- Festival periods affect stockout risk.
- Supplier reliability plays an important role in stock availability.
- Random Forest achieves the highest Imminent Recall according to the notebook's conclusion.
- The notebook reports an Imminent Recall of 0.985 (98.5%).

## 10. Conclusion
The QuickCart Stockout Risk Prediction project uses Machine Learning to identify products that may go out of stock.

Among the evaluated models, Random Forest performs best according to Imminent Recall. The analysis also highlights the importance of festival periods and supplier reliability.

This project helps businesses improve inventory planning, maintain sufficient stock and reduce potential sales losses.

## 11. How to Run the Project

1. Install Python.
2. Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

3. Keep the Jupyter Notebook and all five CSV files in the same folder.
4. Open Jupyter Notebook.
5. Open `QuickCartStockoutRisk_MinorProject7_navya.ipynb`.
6. Run all cells sequentially.
7. View the visualizations, model comparison and predictions.

---
**Project Name:** QuickCart Stockout Risk Prediction  
**Project Type:** Minor Project  
**Domain:** Machine Learning and Data Analytics  
**Language:** Python
**Author:** Navyashree S

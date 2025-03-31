# Sales Prediction Analysis

![Image](https://github.com/Jatin-s16/Sales-Prediction-Dataset/blob/main/sales-forecast-illustration-wooden-table-260nw-463853141.webp)

## Project Overview
This project analyzes how advertising expenditures (TV, Radio, Newspaper) impact product sales using linear regression. The analysis answers key business questions and evaluates different modeling approaches.

## Business Questions and Results

### 1. What is the average amount spent on TV advertising?
**Result:**  
The average expenditure on TV advertising was **$147.04**  
*This indicates TV receives the largest share of the advertising budget.*

### 2. What is the correlation between radio advertising and product sales?
**Result:**  
The correlation between Radio advertising and Sales is **0.35**  
*This moderate positive correlation suggests radio ads have some impact on sales.*

### 3. Which advertising medium has the highest impact on sales?
**Result:**  
**TV advertising** has the strongest correlation with sales (0.90)  
*This strong correlation indicates TV ads are the most effective medium for driving sales.*

### 4. Linear Regression Model Performance
**Results:**  
- R-squared: 0.906 
- Mean Squared Error: 2.90  
- Root Mean Squared Error: 1.70  

**Key Coefficients:**
- TV: 0.0545 (most significant)
- Radio: 0.1010
- Newspaper: -0.0043 

*The model explains 89.9% of sales variance, with TV being the most influential predictor.*

![Image](https://github.com/Jatin-s16/Sales-Prediction-Dataset/blob/main/predicted_sales.png)
*Visualization shows strong alignment between predicted and actual sales*

### 5. Sales Prediction for New Expenditures
**Input:**  
- TV: $200  
- Radio: $40  
- Newspaper: $50  

**Predicted Sales:** **19.87 units**  
*This helps budget allocation decisions for optimal sales impact.*

### 6. Effect of Normalization
**Result:**  
Normalization produced identical performance metrics:  
- R-squared: 0.906 
- MSE: 2.90  

*Normalization doesn't affect linear regression performance but aids interpretation when features have different scales.*

### 7. Impact of Using Only Radio & Newspaper
**Results:**  
- R-squared: 0.1097  
- MSE: 27.51  

*Dramatic performance drop confirms TV's critical role in sales prediction.*

## Key Insights
1. TV advertising drives the most sales
2. Newspaper ads show negligible impact (negative coefficient)
3. The full model explains 90% of sales variation
4. Removing TV from predictors makes the model ineffective

## How to Run
1. Clone the repository
2. Install requirements: `pip install -r requirements.txt`
3. Run the notebook: `jupyter notebook sales_prediction.ipynb`

## Dependencies
- Python 3.7+
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

## Files
- `sales_prediction.ipynb`: Jupyter notebook with full analysis
- `advertising_sales_data.xlsx`: Dataset

# Part 3: Regression-Based Business Insights & Model Interpretation

## Business Problem Summary

A retail chain wants to identify the key factors influencing monthly sales across its stores. The objective is to use regression analysis to understand which business variables are most strongly associated with sales so that leadership can make informed decisions regarding marketing investment, inventory management, staffing, and regional business strategy.

---

## Dataset Description

The dataset contains monthly performance data for **320 store-month observations**. It includes store information, marketing activity, customer behaviour, operational metrics, and financial performance.

Key variables include:

* Store ID
* Month
* Region
* Store Type
* Marketing Spend
* Footfall
* Average Discount Percentage
* Staff Count
* Inventory Availability Percentage
* Competitor Distance
* Holiday Flag
* Customer Rating
* Monthly Sales
* Monthly Profit

---

## Dependent and Independent Variables

### Dependent Variable

* **monthly_sales**

### Independent Variables

* marketing_spend
* footfall
* inventory_availability_pct
* avg_discount_pct
* customer_rating
* Region dummy variables (North, South, West)

---

## Regression Approach

The analysis was completed in the following stages:

1. Data cleaning and preparation
2. Creation of dummy variables for categorical data
3. Simple Linear Regression using:

   * Marketing Spend
   * Footfall
4. Multiple Linear Regression using:

   * Marketing Spend
   * Footfall
   * Inventory Availability
   * Region Dummy Variables
5. Model comparison using R-squared and statistical significance
6. Residual analysis for prediction accuracy

---

## Dummy Variable Approach

The categorical variable **Region** was converted into dummy variables.

Created dummy variables:

* Region_North
* Region_South
* Region_West

**East** was selected as the reference category to avoid the dummy variable trap.

---

## Model Comparison Summary

| Model                               | R²     | Summary                                              |
| ----------------------------------- | ------ | ---------------------------------------------------- |
| Simple Regression (Marketing Spend) | 0.1672 | Moderate relationship with sales                     |
| Simple Regression (Footfall)        | 0.7363 | Strong relationship with sales                       |
| Multiple Regression                 | 0.8114 | Best performing model with highest explanatory power |

The multiple regression model explains approximately **81.14%** of the variation in monthly sales and outperformed both simple regression models.

---

## Final Model Selected

The **Multiple Regression Model** was selected because it provides the highest R-squared value, includes multiple important business drivers, and offers stronger predictive performance than the individual simple regression models.

---

## Business Recommendation

The analysis suggests that leadership should prioritize:

* Increasing customer footfall
* Optimizing marketing spend
* Maintaining high inventory availability

Regional differences should be interpreted carefully, as not all regional coefficients were statistically significant.

The multiple regression model should be used to support strategic planning and resource allocation.

---

## Assumptions and Limitations

### Assumptions

* Linear relationship exists between predictors and monthly sales.
* Residual errors are independent.
* Predictor variables are measured accurately.
* Historical data represents current business conditions.

### Limitations

* Regression identifies association rather than causation.
* External business factors such as economic conditions, competitor promotions, and seasonality were not included.
* Predictions may differ under future market conditions.

---

## Screenshots Included

* simple_regression_output.png
* multiple_regression_output.png
* residuals_preview.png
* model_comparison_preview.png

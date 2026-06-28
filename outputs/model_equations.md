# Dummy Variable Approach

The categorical variable **region** was converted into dummy variables before performing multiple regression analysis.

The following dummy variables were created:

* Region_North
* Region_South
* Region_West

The **East** region was selected as the **reference category** and therefore was not converted into a dummy variable.

When all dummy variables have a value of 0, the observation belongs to the East region.

This approach avoids the Dummy Variable Trap by preventing perfect multicollinearity in the regression model.

The dummy variables will be included in the multiple regression model to estimate the effect of different regions on monthly sales compared with the reference category.



# Model Equations

## Simple Regression Model 1 – Marketing Spend

### Regression Equation

Monthly Sales = 560777.30 + (2.129575 × Marketing Spend)

### Coefficient Explanation

- **Intercept (560777.30):** Estimated monthly sales when marketing spend is zero.
- **Marketing Spend Coefficient (2.129575):** For every one-unit increase in marketing spend, monthly sales are expected to increase by approximately **2.13 units**, assuming all other factors remain constant.

### Business Interpretation

Marketing spend has a positive relationship with monthly sales. Increasing marketing investment is associated with higher sales, although this simple model explains only a limited portion of the variation in sales.

---

# Simple Regression Model 2 – Footfall

### Regression Equation

Monthly Sales = 446410.60 + (35.67803 × Footfall)

### Coefficient Explanation

- **Intercept (446410.60):** Estimated monthly sales when footfall is zero.
- **Footfall Coefficient (35.67803):** Every additional customer visiting the store is associated with an increase of approximately **35.68 units** in monthly sales.

### Business Interpretation

Footfall is a strong predictor of monthly sales. Stores with higher customer traffic generally achieve higher sales performance.

---

# Multiple Regression Model

### Regression Equation

Monthly Sales =
131460.30
+ (1.185914 × Marketing Spend)
+ (33.87042 × Footfall)
+ (2818.207 × Inventory Availability %)
+ (10547.38 × Region_North)
+ (21940.49 × Region_South)
+ (17491.37 × Region_West)

### Coefficient Explanation

- **Intercept (131460.30):** Estimated monthly sales when all predictors are zero and the store belongs to the reference region.
- **Marketing Spend (1.185914):** Higher marketing investment is associated with increased monthly sales.
- **Footfall (33.87042):** Additional customer visits contribute positively to monthly sales.
- **Inventory Availability (2818.207):** Better inventory availability is associated with higher monthly sales by reducing stock-outs.
- **Region_North (10547.38):** Stores in the North region are estimated to generate about 10,547 more monthly sales than the reference region, although this variable was not statistically significant.
- **Region_South (21940.49):** Stores in the South region are estimated to generate approximately 21,940 more monthly sales than the reference region.
- **Region_West (17491.37):** Stores in the West region are estimated to generate approximately 17,491 more monthly sales than the reference region.

---

# Dummy Variable Explanation

The categorical variable **Region** was converted into dummy variables for regression analysis.

Dummy variables created:

- Region_North
- Region_South
- Region_West

The **East** region was selected as the **reference category** and was intentionally excluded from the regression model to avoid the dummy variable trap (perfect multicollinearity).

Each region coefficient represents the expected difference in monthly sales compared with stores located in the East region.

---

# Final Model Selected

The **Multiple Regression Model** was selected as the final model.

## Reason for Selecting the Final Model

The multiple regression model provides the strongest explanation of monthly sales with an **R-squared value of 0.811396**, meaning it explains approximately **81.14%** of the variation in monthly sales.

Unlike the simple regression models, it considers multiple business drivers simultaneously, including marketing spend, customer footfall, inventory availability, and regional differences. This provides a more realistic and useful representation of the factors influencing store sales.

Therefore, the multiple regression model is the most appropriate model for supporting business decisions and forecasting monthly sales.

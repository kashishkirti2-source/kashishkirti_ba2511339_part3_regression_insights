# Model Comparison

## Model 1: Simple Regression – Marketing Spend

**Dependent Variable:** monthly_sales

**Independent Variable:** marketing_spend

**R-Squared:** 0.167245

**Significant Variable**

- Marketing Spend (P-value = 2.48E-14)

### Business Usefulness

Marketing spend has a statistically significant positive relationship with monthly sales. However, the model explains only about 16.7% of the variation in sales, indicating that additional factors influence store performance.

### Limitations

- Considers only one predictor.
- Ignores customer traffic, inventory availability, and regional differences.
- Limited predictive power for business decisions.

---

## Model 2: Simple Regression – Footfall

**Dependent Variable:** monthly_sales

**Independent Variable:** footfall

**R-Squared:** 0.736285

**Significant Variable**

- Footfall (P-value = 4.75E-94)

### Business Usefulness

Footfall is a strong predictor of monthly sales. The model explains approximately 73.6% of the variation in sales, making it substantially better than the marketing-only model.

### Limitations

- Does not account for marketing investment, inventory levels, or regional differences.
- Cannot fully explain sales performance by itself.

---

## Model 3: Multiple Regression

**Dependent Variable:** monthly_sales

**Independent Variables**

- marketing_spend
- footfall
- inventory_availability_pct
- Region_North
- Region_South
- Region_West

**R-Squared:** 0.811396

### Significant Variables

| Variable | P-value | Result |
|----------|---------|--------|
| Marketing Spend | 2.17E-17 | Significant |
| Footfall | 5.40E-101 | Significant |
| Inventory Availability | 9.51E-09 | Significant |
| Region South | 0.003209 | Significant |
| Region West | 0.008029 | Significant |
| Region North | 0.148360 | Not Significant |

### Business Usefulness

The multiple regression model provides the highest explanatory power (81.1%). It captures multiple business drivers simultaneously, making it the most useful model for forecasting monthly sales and supporting business decision-making.

### Limitations

- Regression measures association, not causation.
- Other external factors such as competition, economic conditions, and seasonal trends may also influence sales.
- Region North was not statistically significant and should not be over-interpreted.

---

# Overall Comparison

| Model | R-Squared | Recommendation |
|--------|----------:|----------------|
| Marketing Spend | 0.167245 | Weak explanatory power |
| Footfall | 0.736285 | Strong predictor |
| Multiple Regression | 0.811396 | Selected as the final model |

## Final Model Selected

The Multiple Regression model is selected because it has the highest R-squared value (81.1%), includes multiple significant business variables, and provides the strongest support for business decision-making.

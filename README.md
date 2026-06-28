# Business Problem Summary

The leadership team of a retail chain wants to understand which business factors are most strongly associated with monthly sales performance across stores. The objective is to use regression analysis to identify the key drivers of sales and support business decisions related to marketing, inventory management, staffing, discount strategy, and store operations.

---

# Dataset Description

The dataset contains monthly business information for retail stores, including sales, marketing spend, customer footfall, discounts, inventory availability, staffing, customer ratings, region, and store type. These variables are used to build regression models for explaining variations in monthly sales.

---

# Dependent and Independent Variables

## Dependent Variable

**monthly_sales**

This is the target variable that the regression models aim to predict and explain.

## Potential Independent Variables

* marketing_spend
* footfall
* avg_discount_pct
* staff_count
* inventory_availability_pct
* competitor_distance_km
* holiday_flag
* customer_rating
* region (Dummy Variables)
* store_type (Dummy Variables)

---

# Numerical Variables

* marketing_spend
* footfall
* avg_discount_pct
* staff_count
* inventory_availability_pct
* competitor_distance_km
* customer_rating
* monthly_sales
* monthly_profit

---

# Categorical Variables

* region
* store_type

---

# Variables That May Need Cleaning or Transformation

The following preprocessing steps may be required before regression analysis:

* Check for missing values.
* Verify numerical columns for invalid or extreme values.
* Convert categorical variables (such as region and store_type) into dummy variables.
* Keep one category as the reference category to avoid the dummy variable trap.

---

# Variables That May Not Be Useful for Regression

* store_id (Unique identifier only)
* month (Used mainly for identification or trend analysis and not included in the regression model)

These variables do not directly explain monthly sales and are therefore excluded from the regression models.

# Task 1: Dataset Understanding

## Dependent Variable
- monthly_sales

## Potential Independent Variables
- marketing_spend
- footfall
- avg_discount_pct
- staff_count
- inventory_availability_pct
- competitor_distance_km
- holiday_flag
- customer_rating
- region
- store_type

## Numerical Variables
- marketing_spend
- footfall
- avg_discount_pct
- staff_count
- inventory_availability_pct
- competitor_distance_km
- customer_rating
- monthly_sales
- monthly_profit

## Categorical Variables
- region
- store_type
- store_id

## Variables That May Need Cleaning or Transformation
- month (date variable)
- region (dummy encoding required)
- store_type (dummy encoding required)
- store_id (identifier, not useful directly)

## Variables Not Useful for Regression
- store_id


# Task 2: Dataset Description

This dataset contains retail store performance data collected across different regions, store types, and time periods.

### Objective

The objective of the analysis is to identify factors associated with monthly sales and build regression models to predict sales performance.

### Dependent Variable

- monthly_sales

### Independent Variables

- marketing_spend
- footfall
- avg_discount_pct
- staff_count
- inventory_availability_pct
- competitor_distance_km
- holiday_flag
- customer_rating
- region
- store_type

### Dataset Characteristics

- Contains sales, marketing, operational, and customer-related information.
- Includes both numerical and categorical variables.
- Store type and region require dummy variable encoding before regression analysis.
- Store ID is used as an identifier and is not included as a predictor in regression models.

  
# Task 3: Create Dummy Variables 

## Dummy Variable Approach

The categorical variable `store_type` was converted into dummy variables for regression analysis.

Reference Category:
- Airport

Dummy Variables Created:
- Residential_Dummy
- HighStreet_Dummy

Airport stores were used as the baseline category. Residential and High Street stores were compared against Airport stores using dummy variables.


# Task 4: Regression Approach

Three regression models were developed:

### Simple Regression 1
Dependent Variable: monthly_sales

Independent Variable: marketing_spend

Purpose:
To understand the relationship between marketing investment and sales.

### Simple Regression 2
Dependent Variable: monthly_sales

Independent Variable: footfall

Purpose:
To understand how customer traffic influences sales.

### Multiple Regression
Dependent Variable: monthly_sales

Independent Variables:
- marketing_spend
- footfall

Purpose:
To evaluate the combined impact of multiple business factors on monthly sales and improve prediction accuracy.


# Task 5: Model Comparison Summary

Three models were evaluated:

| Model | Variables Used | Performance |
|---------|---------|---------|
| Simple Regression 1 | marketing_spend | Moderate |
| Simple Regression 2 | footfall | Strong |
| Multiple Regression | marketing_spend + footfall | Best |

The Multiple Regression model achieved the highest explanatory power with R² ≈ 0.782 and was selected as the final model.


# Task 6: Final Model Selected

The Multiple Regression model was selected as the final model.

Reasons:

- Highest R² value (0.7819)
- Both marketing_spend and footfall were statistically significant
- Better prediction accuracy than simple regression models
- Explains approximately 78% of the variation in monthly sales


# Task 7: Business Recommendation

Based on the regression analysis:

- Increase marketing investment in high-performing campaigns.
- Focus on increasing customer footfall through promotions and customer engagement.
- Monitor both marketing spend and footfall regularly.
- Use the regression model to support sales forecasting and planning.

The analysis indicates that marketing spend and footfall are the strongest drivers of monthly sales.


# Task 8: Assumptions and Limitations

Assumptions:

- Linear relationship exists between predictors and sales.
- Historical data represents future behavior.
- Variables are measured accurately.

Limitations:

- Regression shows association, not causation.
- External factors such as market conditions and competition may influence sales.
- The model explains approximately 78% of sales variation, leaving some variation unexplained.


# Task 9: Screenshots Included

The repository contains screenshots supporting:

- Simple Regression Output
- Multiple Regression Output
- Model Comparison
- Residual Analysis

Screenshots are available in the screenshots folder.

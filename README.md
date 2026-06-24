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


# Task 3: Create Dummy Variables 

## Dummy Variable Approach

The categorical variable `store_type` was converted into dummy variables for regression analysis.

Reference Category:
- Airport

Dummy Variables Created:
- Residential_Dummy
- HighStreet_Dummy

Airport stores were used as the baseline category. Residential and High Street stores were compared against Airport stores using dummy variables.

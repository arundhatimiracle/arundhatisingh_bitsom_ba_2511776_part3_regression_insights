# Dummy Variable Approach

## Categorical Variable Used

store_type

## Reference Category

Airport

## Dummy Variables Created

* Residential_Dummy
* HighStreet_Dummy

## Explanation

To use the categorical variable `store_type` in regression analysis, dummy variables were created.

* Residential_Dummy = 1 if the store type is Residential, otherwise 0.
* HighStreet_Dummy = 1 if the store type is High Street, otherwise 0.
* Airport stores are used as the reference category and therefore do not require a separate dummy variable.

This approach avoids the dummy variable trap and allows comparison of Residential and High Street stores against Airport stores in the regression model.

## 1. Dummy Variable Approach

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

---

## 2. Simple Regression Model 1 (Marketing Spend)

Monthly Sales = 396109.26 + 1.1438 × Marketing Spend

### Interpretation
- Intercept (396109.26): Expected monthly sales when marketing spend is zero.
- Marketing Spend Coefficient (1.1438): For every additional 1 unit spent on marketing, monthly sales increase by approximately 1.14 units.

---

## 3. Simple Regression Model 2 (Footfall)

Monthly Sales = 396109.26 + 33.53 × Footfall

### Interpretation
- Intercept (396109.26): Expected monthly sales when footfall is zero.
- Footfall Coefficient (33.53): Every additional customer visit increases monthly sales by approximately 33.53 units.

---

## 4. Multiple Regression Model

Monthly Sales = 396109.26 + 1.1438 × Marketing Spend + 33.5344 × Footfall

### Interpretation of Coefficients

#### Intercept (396109.26)
Represents the baseline monthly sales when all predictors are zero.

#### Marketing Spend (1.1438)
Keeping footfall constant, every additional unit spent on marketing increases monthly sales by approximately 1.14 units.

#### Footfall (33.5344)
Keeping marketing spend constant, every additional customer visit increases monthly sales by approximately 33.53 units.

---

## 5. Reference Category Used

The reference category is the category omitted during dummy variable creation.

All dummy variable coefficients are interpreted relative to this reference category.

---

## 6. Final Model Selected

Multiple Regression Model

Monthly Sales = 396109.26 + 1.1438 × Marketing Spend + 33.5344 × Footfall

---

## 7. Reason for Selecting the Final Model

The multiple regression model was selected because it provides a higher explanatory power (R² = 0.7819) while considering more than one business factor.

Both Marketing Spend and Footfall are statistically significant predictors with very small p-values.

This model is more useful for business decision-making because sales are influenced by multiple factors rather than a single variable. By considering both marketing activity and customer traffic, the model provides more reliable sales predictions.

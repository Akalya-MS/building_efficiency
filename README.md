# Building Energy Efficiency Prediction
The goal of this project is to predict the Heating Load (HL) and Cooling Load (CL) of buildings based on their design parameters. These predictions can help architects and engineers design energy-efficient buildings that minimize operational costs and environmental impact.

**Dataset**
* Samples: 768
* Features: 8 building design parameters, including:
  1. Relative Compactness
  2. Surface Area
  3. Wall Area
  4. Roof Area
  5. Overall Height
  6. Orientation
  7. Glazing Area
  8. Glazing Area Distribution
* Targets:
  * Heating Load (HL)
  * Cooling Load (CL)

## Preprocessing Steps
* Checked for null values 
* Computed mean, median, mode, and standard deviation (SD) for each feature to understand data distribution.
* Standardized numerical features for consistent scale.
* Split the dataset into 80% training and 20% testing sets.

## Algorithm Used — LGBMRegressor
  * Fast and efficient gradient boosting model.
  * Handles small-to-medium datasets with excellent performance.
  * Captures complex nonlinear relationships without heavy preprocessing.
  * Requires fewer resources compared to deep learning models.
  * Trained two separate models: one for HL and one for CL.

## Model Evaluation
* Metrics used: R² Score, Mean Absolute Error (MAE), Mean Squared Error (MSE).
* Achieved high R² values (> 0.95) for both HL and CL on test data, showing excellent predictive power.

## Accuracy and Results

| Target       | R² Score | MAE  | MSE  |
| ------------ | -------- | ---- | ---- |
| Heating Load | 1.00     | 0.38 | 0.33 |
| Cooling Load | 0.98     | 0.92 | 1.80 |







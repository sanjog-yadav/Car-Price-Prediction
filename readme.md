# Car price Prediction

**Problem Statement:**
Predict the price of a car based on various parameters like car make, car model, car year engine cylinder, driven wheels, market category etc. The company wants to know —
	- which variables are significant in predicting the price of a car
	- how well those variables describe the price of a car

**Steps taken:**
1. Reading and Understanding the data
2. Visualising the data
	- Visualising numeric values using `pairplot`
	- Visualising data using heatmap
3. Data Preparation
	- Create dummy variables
	- Drop unneccessary columns
	- Fix missing values
4. Splitting the data into training and testing dataset
	- Rescaling the features using `MinMaxScalar`
5. Building a linear model
	- Check for p-values and remove unneccessary columns
	- Check VIFs
6. Residual Analysis of the train data
	- Plot `Error terms` using `distplot`
7. Making predictions using the final model
8. Model Evaluation
	- Plot `y_test` vs `y_pred` using `scatter` plot
9. Compare with benchmark model
	- In this case, using **SLR: Simple Linear Regression**
10. Conclusion
	- R-squared value for
		- Multiple Linear Regression: `0.814`
		- Linear Regression: `0.429`
	- Overall we have a decent model, but we also acknowledge that we could do better.
	- We have below option to get more accurate:
		- Build a non-linear model
Its good to do correlation to understand multiocollinearity. 
This is usually done during the preprocessing phase.

Use the built in formual df.corr(indepentvariables) to calculate the multicollinearity.
Later on use seaborn heatmap to plot the same.

While ding preprocessing its better to check if all independent variables are in same magnitude.
If not in same magnitude,one indepenet variable with higher magniture will dominate the reg model.

Two ways to do the feature scaling.

a.Standard scalar.
 Convert the values to Z scores by using standard techniques -> (x-mean)/(std.deviation)
 bewre of the speelling ->StandardScaler and not StandardScalar

b.Why do we perform fit_transform on train data set and transfrom on x_test set ->
Bcause we want to centre the test data set on same mean/standard deviation on train data set.After all this is subset of
original data set.

c.Always keep random_state with same value to replicate the results.

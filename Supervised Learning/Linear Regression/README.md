### Linear Regression
Simple linear regression is a statistical method that allows us to summarize and study relationships between two continuous (quantitative) variables:
- One variable, denoted x, is regarded as the predictor, explanatory, or independent variable.
- The other variable, denoted y, is regarded as the response, outcome, or dependent variable.
Simple linear regression gets its adjective "simple," because it concerns the study of only one predictor variable.  

common notation:
- yi denotes the observed response for experimental unit i  
- xi denotes the predictor value for experimental unit i
- <img src="https://render.githubusercontent.com/render/math?math=\hat{y}_i"> is the predicted response (or fitted value) for experimental unit i  

Then, the equation for the best fitting line is:
<img src="https://render.githubusercontent.com/render/math?math=\hat{y}_i=b_0 %2B b_1x_i">  

In general, when we use <img src="https://render.githubusercontent.com/render/math?math=\hat{y}_i=b_0 %2B b_1x_i"> to predict the actual response <img src="https://render.githubusercontent.com/render/math?math=\hat{y}_i"> we make a prediction error (or residual error) of size: <img src="https://render.githubusercontent.com/render/math?math=e_i=y_i-\hat{y}_i">

A line that fits the data "best" will be one for which the n prediction errors — one for each observed data point — are as small as possible in some overall sense. One way to achieve this goal is to invoke the "least squares criterion," which says to "minimize the sum of the squared prediction errors." That is:  
- The equation of the best fitting line is: <img src="https://render.githubusercontent.com/render/math?math=\hat{y}_i=b_0 %2B b_1x_i">  
- We just need to find the values b0 and b1 that make the sum of the squared prediction errors the smallest it can be.
- That is, we need to find the values b0 and b1 that minimize: <img src="https://render.githubusercontent.com/render/math?math=Q=\sum_{i=1}^{n}(y_i-\hat{y}_i)^2">  

The formulas are determined using methods of calculus. We minimize the equation for the sum of the squared prediction errors: <img src="https://render.githubusercontent.com/render/math?math=Q=\sum_{i=1}^{n}(y_i-(b_0%2Bb_1x_i))^2">    
Take the derivative with respect to b0 and b1, set to 0, and solve for b0 and b1 and get the "least squares estimates" for b0 and b1: <img src="https://render.githubusercontent.com/render/math?math=b_0=\bar{y}-b_1\bar{x}"> and <img src="https://render.githubusercontent.com/render/math?math=b_1=\frac{\sum_{i=1}^{n}(x_i-\bar{x})(y_i-\bar{y})}{\sum_{i=1}^{n}(x_i-\bar{x})^2}">

Assumption:
- Linear: the mean of the response variable is a linear combination of the parameters (regression coefficients) and the predictor variable
- Independence of errors
- Constant variance (homoscedasticity). This means that the variance of the errors does not depend on the values of the predictor variables
- Errors are normally distributed

The OLS method minimizes the sum of squared residuals, and leads to a closed-form expression for the estimated value of the unknown parameter vector β: <img src="https://render.githubusercontent.com/render/math?math={\displaystyle {\hat {\boldsymbol {\beta }}}=(\mathbf {X} ^{\mathsf {T}}\mathbf {X} )^{-1}\mathbf {X} ^{\mathsf {T}}\mathbf {y} ,}">

<img src="https://miro.medium.com/max/1376/1*G1Y_-X14q2xMVHlUuaUUdA.png" width="700"/>


### Gradient Descent

**[Gradient descent](https://en.wikipedia.org/wiki/Gradient_descent)** is an iterative approach to determining a local minimum of a differentiable function. Steps should be repeatedly taken in the opposite direction of the gradient (or approximate gradient) of the function at the current point, since this is the direction of steepest descent. Everytime when the prediction is not correct, the gradient descent will help to correct the weight vector to the right direction for the next iteration.

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/ff/Gradient_descent.svg/350px-Gradient_descent.svg.png" width="400"/>

1. We first build a linear model: 
$\hat{y} = X\times \hat{w}_{i}$ + b  
We sample the weight: w_hat and bias: b from a uniform distribution.  

2. We write a loss function. We use Mean Square Error here. $\displaystyle\frac{1}{2}\sum_{i=1}^{n}(x_{i}\hat{w}_{i} +b_{i} - y_{i})^2$  

3. Calculate the gradient of the loss function $\displaystyle\frac{\partial L}{\partial w}$ and $\displaystyle\frac{\partial L}{\partial b}$  
<center>$\displaystyle\frac{\partial L}{\partial w} = \sum_{i=1}^{n}(x_{i}\hat{w}_{i} +b_{i} - y_{i})x_{i} $</center>  
<center>$\displaystyle\frac{\partial L}{\partial b} = \sum_{i=1}^{n}(x_{i}\hat{w}_{i} +b_{i} - y_{i})$</center>  

4. Set up a learning rate alpha  and update w_hat and b.  
Updated $\hat{w}$ = previous $\hat{w}$ - alpha $\displaystyle\times\frac{\partial L}{\partial w}$  
Updated b = previous b - alpha $\displaystyle\times\frac{\partial L}{\partial b}$  

We do not want a too large alpha (large steps) because it might overshoot the minimum, but also do not want a too small alpha (small steps) because it might take a long time to train. Thus, we may need to try a couple times to find the right learning rate.


5. Repeat this process for different times (iteration): 10, 100, 1000, and 10000 times and calculate their losses and compare.


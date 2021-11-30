### Perceptron

#### A perceptron has four parts: Inputs, weights and bias, net sum, and activation function.  
1. All inputs <img src="https://render.githubusercontent.com/render/math?math=X_{i}"> and a constant 1 for bias are multiplied by their weights <img src="https://render.githubusercontent.com/render/math?math=W_{i}">  
2. Sum all the multiplied values
3. Plug the weighted sum to the activation function, and it will generate an output. If the output is greater than a certain threshold, then it will classify the point to a certain class, and if not then it will be classified to the other class.

The perceptron drawn as a neuron

<img src="https://miro.medium.com/max/700/1*n6sJ4yZQzwKL9wnF5wnVNg.png" width="500"/>  

The input data will be paired with the corresponding weights and sum together, and the put into an activation function to create the output.
<img src="https://render.githubusercontent.com/render/math?math=\hat y^i = \text{sign}(w^T\bar x^i)">  

 

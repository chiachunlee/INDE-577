### Multilayer Perceptron
Multilayer perceptron (MLP) is a class of feed forward neural network and sometimes refer to networks composed of multiple layers of perceptrons. 

There are at least three layers of nodes in MLP: an input layer, a hidden layer and an output layer. The MLP consists of three or more layers (an input and an output layer with one or more hidden layers) of nonlinearly-activating nodes. Since MLPs are fully connected, each node in one layer connects with a certain weight $w_{ij}$ to every node in the following layer.
For the layers after input layer, every node is a neuron that uses a nonlinear activation function. MLP model use backpropagation for training, and it is a supervised learning technique.

#### Activation function
If a multilayer perceptron has a linear activation function in all neurons, that is, a linear function that maps the weighted inputs to the output of each neuron, then linear algebra shows that any number of layers can be reduced to a two-layer input-output model. In MLPs some neurons use a nonlinear activation function that was developed to model the frequency of action potentials, or firing, of biological neurons.

The two historically common activation functions are both sigmoids, and are described by <img src="https://wikimedia.org/api/rest_v1/media/math/render/svg/167e8b5c38130ec92a2771bc384658772f387d02" width="300"/> In recent developments of deep learning the rectifier linear unit (ReLU) is more frequently used as one of the possible ways to overcome the numerical problems related to the sigmoids. Here <img src="https://render.githubusercontent.com/render/math?math=y_{i}"> is the output of the ith node (neuron) and <img src="https://render.githubusercontent.com/render/math?math=v_{i}"> is the weighted sum of the input connections. 

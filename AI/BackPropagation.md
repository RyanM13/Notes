> [!NOTE]
> source: https://mattmazur.com/2015/03/17/a-step-by-step-backpropagation-example/comment-page-15/

# SuperVised Learning

- Answers are known
- They are referred to as expected output
- You want to train a model & this model needs to become better at that.
- The model will compute something which we will refer to as prediction
- Difference between expected & prediction will give me a method that will will help me to estimate
- if the model has learned to a satisfactory level, or, if it is necessary to continue training.

## Neural Network

- HyperParameters
- Subject to tunning
  > [!NOTE]
  > W -> Weights
  > B -> Biases

image: https://mattmazur.com/wp-content/uploads/2018/03/neural_network-7.png

Three layers
Fully connected

layer 0 input layer
layer 1 hidden layers
output layer

Fully Connected Neuarl Network
layer1/outputLayer

- Neuron
- Activation unit
- Node
- 2 phase computational unit

2 computational phase because

- 2 phases
- phase 1 and phase 2
- Feed something to -> phase 1, some math
- feed outcome(p1) to -> phase 2, output from phase 2.

Initially forward Propagation than when the model needs to learn more we do backpropagation.

> [!IMPORTANT]
> The goal of backpropagation is to optimize the weights so that the neural network can learn how to correctly map arbitrary inputs to outputs.

If the values do not change [Weights, Biases] than the Neuarl network does not change.

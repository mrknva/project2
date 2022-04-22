# project2
You will be provided a network as follows: Network = [layer1, layer2, .., layerL],
where each layer is either of the following:
• [’linear_I’, Weights]: A linear layer with weights Weights, which is a list. I is an integer representing the order of this layer among all linear layers. If this layer is a mapping from Mj to Mj+1, Weights has Mj+1 elements where each element has Mj numbers for aj.
 0, 1+e−x
if − 700 ≤ x
if − 700 < x < 700 (6) if 700 ≤ x
  1,
The Sigmoid layer between aj ∈ RMj and aj+1 ∈ RMj+1 is then defined as follows:
• ’relu_I’: The non-linear layer in Eqn. 4. I is an integer representing the order of this layer among all ReLU layers.
• ’sigmoid_I’: The non-linear layer in Eqn. 7. I is an integer representing the order of this layer among all Sigmoid layers.
Your task is to write a function called forward_pass(Network, X), where Network is as de- fined above and X is a 784-dimensional list representing an image. The output of the forward_pass function is the output of the last layer in the Network. We will arrange the Network such that its last layer will have C = 10 many numbers (i.e. prediction scores) if there are C = 10 classes. forward_pass() should not select the class with the highest score; that will be the job of other functions.

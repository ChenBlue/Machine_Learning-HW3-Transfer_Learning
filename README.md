# Machine_Learning-HW3-Transfer_Learning
This is the homework from CS5651 Machine Learning in National Tsing Hua University.

## Instruction
In previous HW, we trained a model for 0\~4 digits in MNIST handwritten digits dataset. The previous network structure is 5 hidden layer with 128 neurons and 1 softmax layer with 5 neurons. We will reuse pretrain model from HW2 to train **5\~9** digits. In data set, I will only keep **100** instances per digit for training set, **30** instances per digit for validation set, and whole testing set. There are 4 parts in this homework. </br>
### Part 1
Freeze 5 hidden layers and only train softmax layer.

### Part 2
Freeze 5 hidden layers and feed the training sets and validation sets into these 5 hidden layers. Next, cache the output of 5th layer, and feed these output as input when training the softmax layer.

### Part 3
Freeze first 4 hidden layers and abort 5th hidden layer. Add a new softmax layer at the end and start training this layer.

### Part 4
Freeze 3rd and 4th layers and abort 5th layer. Add a new softmax layer at the end and start training 1st, 2nd and softmax layer.



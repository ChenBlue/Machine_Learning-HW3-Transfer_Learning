# Machine_Learning-HW3-Transfer_Learning
This is the homework from CS5651 Machine Learning in National Tsing Hua University.

## Instruction
In previous HW, we trained a model for 0\~4 digits in MNIST handwritten digits dataset. The previous network structure is 5 hidden layer with 128 neurons and 1 softmax layer with 5 neurons. We will reuse pretrain model from HW2 to train **5\~9** digits. In data set, I will only keep **100** instances per digit for training set, **30** instances per digit for validation set, and whole testing set. Besides, I set an early stop critirion. When the best loss doesn't decrease for 20 epochs.There are 4 parts in this homework. </br>
### Part 1
Freeze 5 hidden layers and only train softmax layer.
![structure1](https://github.com/ChenBlue/Machine_Learning-HW3-Transfer_Learning/blob/master/FIG/part1_structure.PNG) </br>

### Part 2
Freeze 5 hidden layers and feed the training sets and validation sets into these 5 hidden layers. Next, cache the output of 5th layer, and feed these output as input when training the softmax layer.
![structure2](https://github.com/ChenBlue/Machine_Learning-HW3-Transfer_Learning/blob/master/FIG/part2_structure.PNG) </br>

### Part 3
Freeze first 4 hidden layers and abort 5th hidden layer. Add a new softmax layer at the end and start training this layer.
![structure3](https://github.com/ChenBlue/Machine_Learning-HW3-Transfer_Learning/blob/master/FIG/part3_structure.PNG) </br>

### Part 4
Freeze 3rd and 4th layers and abort 5th layer. Add a new softmax layer at the end and start training 1st, 2nd and softmax layer.
![structure4](https://github.com/ChenBlue/Machine_Learning-HW3-Transfer_Learning/blob/master/FIG/part4_structure.PNG) </br>

## Result
### Part 1
Accuracy rate: 82.843 % </br>
Training time: 18.89 sec

### Part 2
Accuracy rate: 82.843 % </br>
Training time: 17.69 sec </br>
Training time is shorter than Part 1 because it saves the output of 5th layer.

### Part 3
Training time: 18.65 sec

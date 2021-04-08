# CMPE258 Assignment 3

- **CMPE258_HW3_PartA** contains code for building a 3 layer neural network using pure numpy datastructures. <br/>
The flow includes the following:  
    1. Weight initialization - shape 2 * 3 tensor
    2. Appropriate bias tensor initialization - 2 * 1
    3. Calculated the actual value of output given by equations: 
        - y1 = x_1^2 + 2 * x_2^2 + 3 * x_3^2 + x_1 + 2 * x_2 + 3 * x_3 + 1
        - y2 = 4 * x_1^2 + 5 * x_2^2 + 6 * x_3^2 + 4 * x_1 + 5 * x_2 + 6 * x_3 + 0.5
    4. Forward pass to compute the random initial y_pred values.
    5. Compute the loss value - difference between actual and expected output (MSE)
    6. Using backward pass we update the weight values by making use of the loss.

- **CMPE258_HW3_PartB_1** contains code for the same but in low level Pytorch and with no auto differentiation and custom linear layer function.

- **CMPE258_HW3_PartB_2** contains code for the same but in mid level Pytorch and with auto differentiation.

- **CMPE258_HW3_PartB_3** contains code for the same but in high level Pytorch and in-built linear module.

- **CMPE258_HW3_PartC_1** contains code for the same but in low level TensorFlow and with no auto differentiation and custom linear layer function.

- **CMPE258_HW3_PartC_2** contains code for the same but in mid level TensorFlow and with auto differentiation.

- **CMPE258_HW3_PartC_3** contains code for the same but in high level TensorFlow and in-built linear module.

*Please Note: In depth details are provided in the respective notebooks.*

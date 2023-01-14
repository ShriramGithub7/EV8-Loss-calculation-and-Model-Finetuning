# EV8-Loss-calculation-and-Model-Finetuning

This repository has 2 parts:

**Part 1:** This section shows illustration of how loss is calculated and weights are updated in back-propogation. Excel is used that has mathematical formulas that will show how loss value is calculated after each batch. 

**Part 2:** This section has MNIST model that is finetuned to achive 99.40% accuracy, within 20 epochs and with 18820 parameters. GAP, FC, Batch normalization is used in the model. 

**Part 1: LOSS Calculation and Back Propogation**:

Below screenshot shows the basic network structure with 1 input, 1 hidden and 1 output layer. It also shows how individual parameter values and derivative values are calculated. These values are then used to calculate gradient of the network.

Please note that excel sheet is also attached in the repository, so it can be used to cross check below details. Also, we can play with different input, output values, initial weights and different learning rates to see how loss is updated and graph is projected.

![image](https://user-images.githubusercontent.com/93775361/212448379-7a9e2891-21d9-428a-be8e-9d184515b8b7.png)


After parameter and derivatives formulas are calculated, use these formulas and calculate the actual values of loss and gradients for first batch. For the susequent batch/epochs, use the gradients from previous layer and update the weights and calculate the loss. 

![image](https://user-images.githubusercontent.com/93775361/212448303-c557fe8f-6d1d-4a96-8ac8-01f7ff3ecdbd.png)


Red highlighted column shows calculated loss after each epoch.

![image](https://user-images.githubusercontent.com/93775361/212448324-44e528d0-3613-428b-94c2-60afa9b07815.png)


Plot the graph between epochs and loss. It can be seen how loss gets reduced with increase in number of epochs

![image](https://user-images.githubusercontent.com/93775361/212448206-e5fb58b1-a459-4e1c-a3d5-b3479ff19e64.png)



Now change the learning rates see below the effect of the same on Loss graph:

**Learning Rate: 0.1**
Note: Above graph, there are couple of records of excel sheet. That shows updated loss value after last epoch

![image](https://user-images.githubusercontent.com/93775361/212443604-4fb38af6-7db0-4247-8c0f-918f8445a5ee.png)


**Learning Rate: 0.2**

![image](https://user-images.githubusercontent.com/93775361/212443648-a231a6ef-f179-49de-a63f-1c4505d0fa60.png)


**Learning Rate: 0.5**

![image](https://user-images.githubusercontent.com/93775361/212443732-63af1b41-1233-48b3-8e26-b33e90db79df.png)


**Learning Rate: 0.8**

![image](https://user-images.githubusercontent.com/93775361/212443761-2397e226-6773-4676-bbf2-a9e0de679feb.png)


**Learning Rate: 1.0**

![image](https://user-images.githubusercontent.com/93775361/212443797-13057ac8-71cb-4adf-81fd-96031e329955.png)


**Learning Rate: 2.0**

![image](https://user-images.githubusercontent.com/93775361/212443819-675fc9a4-00fc-4c0f-b0de-59c96cf5b105.png)



**Part 2: MNIST dataset model finetuning**:

Model is finetuned to achieve 99.40% accuracy. 
Existing code is changed thereby adding Batch normalization, Dropout, GAP, and Fully connected layer.

**Below is final statistics:**

total number of parameters: **18820**

final validation/test accuracy: **99.40%**

other additional things you might have used in your code: **Added BN, Dropout, GAP, FC layer and changed values of number of kernals in each layer.**

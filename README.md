# EV8-Loss-calculation-and-Model-Finetuning

This repository has 2 parts:

**Part 1:** This section shows illustration of how loss is calculated and weights are updated in back-propogation. Excel is used that has mathematical formulas that will show how loss value is calculated after each batch. 

**Part 2:** This section has MNIST model that is finetuned to achive 99.40% accuracy, within 20 epochs and with 18820 parameters. GAP, FC, Batch normalization is used in the model. 

**Part 1: LOSS Calculation and Back Propogation**:

![image](https://user-images.githubusercontent.com/93775361/212448277-0bd2fdeb-2c11-4a6c-af61-e8108ab656f2.png)

![image](https://user-images.githubusercontent.com/93775361/212448303-c557fe8f-6d1d-4a96-8ac8-01f7ff3ecdbd.png)

![image](https://user-images.githubusercontent.com/93775361/212448324-44e528d0-3613-428b-94c2-60afa9b07815.png)


![image](https://user-images.githubusercontent.com/93775361/212448206-e5fb58b1-a459-4e1c-a3d5-b3479ff19e64.png)



Now change the learning rates see below the effect of the same on Loss graph:

Learning Rate: 0.1

![image](https://user-images.githubusercontent.com/93775361/212443604-4fb38af6-7db0-4247-8c0f-918f8445a5ee.png)

Learning Rate: 0.2

![image](https://user-images.githubusercontent.com/93775361/212443648-a231a6ef-f179-49de-a63f-1c4505d0fa60.png)

Learning Rate: 0.5

![image](https://user-images.githubusercontent.com/93775361/212443732-63af1b41-1233-48b3-8e26-b33e90db79df.png)


Learning Rate: 0.8

![image](https://user-images.githubusercontent.com/93775361/212443761-2397e226-6773-4676-bbf2-a9e0de679feb.png)


Learning Rate: 1.0

![image](https://user-images.githubusercontent.com/93775361/212443797-13057ac8-71cb-4adf-81fd-96031e329955.png)


Learning Rate: 2.0

![image](https://user-images.githubusercontent.com/93775361/212443819-675fc9a4-00fc-4c0f-b0de-59c96cf5b105.png)

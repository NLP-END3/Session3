# Session3

## Problem Statement

Write a neural network that can:
1. take 2 inputs:  
    1. an image from the MNIST dataset (say 5), and  
    2. a random number between 0 and 9, (say 7)
2. and gives two outputs:  
    1. the "number" that was represented by the MNIST image (predict 5), and  
    2. the "sum" of this number with the random number and the input image to the network (predict 5 + 7 = 12)
3. you can mix fully connected layers and convolution layers  
4. you can use one-hot encoding to represent the random number input as well as the "summed" output.  
    a. Random number (7) can be represented as 0 0 0 0 0 0 0 1 0 0  
    b. Sum (13) can be represented as: 
        1. 0 0 0 0 0 0 0 0 0 0 0 0 0 1 0 0 0 0 0  
        2. 0b1101 (remember that 4 digits in binary can at max represent 15, so we may need to go for 5 digits. i.e. 10010


![image](https://user-images.githubusercontent.com/30425824/136686498-1fb5e23f-1483-4ca9-9e7d-fc99c9536494.png)

**Your code MUST be:**
1. well documented (via readme file on github and comments in the code)  
2. must mention the data representation
![image](https://user-images.githubusercontent.com/30425824/137435089-b231d73c-ee7e-406e-82d1-de975b62caa6.png)
![image](https://user-images.githubusercontent.com/30425824/137435132-41627581-b165-4165-a108-a951ff964244.png)

3. must mention your data generation strategy (basically the class/method you are using for random number generation)  
![image](https://user-images.githubusercontent.com/30425824/137435360-86008d4d-d000-48e6-b2bd-bb09a61ec4f5.png)

5. must mention how you have combined the two inputs (basically which layer you are combining)  

Two methods were tried in this study with the same hyperparameters (```Optimizer = Adam, Epochs = 20, Leraning_rate = 0.001, batch_size = 1000 ```)

a. ``` Method1: Neural Network with **Convolutional Layers & Fully Connected Layers**```  
![image](https://user-images.githubusercontent.com/30425824/137436572-8f274f50-0b73-4dcf-87b4-42d1bd56494d.png)  

b. ``` Method2: Neural Network with **Only Fully Connected Layers**```  

![image](https://user-images.githubusercontent.com/30425824/137449271-de53444e-df92-4e8c-b580-3ff8f61c7592.png)

7. must mention how you are evaluating your results   
8. must mention "what" results you finally got and how did you evaluate your results  
9. must mention what loss function you picked and why!  
10. **training MUST happen on the GPU** **--> NOT INCORPORATED IN THE CODE**  
11. Accuracy is not really important for the SUM  

![image](https://user-images.githubusercontent.com/30425824/137450278-e11adae4-c25b-42ce-95b3-5ce2fdce3786.png)

## Reference
1. https://github.com/pytorch/examples/blob/master/mnist/main.py
2. https://pytorch.org/tutorials/intermediate/tensorboard_tutorial.html

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
3. must mention your data generation strategy (basically the class/method you are using for random number generation)  
4. must mention how you have combined the two inputs (basically which layer you are combining)  
5. must mention how you are evaluating your results   
6. must mention "what" results you finally got and how did you evaluate your results  
7. must mention what loss function you picked and why!  
8. **training MUST happen on the GPU** **--> NOT INCORPORATED IN THE CODE**  
9. Accuracy is not really important for the SUM  


![image](https://user-images.githubusercontent.com/30425824/136686451-088e9e4b-615a-4cdd-b7fc-988cbff896ef.png)

## Reference
1. https://github.com/pytorch/examples/blob/master/mnist/main.py
2. https://pytorch.org/tutorials/intermediate/tensorboard_tutorial.html

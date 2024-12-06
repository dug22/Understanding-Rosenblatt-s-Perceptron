## Understanding The Perceptron Model
<p align="justify">
This repository provides an in-depth exploration of the fundamental steps involved in Rosenblatt's Perceptron Model. The accompanying Python notebook meticulously breaks down the concept of the Perceptron, offering a comprehensive explanation of how it functions. The notebook delves into the underlying theory of the model, walking through each step of the process, from input data handling to the calculation of weighted sums and the application of the step function. By offering detailed insights into the mechanics of the Perceptron, the notebook ensures a clear and fundamental understanding of its role in binary classification tasks, as well as the iterative process that enables it to learn and make decisions based on input data.
</p>

## Introduction
<p align="justify">
The perceptron serves as a fundamental unit of logic in artificial neural networks. The perceptron is modified to handle binary classification tasks, distinguishing between two possible outcomes (1 or 0, yes or no, etcetera). 
</p>

## Preparing The Dataset
We must come up with an organized dataset of assigned input and weight values. Below is a representation of my dataset.
| Input | Weights |
| :---:   | :---: |
| 0.6 | 0.4   |
| 0.4 | 0.3   |
| 0.4 | 0.3   |

## Multiplying Corresponding Inputs & Weights
The input of 0.6 with a corresponding weight of 0.4 is the most significant since its weight is greater than the others. To reach a conclusion, we can multiply each input by its corresponding weight. 

x0 * w0 = 0.6 * 0.4 = 0.24

x1 * w1 = 0.4 * 0.3 = 0.12

x2 * w2 = 0.4 * 0.3 = 0.12

## Finding The Sum of the Corresponding Products
Now we need to find the sum of the corresponding products. If you add them all up you should get an answer of **0.48**.

## Applied Activation Function

Next, we check if the sum exceeds a certain threshold, also known as the bias. To evaluate whether the threshold has been met, we use an activation function called the step function. Our bias/threshold value will be 0.5.

**Step Function Formula:** f(x) = 1, if x > 0.5 0, otherwise

Since **x** being equal to **0.48** isn't greater than our bias/threshold our final output is 0. 

## Perceptron Overall Diagram
Here is a visual summary that illustrates the key components of the Perceptron Model.
![Untitled](https://github.com/user-attachments/assets/d5551942-d63f-4f2d-a4a3-46c31e3d8b7c)

## Key Notes
1. We learned the basics behind the Perceptron Model.
2. We constructed a structured dataset containing our inputs and corresponding weights.
3. We multiplied each input by its respective weight.
4. We computed the sum of the resulting products.
5. The summed value was then passed through an activation function (the step function).
6. The threshold/bias value was set to 0.5.
7. The output was 0, as the computed sum of 0.48 did not exceed the bias value of 0.5.

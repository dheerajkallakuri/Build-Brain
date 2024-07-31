# Building a Brain in 10 Minutes

## Introduction

Artificial neural networks have been developed to mimic the learning capabilities of humans and animals. This brief guide walks you through a hands-on exercise in image classification using the Fashion MNIST dataset, showcasing how neural networks can learn through a process similar to human trial and error.

## Data

Our challenge is to classify articles of clothing using computer vision. We will use the Fashion MNIST dataset, which includes various images of clothing.

Neural networks, inspired by human learning, use a method similar to digital flashcards. Our goal is for the artificial brain to guess the type of clothing in each flashcard, learn from its mistakes, and improve over time.

To ensure our models are learning, we will divide our data into a training dataset and a validation dataset. The training dataset is used to teach the model, while the validation dataset is used to test its understanding.

## Building a Neuron

Neurons are the fundamental units of a neural network. They process numerical inputs to produce outputs. Here’s how we can break down building a neuron into three key steps:

1. **Defining the Architecture**
2. **Initiating Training**
3. **Evaluating the Model**

### Defining the Architecture

Biological neurons transmit information through electrical impulses. In artificial neural networks, we simplify this process using mathematical formulas. We will start with a basic linear regression function: 

``` y = mx + b ```

where:
- ``` x ``` represents the input (like pixel values)
- ``` y ``` is the output
- ``` m ``` and ``` b ``` are variables that adjust as the model learns

In practice, each pixel in our images has a weight. For example, in a 28x28 pixel image, each of the 784 pixels will have a corresponding weight. Thus, our equation becomes:

``` y = w0x0 + w1x1 + w2x2 + ... + b ```

### The Math

Computers use discrete values (0s and 1s), while biological systems use more continuous values. Early artificial neurons used linear regression to approximate this continuous input-output relationship.

For our Fashion MNIST dataset:
- Each pixel value ranges from 0 (black) to 255 (white)
- We assign a weight to each pixel value

For more info:

https://learn.nvidia.com/courses/course?course_id=course-v1:DLI+T-FX-01+V1&unit=block-v1:DLI+T-FX-01+V1+type@vertical+block@bdccdcc4ef7549e59043f146d354e9e5

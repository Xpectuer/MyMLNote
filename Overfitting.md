# Methods to imporve OVERFITTING

## What OVERFITTING looks like?


>Normally, when a model performs **well** in **train data set** but **poor** in **test set**.

![image of overfitting](images/overfitting.png)
***
## Why OVERFITTING?

### <font color="#B40404 ">Model</font>

When it comes to overfitting, we should really think about the **model** in use.

Once it get too much complexity, the problem of efficiency and overfitting arises.

### <font color="#B40404 ">Data set</font>

When you feed too **little** size of data set for **training** ,the problem arises.

### <font color="#B40404 ">Unvoidable Problem</font>

The problem of OVERFITTING is **unavoidable** because you will never know which size is proper to gain the equilibrim between **efficiency** and the 
***solution of overfitting***

However, what we can do is to relief the problem.Thus, we have these method to **improve** the situation.

## Solutions

### ReLU 
> **Rectified Linear Unit:**
>An activate function  defined as the positive part of its argument

$f(x)=x^{+} =max(0,x)$    
 
![image for ReLU](images/ReLU.png)

Reasons:
1. Fast to compute
2. Infinite sigmoid with different biases
3. Vanishing **gradient problem**







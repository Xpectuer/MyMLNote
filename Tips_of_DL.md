# Tips for DNN

## Vanished Gradient Problem

In our previous neuron network building, we used **sigmoid** as an activate function 

<font size='6'>$\sigma$(z)=$\frac{1}{1+e^{-z} }$</font>

However, the **activate function** may have some problems.  

### <font color='red'>Too Deep Network</font>

As the network deepen, the gradient in deeper layer tend to be larger.  
$\Delta depth ⬆ \to\Delta w⬆$

![VGP](images/VGP1.png)

 When the input gradient was very **low**, the output side has already complete the **converge** (**high gradient**).

 ![sigmoid](images/sigmoid.png)

 When input changes, output changes very **slow** in **output**

 ## Solutions

 ### <font color='red'>Better activate function</font>

#### ***ReLU*** 
> **Rectified Linear Unit:**
>An activate function  defined as the positive part of its argument

$f(x)=x^{+} =max(0,x)$    
 
![image for ReLU](images/ReLU.png)

Reasons:
1. Fast to compute
2. Infinite sigmoid with different **biases**
3. Biological reason

Problems:
1. Linear: considered as non-linear in different regions
2. Unable to **differential**  (Do not have **smaller** **gradient**)

#### ***ReLU - variant***

![ReLU -variant](image/../images/reLU_variant.png)

### <font color='red'>Maxout</font>

>**idea:**   
**learnable **activation function****

![Maxout](images/Maxout.png)

1. input value multipies weight 
2. find the max value as the input of next neuron
3. next iteration

**tip:** ReLU is a special cases of Maxout

![ReLU is a special cases of Maxout](images/ReLU_as_a_sp_case.png)

![more than ReLU](images/More_Than_RELU.png)

### Maxout-Training
***point***  
Find the max **z** value, discard the others.

![how to train](images/Training_for_Maxout.png)


### Adaptaive Learning Rate









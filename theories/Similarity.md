# Jaccard Similarity

## Also seen as Jaccard Index
[wikipedia](https://en.wikipedia.org/wiki/Jaccard_index)

### Basic Concept
A statistic used for measuring the **simularity and diversity** sample sets

>**The Jaccard coefficient** measures the similarity of between the finite sample sets, and is defined as the intersection divided by the **size** of union of the sample sets.


<font size='5'>$J(A,B)=\frac{|A\cap B|}{|A\cup B|}=|\frac{|A\cap B|}{|A|+|B|-|A\cap B|}|$</font>

<font color='red'>tips:</font>  

1.  If A and B are both empty, define   $J(A,B)=1$
   
2.  $0\le J(A,B) \le1$
   
 >**The Jaccard distance**  
 The scale that measure dissimiarity between sample sets, is complementary(互补的) to the **Jaccard coefficient**

<font size='5'>
 
 $d_{J}(A,B)=1-J(A,B)=\frac{|A\cup B|-|A\cap B|}{|A\cup B|}$

</font>

>**Alternative interpretation** of the Jaccard distance is as the ratio of the size of the [symmetric difference](https://en.wikipedia.org/wiki/Symmetric_difference)

![symmetric difference](images/symmetric_difference.png)

$A\Delta B=(A\cup B)-(A\cap B)$


This interpretaion commonly used as the calculation of an $n\times n$ matrix for [clustering](https://en.wikipedia.org/wiki/Cluster_analysis) and [multidimentional scaling](https://en.wikipedia.org/wiki/Multidimensional_scaling)(MDS)

If $\mu$ is a measure on a [measurable space](https://en.wikipedia.org/wiki/Measurable_space) $X$,then we define the Jaccard coefficient by

<font size='5'>

$J_{\mu}(A,B)=\frac{\mu(A\cap B)}{\mu (A\cup B)}$

</font>

and

<font size='5'>

$d_{\mu}(A,B)=1-J_{\mu}(A,B)=\frac{\mu(A\Delta B)}{\mu(A\cap B)}$


</font>

***
# Cosine Similarity
[wikipedia](https://en.wikipedia.org/wiki/Cosine_similarity)

>A measure of similarity between two non-zero vectors of an [inner product  space](https://en.wikipedia.org/wiki/Inner_product_space)  


## Definition
<font size='5'>$similarity =cos(\theta)=\frac{A\cdot B}{||A||B||}=\frac{\sum_{i=1}^{n}A_{i}B_{i}}{\sqrt{\sum_{i=1}^{n}A_{i}^{2}}\sqrt{\sum_{i=1}^{n}B_{i}^{2}}}$
</font>

## Normalisation issues

<font size='5'>

$if\ A=[A_{1},A_{2}]^{T}$

$then\ \bar{A}=[\frac{(A_{1}+A_{2})}{2},\frac{(A_{1}+A_{2})}{2}]^{T}$


$so\ A-\bar{A}= [\frac{(A_{1}-A{2})}{2},\frac{(-A_{1}+A_{2})}{2}]^T$

</font>

## Angular distance and similarity
>For the vector elements may be positive or negative
<font size='5'>

$angular\ distance =\frac{cos^{-1}(cosine\ similarity)}{\pi}$ 

$angular\ similarity=1-angular \ distance$

</font>

>For those always positive

<font size='5'>

$angular\ distance =\frac{2\cdot cos^{-1}(cosine\ similarity)}{\pi}$ 

$angular\ similarity=1-angular \ distance$

</font>

## Otsuka-Ochiai coefficient  

>Useful in **set** similarity researches and here A and B are both sets.
<font size='5'>

$K=\frac{|A\cap B|}{\sqrt{|A|\times |B|}}$

</font>
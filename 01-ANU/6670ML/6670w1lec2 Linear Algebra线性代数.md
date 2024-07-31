- Base concepts: vectors and systems of linear equations 
- 线性代数：“研究向量和操纵向量的某些规则”
Matrices 
Solving systems of linear equations 

## 1. REVIEW

- **Training** is the process of making the system able to learn.
	- A model that explains a certain situation well may fail in another situation. 
- The training set and test set come from the same distribution (in- distribution vs. out-of-distribution) 
- Before applying a model, check the assumptions!

- Supervised
Input: Data X and **label y** 
Goal: Learn how to map X to y
Examples: Regression, classification Quick review 

- Unsupervised
Input: Data X, **no label** 
Goal: Learn underlying structure of data 
Examples: Clustering, dimensionality reduction 

## 2.1 Basic Concepts
- Base concepts: 
	- vectors and systems of linear equations 
	- 向量和线性方程组 
	- Matrices 
		- 矩阵 
	- Solving systems of linear equations \
		- 解线性方程组
![[Pasted image 20240725152422.png]]


![[Pasted image 20240731003904.png]]

Multiplying:乘法

## 2.2 Matrices

![[Pasted image 20240731004655.png]]


ℝ𝑚𝑚×𝑛𝑛 is the set of all real-valued 𝑚𝑚, 𝑛𝑛 -matrices.

### 2.2.1 Matrix Addition and Multiplication



Multiply
![[Pasted image 20240731005720.png]]

![[Pasted image 20240731005807.png]]

#### 乘法性质
在算术里我们知道：

3 × 5 = 5 × 3  
（乘法的[互换律](https://www.shuxuele.com/associative-commutative-distributive.html)）

但在矩阵的领域这通常是**不**正常的（矩阵乘法**并非可互换**）：

AB ≠ BA

当乘法的次序改变，答案亦（通常）**改变**。

关联性 分配律 与同一矩阵相乘
![[Pasted image 20240731005957.png]]
##### 单位矩阵

"单位矩阵" 是矩阵领域里的 "1":

![单位矩阵](https://www.shuxuele.com/algebra/images/matrix-identity.gif)  
3x3 单位矩阵  

- 单位矩阵是"方形"的（行与列数目相同），
- 对角线全是**1**，其他全是**0**。
- 符号为大写字母 **I**。  
    

它是个**特别的矩阵**，因为把它和一个矩阵相乘，后者不变：
A × I = A  
I × A = A

### 2.2.2 Inverse逆矩阵 and Transpose和转置矩阵

![[Pasted image 20240731010726.png]]

![[Pasted image 20240731010737.png]]


- A矩阵不可逆   
	- <=> |A| = 0  
	- <=> A的列(行)向量组线性相关  
	- <=> R(A)<n  
- <=> AX=0 有非零解  
	- <=> A有特征值0.  
	- <=> A不能表示成初等矩阵的乘积  
	- <=> A的等价标准形不是单位矩阵
	- <=>**不满秩，则不可逆**
	- 


- 重要特性
![[Pasted image 20240731010920.png]]


- Symmetric 对称性
- product 乘积
![[Pasted image 20240731010956.png]]

### 2.2.3 Multiplication by a Scalar标量
![[Pasted image 20240731014038.png]]

![[Pasted image 20240731014046.png]]

### 2.2.4 Compact Representations of Systems of Linear Equations 紧凑表示




## 2.3 Solving systems of linear equations
### 2.3.1 Gaussian elimination-高斯消元法


### 2.3.2 Elementary Transformations 基本变换

将矩阵变为阶梯矩阵
row-echelon form (REF)




# Calculating the Inverse with Gaussian Elimination

![[Pasted image 20240731015307.png]]



# Moore-Penrose pseudo-inverse

摩尔-彭罗斯伪反演


We can calculate 𝑨𝑨−1only when 𝑨𝑨 is a square matrix and is invertible

![[Pasted image 20240731022344.png]]











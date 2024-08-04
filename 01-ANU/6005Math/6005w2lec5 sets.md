# Making new sets from old 
## 运算
Suppose that A and B are subsets of a universe U

The **union并** of A and B, denoted A ∪ B, is the set
{x ∈ U | (x ∈ A) ∨ (x ∈ B)

The **intersection交** of A and B, denoted A ∩ B, is the set
{x ∈ U | (x ∈ A) ∧ (x ∈ B)

The difference of B **minus** A, or B **without** A, denoted B − A or B \\ A, is the set {x ∈ U | (x ∈ B) ∧ (x̸ ∈ A)}


The **complement补集** of A (in U), denoted Ac , is the set {x ∈ U | x̸ ∈ A}
![[Pasted image 20240804115245.png]]
The complement of A cannot be understood unless the universe of discourse has been communicated. 一定要交代全集是啥

The **symmetric difference对称差** of A and B, denoted A△B, is the set {x ∈ U | (x ∈ A) **⊕** (x ∈ B)}


#### Example
Suppose that the universe of discourse is the set Z and let 
O be the set of odd integers 
E be the set of even integers 
P be the set of primes 
C be the set of composite numbers


A **composite number** is a positive integer that can be formed by multiplying two smaller positive integers.
- 合数是由两个较小的正整数相乘而成的正整数。
- 对应素数
***重点***
![[Pasted image 20240804123701.png]]

注意素数和合数不同



## Using logic to prove set identities
![[Pasted image 20240804160854.png]]

## Another way to construct a new set from an old set

![[Pasted image 20240804160913.png]]



# Cartesian products: Another way to make new sets from old 笛卡尔积

## Order and multiplicity 
In sets, there is **no sense of the order** in which elements appear and there is no idea of how many times an elements appears. 

However, in many situations the **order in which data appears is important**, and the same data sometimes appears multiple times. We now look at a construction that allows us to represent order and multiplicity

## Ordered n-tuples

Let n be a positive integer and let x1, x2, . . . , xn be (not necessarily distinct) elements. The ordered n-tuple (x1, x2, . . . , xn) consists of x1, x2, . . . , xn together with the ordering: first x1, then x2, and so forth up to xn. An ordered **2-tuple** is called an **ordered pair**, and an ordered **3-tuple** is called an **ordered triple**

#### examples:
![[Pasted image 20240804161304.png]]























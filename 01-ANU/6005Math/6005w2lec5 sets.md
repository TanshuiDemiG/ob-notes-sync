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



# Cartesian products 笛卡尔积: Another way to make new sets from old 

## Order and multiplicity 
In sets, there is **no sense of the order** in which elements appear and there is no idea of how many times an elements appears. 

However, in many situations the **order in which data appears is important**, and the same data sometimes appears multiple times. We now look at a construction that allows us to represent order and multiplicity

## Ordered n-tuples

Let n be a positive integer and let x1, x2, . . . , xn be (not necessarily distinct) elements. The ordered n-tuple (x1, x2, . . . , xn) consists of x1, x2, . . . , xn together with the ordering: first x1, then x2, and so forth up to xn. An ordered **2-tuple** is called an **ordered pair**, and an ordered **3-tuple** is called an **ordered triple**

#### examples:
![[Pasted image 20240804161304.png]]

## Cartesian product 笛卡尔积

- expression
	- “the set of all ordered n-tuples with elements a1, a2, through, an such that a1 comes from A1, a2 comes from A2, through an comes from An.”

- The expression {(a1, a2, . . . , an) | a1 ∈ A1, a2 ∈ A2, . . . , an ∈ An}. 
	- does not appear to conform to the rules of set-builder notation we laid out in the last lecture 
- because
	- the domain part introduces variables but does not specify a domain for each; 
	- the “predicate” **does not appear to be a single predicate**


#### Example
![[Pasted image 20240805121511.png]]

## Strings and languages                 

Let A be a set. A string (or word) of length n **over (the alphabet)**
A is an ordered n-tuple, written without parentheses or commas, in which every element is taken from A. 
The **null string** (or empty word) over A is the “string” with no characters. 
The null string over A is denoted λ and said to have length 0. 
We write A∗ for the set of all strings over the alphabet A. 
Any subset of A∗ is called **a language.**

#### example of language


![[Pasted image 20240805122144.png]]


# Partitions 分区: A structure for recognising that a classification works well
分区： 识别分类效果的结构
A common task in any discipline (science, mathematics, philosophy, humanities, ...) is that of classifying things of a certain type into various sub-types. Thanks to our development of set theoretic tools, we have a way to formalise what it means for such a classification scheme to work really well

任何学科（科学、数学、哲学、人文学科......）都有一项共同的任务，那就是将某一类型的事物划分为不同的子类型。得益于集合论工具的发展，我们有了一种方法，可以将这种分类方案真正有效的含义形式化

e.g. 
We classify each integer as positive, negative or 0

## disjoint sets
joint sets Sets A, B are called disjoint when A ∩ B = ∅

- Given a set of sets **S**, the sets in S are said to be **pairwise disjoint成对互联** 
	- when 
![[Pasted image 20240805124323.png]]
#### example of pairwise disjoint
![[Pasted image 20240805124422.png]]

## Partitions 分区





























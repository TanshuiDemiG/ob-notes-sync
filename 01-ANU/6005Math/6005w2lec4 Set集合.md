

# Sets 集合定义
- A set is a ***collection of elements***.
- The notation a ∈ S is read “a is an element of S”. 

## **Axiom** of extensionality延展定理 
- A set is a collection of elements. This is an **intuitive直观的** statement, but cannot be considered a definition

	- A set is determined by what its elements are. 
	- **No importance is placed on the order** in which elements are considered, or how many times an element appears in the set. Membership is the only things that matters. 无序性

- 属于 a ∈ S 


 # Methods for describing a set（3 ways） 表达
- Describe S with language that communicates the precise nature of the set
- Use set-roster notation 
- Use set-builder notation

- We write **∅** for the emptyset. **空集**
- It is the set with no elements Let **Z**≥0 denote the set of non-negative integers **正整数集**
- Let **N** denote the set of positive integers (sometimes called the natural numbers). **自然数 normal **
	- Note that 0̸ ∈ N but 0 ∈ Z≥0. 
- Let **Z** denote the set of **integers**. 
- Let **Q** denote the set of **rational numbers**.**有理数** 
- Let **R** denote the set of **real numbers**.**实数**

### Predicates with domain ∅ 域∅的谓词
if D is empty
	∀x p(x)  TRUE
	**∃x p(x)   FALES**
		**NO elements in domain**
	
- if D is not empty
	- ∀x p(x) → ∃x p(x).
	- ∃!x p(x) → ∃x p(x).


### Specifying membership with precision


## notation 集合符号 表达
### Set-roster 
- roster 就是{}
- normally
	- Describe each of the following sets in words. 
	- S = {Helium, Argon, Neon, Krypton, Xenon, Radon} 
	- O = {. . . , −3, −1, 1, 3, 5, . . . } **ODD**
	- T = {2, 3, 5, 7, . . . } **sometimes P Prime numbers 素数**
	- U = {3, 5, 7, . . . , 19}
### Set-builder notation
- write {x ∈ D | p(x)}
- The use of | to separate the specification of the domain from the predicate is not universal.
- Other commonly used symbols include ‘:’ and ‘;’. In all cases, the symbol may be read as **“such that” or “for which”**
![[Pasted image 20240804110700.png|1000]]


**Example**:
- Let T = {p ∈ Z+ | p and p + 2 are both prime}
- The set T has infinitely many elements

-  **the Twin Prime Conjecture猜想**
	- 孪生质点猜想


## subsets

Let A and B be sets. We say that A is a subset of B, or A is contained in B, and we write A ⊆ B, when every element of A is also an element of B. 
Symbolically, A ⊆ B ⇔ ∀x (x ∈ A → x ∈ B).
You may say that ⊆ is the set **theoretic analogue** of IMPLIES in logic
可以说，⊆ 是逻辑中 IMPLIES 的**集合论类似物**


### Understanding A̸不 ⊆ B
We often indicate that the negation of a statement is true by placing a diagonal slash through the key symbol in the statement. 反证

A̸ ⊆ B 
⇔ ¬(A ⊆ B) 
⇔ ¬∀x (x ∈ A → x ∈ B) 
⇔ ∃x ¬(x ∈ A → x ∈ B) 
⇔ ∃x x ∈ A ∧ (¬(x ∈ B)) 
⇔ ∃x x ∈ A ∧ x̸ ∈ B.

We can interpret this intuitively: A̸ ⊆ B means that there is at least one element in A that is not in B.


### Proper containment 真包含

We say that A is a proper subset of B, or A is properly contained in B, and write A ⊊ B, when every element of A is in B but there is at least one element of B that is not in A. Symbolically
![[Pasted image 20240804112759.png]]

![[Pasted image 20240804113845.png]]

![[Pasted image 20240804114124.png]]
- c是复数

### Set equality

![[Pasted image 20240804113004.png]]

![[Pasted image 20240804113845.png]]

### to proof
正反两次证明

![[Pasted image 20240804114430.png]]

![[Pasted image 20240804114712.png]]

### Alternate proof 可选证明

![[Pasted image 20240804114748.png]]




















## Universe of discourse


1111












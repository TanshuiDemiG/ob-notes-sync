# Russell’s Paradox罗素悖论
- Most sets are not members of themselves.
P̸ ∈ P
- but some sets are members of themselves. 
- Examples: 
	- The set of all sets. 
	- The set of all things that are not birds.
- 出现自指


## Axiomatic Set Theory 公理集合论

###  ZFC (Zermelo-Fraenkel with choice）
- **Axiom 1:** 
	A set T can only be defined as a subset of a known set U. That is, the definition must have the form: T = {x ∈ U | p(x)} where the domain of predicate p includes all elements of U.
	公理 1：集合 T 只能定义为已知集合 U 的子集：
	T = {x ∈ U | p(x)} 其中谓词 p 的域包括 U 的所有元素。

e.g. A: set of all animals. B = {b ∈ A | b is a bird} ⊆ A.
#### 策梅洛-弗兰克尔集合论的一些关键公理：

1. **外延公理（Axiom of Extensionality）**：如果两个集合有相同的元素，那么它们是相等的。这确保了集合是由其元素唯一确定的。
    
2. **正则公理（Axiom of Regularity, Axiom of Foundation）**：每个非空集合 AAA 都包含一个与 AAA 不相交的元素。这个公理直接防止了集合包含自己或包含一个循环的情况。
    
3. **分离公理模式（Axiom Schema of Separation）**：确保只能构造某些特定的子集，而不是任意的集合。这限制了集合的构造方式，避免了许多潜在的悖论。
## Russell’s paradox removed 消除罗素悖论
in ZFC we can still say that a set S is regular if and only if it satisfies the condition (predicate) S̸ ∈ S. However we cannot define R as the set of all regular sets. Instead, for any known set of sets U we can define RU by 
RU = {S ∈ U | S is regular} = {S ∈ U | S̸ ∈ S}






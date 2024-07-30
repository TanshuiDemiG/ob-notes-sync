# Logical Equivalences恒等式 

When two statement forms f , g have identical truth tables we say they are ***logically equivalent*** and write f ≡ g

(***Alt. Def.:*** When f , g are statement forms and f ↔ g is a tautology, we say that f and g are logically equivalent and write f ≡ g.)


***t is toutology c is contridiction***
- 所有下述公式为  ***恒等式***
- **commutative** laws 交换
	- P合取或析取Q = Q合取或析取P
- **assiciative** laws 同位法
	- p合取(P合取R)= (P合取Q)合取R
- **distrubtive** laws 分配律
	- P合取（Q析取R） = （P合取Q）析取（P合取Q）
	- 反之亦然
- **identity** laws  同一律
	- P析取T1恒等于P P合取C0恒等于P
- **negation** laws 否定律
	- p析取~p为t真 p合取~p为c恒假
- **double negative** law双重否定
	- ~\~p为p
- **idempotent** law 幂律（归一律）
	- p析取p等于p
	- p合取p等于p
- **universal** **bond** laws
	- p析取t 为t
	- p合取c为c
- **De Morgan's** laws 德摩根定律
	- ~（p析取q）恒等于~p合取~q
- **Absorption** laws 吸收律
	- p析取（p合取q）恒等于P
	- p合取（p析取q）恒等于p
- Negation of t and c
	- 非重言为永假
	- 非永假为重言
- 
### example: xor equivalent
equivalent is 
p ⊕ q 
≡ (p ∨ q) ∧ ¬(p ∧ q)
≡ (p ∧ ¬q) ∨ (p ∧ ¬q)



## vocabulary associated to p →q
- p →q
	- p implies q 
	- if p then q 
	- p only if q 
	- q if p
- The **converse** of p → q is q → p 
	- 倒数
- The **inverse** of p → q is ¬p → ¬q 
	- 逆蕴
- The **contrapositive** of p → q is ¬q → ¬p
	- 逆反

- Which, if any, of the following statements concerning p → q are true: 
	- A. The converse of the inverse is the contrapositive. 
	- B. The inverse of the converse is the contrapositive. 
	- C. The inverse of the contrapositive is the converse. 
	- D. The converse of the contrapositive is the inverse. 
	- E. The statement form is logically equivalent to its contrapositive. 
	- F. **The inverse is logically equivalent to the converse.** 
	- G. **The statement is not logically equivalent to its converse.**
# 推理
## 充要条件 Necessary and sufficient conditions
- p is a **sufficient** condition for q means p → q. 
	- 必要条件
- p is a **necessary** condition for q means ¬p → ¬q. 
	- 充分条件
	- 等价于 q推p
- Since (¬p → ¬q) ≡ (q → p), we can also say: 
	- p is a necessary condition for q means q → p; 
	- p is a necessary and sufficient condition for q means p ↔ q. 
	- In view of the above terminology, statements of the form p → q and p ↔ q are often referred to as ***conditional statements.（条件语句）***
- 定理
	- ¬(¬p) ≡ p (1) 
	- ¬(p ∧ q) ≡ ¬p ∨ ¬q (2) 
	- ¬(p ∨ q) ≡ ¬p ∧ ¬q (3) 
	- ***¬(p ⊕ q) ≡ (p ∧ q) ∨ (¬p ∧ ¬q) (4)*** 
	- ¬(p → q) ≡ p ∧ ¬q  (5)
	- ¬(p ↔ q) ≡ (p ∧ ¬q) ∨ (¬p ∧ q)


# 功能完整性Functional completeness
##  真值表转换逻辑表达式
- 找到真值表中的真值式子statement forms进行合取（因为永真，故每个变元都真），括号外析取
- 
①找到真值表**输出为1**的行

②输入变量之间是**与**的关系，输出状态之间是**或**的关系

  对于输入输出变量，取**1**值用**原变量**表示，取**0**值用**反变量**表示

③得出逻辑函数表达式并化简（最好用等式或卡诺图法化简）

**（也可以理解为写出最小项表达式）**


## DNF 析取***范式***
A **compound** statement is in ***disjunctive normal form*** it is a disjunction of conjunctions, and in each of the conjunctions each statement variable or its negation appears but not both. 
Example: (p ∧ q ∧ ¬r) ∨ (¬p ∧ q ∧ r) ∨ (¬p ∧ ¬q ∧ r) is in **disjunctive normal form**.

## Theorem 定理
**Theorem**: Every statement form that is not a contradiction is logically equivalent to a disjunctive normal form.
**每一个非假的命题公式都有析取范式**

**Proof**: Consider the truth table of some **arbitrary任意** statement form that is not a contradiction.
**假设一个非矛盾式**

Using a conjunction in which each statement variable or its negation appears but not both, we can make a statement form with a truth table in which there is exactly one T.
**必有成真变元值**

By intentionally choosing between the statement variables and their negations, we can make that T be in any row of the truth table. To make a statement form to match any particular truth table we note the rows in which T’s appear, we use a conjunction for each such row and we combine these conjunctions into a disjunction.
**记录成真条件，行合取（因为永真，故每个变元都真），括号外析取，得到析取范式**




**Theorem**: A set of logical connectives A is functionally complete if any statement form is logically equivalent to a statement form that is made using only statement variables, parentheses, and connectives from A.
- 连接词在集合A上可以完整表达，则具备功能完整性
**Corollary**: The set {∧, ∨, ¬} is a functionally complete set of logical connectives..
- 连接词全功能集
**To proof :**
	Consider the truth table of an arbitrary statement form X. If X is not a contradiction, then by the previous frame we can present the statement form in disjunctive normal form. If X is a contradiction, then then the contradiction p ∧ ¬p, where p is a statement variable of X is logically equivalent to the statement form X.
如：
¬  ∧ ∨ 
¬      ∨ 
¬  ∧ 
¬ → 
补充：
¬ 与非↑ NAND
	不同时 为真z
¬ 或非↓ NOR
	同时为假



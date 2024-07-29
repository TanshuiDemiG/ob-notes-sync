# Logic
## Logical Equivalences恒等式 

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
	- 反推出

- Which, if any, of the following statements concerning p → q are true: 
	- A. The converse of the inverse is the contrapositive. 
	- B. The inverse of the converse is the contrapositive. 
	- C. The inverse of the contrapositive is the converse. 
	- D. The converse of the contrapositive is the inverse. 
	- E. The statement form is logically equivalent to its contrapositive. 
	- F. **The inverse is logically equivalent to the converse.** 
	- G. **The statement is not logically equivalent to its converse.**

# 充要条件 Necessary and sufficient conditions
- p is a **sufficient** condition for q means p → q. 
	- 必要条件
- p is a **necessary** condition for q means ¬p → ¬q. 
	- 充分条件
	- 等价于 q推p
- Since (¬p → ¬q) ≡ (q → p), we can also say: 
	- p is a necessary condition for q means q → p; 
	- p is a necessary and sufficient condition for q means p ↔ q. 
	- In view of the above terminology, statements of the form p → q and p ↔ q are often referred to as ***conditional statements.（条件语句）***


# Set Equality

**Definition:** Two sets are equal (A = B) if they **contain the same elements**

### To show equality:

- Examine **all the elements**
- Show $A ⊆ B$ and $B ⊆ A$
- Use the Laws of Set Operations

**Venn diagrams** can help visualize, **but are not rigorous.**

# Laws of Set Operations

**Material**: P14

| Commutativity | $A ∪ B = B ∪ A$
$A ∩ B = B ∩ A$ |
| --- | --- |
| Associativity | $(A ∪ B) ∪ C = A ∪ (B ∪ C)$
$(A ∩ B) ∩ C = A ∩ (B ∩ C)$ |
| Distribution | $A ∪ (B ∩ C) = (A ∪ B) ∩ (A ∪ C)$
$A ∩ (B ∪ C) = (A ∩ B) ∪ (A ∩ C)$ |
| Identity | $A ∪ ∅ = A$
$A ∩ U = A$ |
| Complementation | $A ∪ (A^c) = U$
$A ∩ (A^c) = ∅$ |

# Derived Laws

| Idempotence | $A ∩ A = A$
$A ∪ A = A$ |
| --- | --- |
| Double complementation | $(A^c)^c = A$ |
| Annihilation | $A ∩ ∅ = ∅$
$A ∪ U = U$ |
| de Morgan’s Laws | $(A ∩ B)^c = A^c ∪ B^c$
$(A ∪ B)^c = A^c ∩ B^c$ |

# Two Useful Results

## Principle of Duality

**Definition:** $dual(A)$ 就是通过

- 将**交集**符号 $∩$ 替换为**并集**符号 $∪$
- 并将**空集 $∅$ 替换为全集 $U$ ，反之亦然，得到的表达式。

**Theorem**: 如果可以使用集合运算法则证明 $A1 = A2$，那么同样可以证明 $dual(A1) = dual(A2)$

## Uniqueness of complement (补集的唯一性)

**Theorem:** $A ∩ B = ∅$ and $A ∪ B = U$ if, and only if, $B = A^c$. 
**Application:** 判断一个集合是否是另一个集合的补集，而不需要直接给出补集的定义

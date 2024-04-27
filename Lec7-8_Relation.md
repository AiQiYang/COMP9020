# Definition and Examples

**Definition:**

- n-ary relation:
    - is a subset of the Cartesian product of n sets $R ⊆ S_1 × S_2 × . . . × S_n$
    - tuples related by R
        - $(x_1, x_2, . . . , x_n) ∈ R$ or $R(x_1, x_2, . . . , x_n)$
- Binary relation:
    - $R ⊆ S × T$
- Domain of $R$
    - $U = S_1 × S_2 × . . . × S_n$
    - $R$ is a relation on $U$

**Examples:**

- Equality: $=$
- Inequality: $≤, ≥, <, >, \neq$
- Divides relation: $|$
- Element of: $∈$
- Subset, superset: $⊆, ⊂, ⊇, ⊃$
- Congruence modulo n: $m =_(n) p$

**Defining Relations:** 

1. Explicit enumeration
2. Attribute identification
3. Construction from other relations

# Binary Relations

## Special Relations

- Identity: $I={(x,x):x∈S}$ representing elements on the diagonal are equal
- Empty: $∅$
- Universal: $S*S$

## Operations for binary relations

- Converse:
    - If $R ⊆ S × T$ is a relation, then $R^← ⊆ T × S$:
    $R^← =def {(t, s) ∈ T × S : (s, t) ∈ R}$
- Composition:
    - If $R_1 ⊆ S × T$ and $R_2 ⊆ T × U$ then $R_1; R_2 ⊆ S × U$:
        - $R_1; R_2 =def \{(s, u) ∈ S × U\}$: there exists $t ∈ T$ such that $(s, t) ∈ R_1$ and $(t, u) ∈ R_2$

### Fact:

$(R^←)^← = R$

## Relational images

Given $R ⊆ S × T$, $A ⊆ S$, and $B ⊆ T$

- **Relational image** of $A, R(A$):
    
    $R(A) =def {t ∈ T : (s, t) ∈ R for some s ∈ A} $
    
- Relational pre-image of $B, R^←(B)$:
    
    $R←(B) =def {s ∈ S : (s, t) ∈ R for some t ∈ B} 
    

# Properties of Binary Relations

- **(Fun)Function**:
    
    For all $s \in S$, there is at most one $t \in T$such that $(s, t) \in R$
    
- **(Tot)Total:**
    
    For all $s \in S$, there is at least one $t \in T$such that $(s, t) \in R$
    
- **(Inj) Injective(单射(映射))**
    
    For all $t \in T$, there is at most one $s \in T$such that $(s, t) \in R$
    
- **(Sur) Surjective(满射)**
    
    For all $t \in T$, there is at least one $s \in T$such that $(s, t) \in R$
    
- **(Bij) bijective(双射)**
    
    Injective and surjective
    

### Function and Function Properties

- **Partial function** is a binary relation that is (Fun).
- A **function** is a binary relation that is **(Fun) and (Tot).**
- An **injection** is a function that is (Inj).
- A **surjection** is a function that is (Sur).
- A **bijection** is a function that is (Bij)

## Properties of Binary Relations $R \in S \times S$

- **(R)Reflexive(自反性)**
    
    For all $x∈S:(x,x)∈R$
    
- **(AR)Antireflexive**(**反自反性**)
    
    For all $x∈S:(x,x)\notin R$
    
- **(S)Symmetric(对称性)**
    
    For all $x,y∈S$: If $(x,y)∈ R$ then $(y,x)∈R$
    
- **(AS)Antisymmetric(反对称性)**
    
    For all $x,y∈S$: If $(x,y), (y, x)∈ R$ then

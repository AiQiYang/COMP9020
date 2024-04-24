# Introduction to Sets

## Set

**Definition:** A set is a collection of objects (elements).

- Order and multiplicity of elements is not considered
- If $x$ is an element of $A$ we write $x ∈ A$

## Subset

**Definition:** $S \subseteq T$, where every element in set $S$ is also an element of set $T$.

**Notation:**

- $S ⊆ T$: includes the case where $S = T$
- $S ⊂ T$: $S ⊆ T$ but $S \neq T$, meaning all elements of the first set are contained in the second set, but the second set has at least one additional element not in the first set
- $∅ ⊆ S$ for all sets $S$
- $S ⊆ U$ for all sets $S$

# Defining sets

1. Explicit enumeration of their elements
2. Defining subsets through logical properties
3. Constructing new sets from already defined sets
    1. Union $(∪)$: includes all elements from both sets, with each element appearing only once
    2. Intersection $(∩)$
    3. Complement $(·^c)$
    4. Set difference $(\backslash)$
    5. Symmetric difference $(⊕)$: includes elements that belong to only one set but not both $= (A / B) ∪ (B / A) = (A ∪ B) - (A ∩ B)$
    6. Power set Pow $(X)$: includes all subsets of X
    7. Cartesian product $(×)$
        1. $∅ × S = ∅$, for every $S$
        2. $|S × T| = |S| · |T|$
        3. $\left| \times_{i=1}^n S_i \right| = \prod_{i=1}^n \left| S_i \right|$: the cardinality of the Cartesian product of multiple sets equals the product of their individual cardinalities

**Fact:**

$A ∪ B = B$ iff $A ∩ B = A$ iff $A ⊆ B$ 

## Cardinality

**Definition:** The number of elements in a set, $|X|$ = #$(X) = card(X)$

# Formal Languages

## Symbols

$Σ$ — alphabet, a finite, nonempty set

The empty word, $λ$, is the unique word with no symbols

$length(vw) = length(v) + length(w)$

## Sets of words

- $Σ^k$ or $Σ^{=k}$: The set of all words of length k
- $Σ^{≤k}$: The set of all words of length at most k
- $Σ^∗$: The set of all finite words
- $Σ^+$: The set of all nonempty words

## Language

A language is a subset of $Σ^∗$

### Set Operations for Languages

- Union $(∪)$
- Intersection $(∩)$
- Complement $(·^c)$
- Set difference $(\backslash)$
- Symmetric difference $(⊕)$: includes elements that belong to only one set but not both $= (A / B) ∪ (B / A) = (A ∪ B) - (A ∩ B)$
- Power set Pow $(X)$: includes all subsets of X
- Cartesian product $(×)$
- Concatenation: {a}, {bc} → {abc}
- Kleene star: concatenating 0 or more words in X
    - $A = \{aa, bb\}$
        
        $A^* = \{λ, aa, bb, aaaa, aabb, bbaa, bbbb, aaaaaa, . . .\}$

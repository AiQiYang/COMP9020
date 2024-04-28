# 1. Induction

**Definition:** A method of proving mathematical propositions; reasoning about objects in a finite way; commonly used for propositions involving natural numbers; involves two steps:

1. **Base Case:** Prove the truth of the proposition for the initial case.
2. **Inductive Step:** If the proposition holds for some natural number, prove that it also holds for the next natural number.

## Induction Reasoning

- Starting from specific examples and then deducing general conclusions
    
    We observe that all swans we have seen are white. These specific examples form our sample of observations. Based on these observations, we infer that all swans are white, i.e., "every swan is white."

Induction reasoning does not provide absolute proof but offers a reasonable inference. In practice, induction reasoning is often effective when our sample of observations is sufficiently large and representative.

**Mathematical induction is a valid variant.**

## Mathematical Induction

Not only based on instances but deduces new cases based on the case where P holds (P(x))

1. **Base Case [B]:** First verify some basic cases, usually n=1, to ensure the property or conclusion to be proved holds in this case.
2. **Inductive Step [I]:** If we know a value x satisfies P(x), then we construct a new value y from the known x and prove that P(y) holds.
3. **Conclusion:** By repeatedly applying the method of constructing y from existing values, we eventually construct the set of all values of interest, i.e., it holds for all values.

# 2. Basic Induction

**Goal:** Show P(n) holds for all $n \in \mathbb{N}$

**Approach:** Show that

**Base case [B]:** P(0) holds; and

**Induction case [I]:** If P(k) holds then P(k + 1) holds

**Conclusion:** P(n) holds for all $n \in \mathbb{N}$

# 3. Variations on basic induction

## 1. Induction From m Upwards

If P(m) **[B]**

∀k ≥ m (P(k) → P(k + 1)) **[I]**

∀n ≥ m (P(n)) **[Conclusion]**

## 2. Induction steps $\ell$ > 1

If P(m) **[B]**

∀k ≥ m (P(k) → P(k + $\ell$)) **[I]**

P(n) for every $\ell$’th

# Number Theory in Computer Science

Number theory in computer science focuses on the theory of integers. Integers are discrete, separate entities rather than continuous.

## Numbers and Numerical Operations

### Notation for numbers

- **Natural numbers:** The set of non-negative integers $\mathbb{N} = \{0, 1, 2, 3, \dots\}$
- **Integers:** The set of all integers, including negative, zero, and positive integers $\mathbb{Z} = \{ \dots, -2, -1, 0, 1, 2, \dots \}$
- **Positive integers:** $\mathbb{Z}_{>0} = \mathbb{N}_{>0} = \{1, 2, 3, \dots\}$
- **Rational numbers:** Any number that can be represented in the form $p/q$, where $q \neq 0$, included in the set of real numbers $\mathbb{Q}$
- **Real numbers:** The set containing all rational and irrational numbers, denoted by $\mathbb{R}$

**Note:**
Although in some cases natural numbers $\mathbb{N}$ and integers $\mathbb{Z}$ may overlap, mathematically they are considered as two different sets, represented by different symbols.

### Numerical Operations

#### Floor and ceiling

$\lfloor . \rfloor : \mathbb{R} \rightarrow \mathbb{Z}$: Floor of $x$, the greatest integer $≤ x$

$\lceil . \rceil : \mathbb{R} \rightarrow \mathbb{Z}$: Ceiling of $x$, the least integer $≥  x$

**Simple properties**:
- $\lfloor -x \rfloor = - \lceil x \rceil, \quad \text{hence} \quad \lceil x \rceil = - \lfloor -x \rfloor$
- For all $t \in \mathbb{Z}$:
    - $\lfloor x + t \rfloor = \lfloor x \rfloor + t$
    - $\lceil x + t \rceil = \lceil x \rceil + t$

#### Absolute value

$|x| = \begin{cases} x & \text{if } x \geq 0 \\ -x & \text{if } x < 0 \end{cases}$

# Divisibility

**Divides:** For $m, n \in \mathbb{Z}$, we say $m$ divides $n$ if $n = k \cdot m$ for some $k \in \mathbb{Z}$, denoted by $m|n$

**Divisible:** For $m, n \in \mathbb{Z}$, we say $n$ is divisible by $m$ if $n = k \cdot m$ for some $k \in \mathbb{Z}$, denoted by $m|n$

$m \nmid n$, $m$ does not divide $n$

**Notion of divisibility applies to all integers**

# Greatest Common Divisor and Least Common Multiple (GCD, LCM)

## Greatest common divisor

The greatest common divisor is the largest positive integer that divides both numbers.

**Definition:** The greatest common divisor of $m$ and $n$, $\text{gcd}(m, n)$, is the largest positive integer $d \in \mathbb{Z}$ such that $d|m$ and $d|n$

## Least Common Multiple

The least common multiple is the smallest positive integer that is a multiple of both numbers.

**Definition:** The least common multiple of $m$ and $n$, $\text{lcm}(m, n)$, is the smallest positive integer $k \in \mathbb{Z}$ such that $m|k$ and $n|k$

$\text{gcd}(m, n)$ and $\text{lcm}(m, n)$ are always taken as non-negative.

**Fact:**

$\text{gcd}(m, n) \cdot \text{lcm}(m, n) = |m| \cdot |n|$

## Prime and Relatively Prime

### Prime numbers

A number $n > 1$ is prime if it is only divisible by $\pm 1$ and $\pm n$

### Relatively Prime

$m$ and $n$ are relatively prime if $\text{gcd}(m, n) = 1$

## Euclid’s gcd Algorithm

$$
\text{gcd}(m, n) = \begin{cases} m & \text{if } m = n \\ \text{gcd}(m - n, n) & \text{if } m > n \\ \text{gcd}(m, n - m) & \text{if } m < n \end{cases}
$$

# Modular Arithmetic

For $m \in \mathbb{Z}$, $n \in \mathbb{Z} > 0$ there exists $q, r \in \mathbb{Z}$ with $0 ≤ r < n$ such that $m = q \cdot n + r$

**Observe:**

- $q = ⌊\frac{m}{n} ⌋$
- $r = m - q \cdot n$

## Modulus operator

1. $m \div n = ⌊\frac{m}{n} ⌋$
2. $m \% n = m - (m \div

# Random Variables and Expectation

## Random Variables

**Definition**: Random variable $X$ is a function from $Ω$ to $Z$. In other words, it associates a number value with **every outcome. 是随机事件的每一个结果**

### Arithmetic to random variables:

- Addition of variables: $X + Y : ω → X (ω) + Y (ω)$
- Multiplication of variables: $X * Y : ω → X(ω) * Y(ω)$
- Scalar addition: $X - k : ω → X(ω) - k$
- Scalar multiplication: $X * k : ω → X(ω) * k$

## Expectation

**Definition:** The expected value (often called “expectation” or “**average**”) of a random variable X is $E(X) = \sum_{k∈Z} P(X = k) · k$

- k: 表示随机变量 $𝑋$可能取的每个值

**期望值提供了对随机变量整体行为的一个总结，反映了在大量重复实验中，该随机变量的平均表现**.

# Linearity of Expectation

For any random variables X, Y and integer k:

- $E(X + Y ) = E(X ) + E(Y)$
- $E(k · X ) = k · E(X )$

## Observation

If $X_1, X_2, . . . , X_n$ are 相互独立且同分布的随机变量, then $E(X_1 + X_2 + . . . + X_n) = E(nX_1) = nE(X_1)$

- 相互独立: 即一个随机变量的取值不会提供关于另一个随机变量取值的任何信息
- 同分布：如果多个随机变量具有相同的概率分布

# Standard Deviation and Variance

## standard deviation

**Definition**: 标准差是衡量数字分布程度的指标

$\sigma = \sqrt{E((X - \mu)^2)}$

## Variance

**Definition:** 方差是与均值的平方差的平均值
$\sigma^2 = E((X - \mu)^2) = E(X^2) - \mu^2$

# IGCSE 0606 Additional Mathematics Comprehensive Notes — Second Edition

These notes are strictly written in accordance with the **Cambridge IGCSE Additional Mathematics (0606) 2028–2030 syllabus**. The Additional Mathematics course builds upon IGCSE Ordinary Mathematics, aiming to deepen understanding in algebra, functions, geometry, trigonometry, and calculus, laying a solid foundation for AS/A Level Further Mathematics, AP Calculus BC, and IB AA HL Mathematics.

Each chapter follows the structure: **Concept Definition → Formula Derivation → Worked Examples**. The examples are drawn from the style of past exam papers, with difficulty aligned to examination requirements.

> **Note**: Some formulas (e.g., sum formulas for arithmetic/geometric progressions, binomial expansion formula) are provided in the exam formula sheet, but these notes still present complete derivations to aid understanding rather than rote memorisation. In the exam, **understanding when to use which formula** is more important than memorising formulas.

---
> These notes are based on the Cambridge IGCSE Additional Mathematics (0606) 2025–2027 syllabus, arranged in a logical cognitive order, covering all topics. They include derivations, worked examples, and common pitfalls. Suitable for self-study.
- These notes are compiled and maintained by **LG-leo**. If you find them helpful, feel free to follow me or leave a ⭐ on GitHub — it helps me continue producing more free learning resources.
- My other course notes: https://github.com/LG-leo?tab=repositories

- This note is maintained by LG-leo. If you find it helpful, feel free to follow me or leave a ⭐ on GitHub. It helps me keep producing more free study resources. Check out my other notes: https://github.com/LG-leo?tab=repositories

---

## Table of Contents

- [Chapter 1: Sequences, Permutations, Combinations, and the Binomial Theorem](#chapter-1-sequences-permutations-combinations-and-the-binomial-theorem)
- [Chapter 2: Vectors and Rates of Change](#chapter-2-vectors-and-rates-of-change)
- [Chapter 3: Quadratic Functions (Including Polynomial Factors)](#chapter-3-quadratic-functions-including-polynomial-factors)
- [Chapter 4: Functions (Linear, Cubic, Exponential, Logarithmic)](#chapter-4-functions-linear-cubic-exponential-logarithmic)
- [Chapter 5: Differentiation (Derivatives)](#chapter-5-differentiation-derivatives)
- [Chapter 6: Equations and Inequalities (Graphical Methods)](#chapter-6-equations-and-inequalities-graphical-methods)
- [Chapter 7: Integration (Indefinite and Definite Integrals)](#chapter-7-integration-indefinite-and-definite-integrals)
- [Chapter 8: Trigonometry (Including Radians)](#chapter-8-trigonometry-including-radians)
- [Chapter 9: Geometry (Straight Lines and Circles)](#chapter-9-geometry-straight-lines-and-circles)
- [Chapter 10: Comprehensive Applications](#chapter-10-comprehensive-applications)

---

# Chapter 1: Sequences, Permutations, Combinations, and the Binomial Theorem

This chapter brings together three topics that may seem different but share a common core. **Sequences** train your ability to discover patterns and compute sums; **permutations and combinations** train your logic for systematic counting; and the **binomial theorem** is a direct application of combinations to algebraic expansions.

---

## Syllabus Mapping

| Syllabus Ref | Syllabus 2028–2030 (English) | Chinese Explanation | Section |
|:-------:|------|---------|:-------:|
| **11.1** | *Recognise the difference between permutations and combinations and know when each should be used.* | Recognise the difference between permutations and combinations and know when to use which | §1.2.4 |
| **11.2** | *Know and use the notation $n!$ and the expressions for permutations and combinations of $n$ items taken $r$ at a time. Includes $0! = 1$.* | Master the notation of $n!$, $^nP_r$, $^nC_r$ and their expressions | §1.2.2, §1.2.3 |
| **11.3** | *Solve problems on arrangement and selection using permutations or combinations. Problems will be either in an everyday context or based on an algebraic problem. Problems involving: repetition of objects; objects arranged in a circle; both permutations and combinations, are **not** included.* | Solve arrangement and selection problems using permutations or combinations (everyday or algebraic contexts). Does **not** include repetition, circular arrangements, or mixed permutation/combination. | §1.2.5 |
| **12.1** | *Use the binomial theorem for expansion of $(a+b)^n$ for positive integer $n$. Includes simplification of coefficients.* | Use the binomial theorem to expand $(a+b)^n$ ($n$ a positive integer), including simplification of coefficients | §1.3.1 |
| **12.2** | *Use the general term $\displaystyle\binom{n}{r}a^{n-r}b^r$, $0 \le r \le n$. For example: Find the term independent of $x$ in the expansion of $\left(x^2 + \frac{1}{x}\right)^{\!10}$. Knowledge of the greatest term and properties of the coefficients is **not** required.* | Use the general term formula to find specific terms (e.g., constant term). Greatest term and properties of coefficients are **not** required. | §1.3.2, §1.3.3 |
| **12.3** | *Recognise arithmetic and geometric progressions and understand the difference between them.* | Recognise arithmetic and geometric progressions and understand the differences between them | §1.1.4 |
| **12.4** | *Use the formulas for the $n$th term and for the sum of the first $n$ terms to solve problems involving arithmetic or geometric progressions. Problems may be in context.* | Use the $n$th term and sum of first $n$ terms formulas to solve arithmetic/geometric progression problems (may include real-world contexts) | §1.1.2, §1.1.3 |
| **12.5** | *Use the condition for the convergence of a geometric progression, and the formula for the sum to infinity of a convergent geometric progression. Includes explaining why a particular geometric progression has or does not have a sum to infinity.* | Use the convergence condition of a geometric progression and the sum to infinity formula, **including explaining why a given geometric series does or does not have a sum to infinity** | §1.1.3 |

---

## 1.1 Sequences (Arithmetic and Geometric)

A sequence is an ordered list of numbers. In Additional Mathematics, we focus on two fundamental types: **arithmetic sequences** (where the difference between consecutive terms is constant) and **geometric sequences** (where the ratio between consecutive terms is constant).

### 1.1.1 Summation Notation $\sum$

Before delving into sequences, we need to master summation notation $\sum$ (the Greek letter Sigma). It represents the sum of a series of numbers:

$$
\sum_{k=1}^{n} a_k = a_1 + a_2 + a_3 + \cdots + a_n
$$

The summation operation satisfies three basic rules:

**Rule 1 — Constant Factor Extraction**:

$$
\sum_{k=1}^{n} (c \cdot a_k) = c \cdot \sum_{k=1}^{n} a_k
$$

**Rule 2 — Splitting a Sum**:

$$
\sum_{k=1}^{n} (a_k \pm b_k) = \sum_{k=1}^{n} a_k \pm \sum_{k=1}^{n} b_k
$$

**Rule 3 — Sum of a Constant**:

$$
\sum_{k=1}^{n} c = n c
$$

**Example**: Evaluate $\displaystyle\sum_{k=1}^{5} (3k - 2)$.

$$
\sum_{k=1}^{5} (3k - 2) = 3\sum_{k=1}^{5} k - \sum_{k=1}^{5} 2 = 3 \times (1+2+3+4+5) - 5 \times 2 = 3 \times 15 - 10 = 45 - 10 = 35
$$

---

### 1.1.2 Arithmetic Progression (AP)

#### Definition

A sequence is called an **arithmetic progression** if, starting from the second term, the difference between each term and its preceding term is a **constant**. This constant is called the **common difference**, denoted by $d$:

$$
a_{n+1} - a_n = d \quad (\text{for all } n \ge 1)
$$

**Example**: $5, 9, 13, 17, 21$ is an arithmetic progression, with $d=4$, $a=5$.

#### Formula for the $n$th Term (Derivation)

Let the first term be $a_1 = a$. Then:

$$
\begin{aligned}
a_2 &= a + d \\
a_3 &= a_2 + d = a + 2d \\
a_4 &= a_3 + d = a + 3d
\end{aligned}
$$

The pattern: the $n$th term is obtained by adding the common difference $(n-1)$ times to the first term.

$$
\boxed{a_n = a + (n-1)d}
$$

**Verification**: For $n=1$, $a_1 = a$; for $n=2$, $a_2 = a + d$. Correct.

#### Formula for the Sum of the First $n$ Terms (Derivation — Reverse Addition Method)

$$
\begin{aligned}
S_n &= a + (a+d) + (a+2d) + \cdots + [a+(n-1)d] \\
S_n &= [a+(n-1)d] + [a+(n-2)d] + \cdots + a
\end{aligned}
$$

Adding the two equations, each pair sums to $2a + (n-1)d$, and there are $n$ pairs:

$$
2S_n = n[2a + (n-1)d]
$$

$$
\boxed{S_n = \frac{n}{2}[2a + (n-1)d]}
$$

If the last term $l = a_n = a + (n-1)d$, then:

$$
\boxed{S_n = \frac{n}{2}(a + l)}
$$

#### Examples

**Example 1**: First term $7$, common difference $3$, find the $15$th term.

$$
a_{15} = 7 + 14 \times 3 = 7 + 42 = 49
$$

---

**Example 2**: First term $2$, common difference $5$, sum of the first $n$ terms is $156$, find $n$.

$$
\frac{n}{2}[4 + (n-1) \times 5] = 156 \quad\Rightarrow\quad \frac{n}{2}(5n - 1) = 156
$$

$$
5n^2 - n - 312 = 0 \quad\Rightarrow\quad n = \frac{1 \pm \sqrt{1 + 6240}}{10} = \frac{1 \pm 79}{10}
$$

Since $n$ is a positive integer, $n = \frac{80}{10} = 8$.

---

**Example 3** (Real-world context): Deposit $500$ in the first year, then increase the deposit by $50$ each subsequent year. What is the total amount saved after $10$ years?

$$
S_{10} = \frac{10}{2}[2 \times 500 + 9 \times 50] = 5 \times (1000 + 450) = 7250
$$

Answer: $7250$ dollars.

---

### 1.1.3 Geometric Progression (GP)

#### Definition

A sequence is called a **geometric progression** if, starting from the second term, the ratio of each term to its preceding term is a **constant**. This constant is called the **common ratio**, denoted by $r$:

$$
\frac{a_{n+1}}{a_n} = r \quad (\text{for all } n \ge 1)
$$

**Example**: $2, 6, 18, 54, 162$ is a geometric progression, with $r=3$, $a=2$.

#### Formula for the $n$th Term

$$
\begin{aligned}
a_2 &= a r \\
a_3 &= a_2 \cdot r = a r^2 \\
a_4 &= a_3 \cdot r = a r^3
\end{aligned}
$$

$$
\boxed{a_n = a r^{\,n-1}}
$$

#### Formula for the Sum of the First $n$ Terms (Derivation — Subtraction Method)

$$
S_n = a + a r + a r^2 + \cdots + a r^{\,n-1}
$$

$$
r S_n = a r + a r^2 + a r^3 + \cdots + a r^{\,n}
$$

Subtracting:

$$
S_n - r S_n = a - a r^{\,n}
$$

$$
S_n(1 - r) = a(1 - r^{\,n})
$$

If $r = 1$: $S_n = n a$.

If $r \neq 1$:

$$
\boxed{S_n = a \cdot \frac{1 - r^{\,n}}{1 - r}} \quad \text{or equivalently} \quad \boxed{S_n = a \cdot \frac{r^{\,n} - 1}{r - 1}}
$$

#### Convergence Condition and Sum to Infinity of an Infinite Geometric Series (**Syllabus 12.5 Key Point**)

$$
S_\infty = \lim_{n \to \infty} S_n = \lim_{n \to \infty} a \cdot \frac{1 - r^{\,n}}{1 - r}
$$

The behaviour of $r^{\,n}$ as $n \to \infty$ determines whether the series converges:

| Range of $r$ | Behaviour of $r^{\,n}$ as $n \to \infty$ | Does the series converge? | Sum to Infinity |
|:-------------:|----------------------------------|:-----------:|:------:|
| $\|r\| < 1$ | $r^{\,n} \to 0$ | ✅ **Converges** | $\displaystyle S_\infty = \frac{a}{1-r}$ |
| $\|r\| > 1$ | $\|r^{\,n}\| \to \infty$ | ❌ **Diverges** | No finite sum |
| $r = 1$ | $r^{\,n} = 1$ (constant) | ❌ **Diverges** | $S_n = n a \to \infty$ |
| $r = -1$ | Oscillates between $1$ and $-1$ | ❌ **Diverges** | Sum is undefined |

Therefore, **the necessary and sufficient condition for a geometric series to converge is $|r| < 1$**.

In the exam, if asked to "explain why a particular geometric series has or does not have a sum to infinity," you should state: when $|r| < 1$, as $n \to \infty$, $r^{\,n} \to 0$, so $S_n \to \dfrac{a}{1-r}$; when $|r| \ge 1$, $r^{\,n}$ does not approach $0$, so $S_n$ does not approach a finite value.

#### Examples

**Example 1**: First term $3$, common ratio $2$, find the $6$th term.

$$
a_6 = 3 \times 2^5 = 3 \times 32 = 96
$$

---

**Example 2** (Convergence check + sum to infinity): $12 + 6 + 3 + \dfrac{3}{2} + \cdots$

First term $a = 12$, common ratio $r = \dfrac{6}{12} = \dfrac{1}{2}$.

Since $|r| = \dfrac{1}{2} < 1$, as $n \to \infty$, $\left(\dfrac{1}{2}\right)^{\!n} \to 0$, so the series converges.

$$
S_\infty = \frac{12}{1 - \frac{1}{2}} = \frac{12}{\frac{1}{2}} = 24
$$

---

**Example 3** (Given $S_\infty$ to find $r$): An infinite geometric series converges, its sum is $8$, and its first term is $4$. Find the common ratio $r$.

$$
8 = \frac{4}{1 - r} \quad\Rightarrow\quad 8(1 - r) = 4 \quad\Rightarrow\quad 1 - r = \frac{1}{2} \quad\Rightarrow\quad r = \frac{1}{2}
$$

Verification: $|r| = \dfrac{1}{2} < 1$, satisfying the convergence condition.

---

### 1.1.4 Comparison: Arithmetic vs Geometric Progressions (**Syllabus 12.3 Key Point**)

| Feature | Arithmetic Progression (AP) | Geometric Progression (GP) |
|:----|:-------------|:-------------|
| **Defining Property** | $a_{n+1} - a_n = d$ (constant difference) | $\dfrac{a_{n+1}}{a_n} = r$ (constant ratio) |
| **How to check** | Subtract consecutive terms, check if constant | Divide consecutive terms, check if constant |
| **$n$th term** | $a_n = a + (n-1)d$ | $a_n = a r^{\,n-1}$ |
| **Sum of first $n$ terms** | $S_n = \dfrac{n}{2}[2a + (n-1)d]$ | $S_n = a\dfrac{1-r^n}{1-r}$ ($r \neq 1$) |
| **Growth pattern** | **Linear growth** (add constant each time) | **Exponential growth/decay** (multiply by constant each time) |
| **Sum to infinity** | Does not exist (except constant sequence with $d=0$) | Converges to $\dfrac{a}{1-r}$ when $|r| < 1$ |

**Practice identifying**:

1. $5, 8, 11, 14, 17, \ldots$ → constant difference of $3$ → **AP** ✓
2. $5, 10, 20, 40, 80, \ldots$ → constant ratio of $2$ → **GP** ✓
3. $1, 4, 9, 16, 25, \ldots$ → differences are $3,5,7,9$ (not constant), ratios are $4, 2.25, 1.78,\ldots$ (not constant) → **Neither** ✗
4. $100, 50, 25, 12.5, \ldots$ → constant ratio of $\dfrac{1}{2}$ → **GP** (convergent) ✓

---

## 1.2 Permutations and Combinations

Permutations and combinations answer the same fundamental question: "How many different ways are there?" The key difference lies in **whether order matters**.

### 1.2.1 Multiplication Principle

If a task can be broken down into $k$ sequential steps, and the $i$th step has $m_i$ ways to be performed, then the total number of ways is:

$$
\boxed{m_1 \times m_2 \times \cdots \times m_k}
$$

**Example**: There are $3$ routes from A to B, and $4$ routes from B to C. The number of routes from A to B to C is $3 \times 4 = 12$.

### 1.2.2 Permutations — Order Matters

**Definition**: Selecting $r$ objects ($r \le n$) from $n$ distinct objects and arranging them in a specific order. Different orders count as different permutations. Denoted by $^nP_r$ or $P(n,r)$.

**Derivation**:

$$
^nP_r = n(n-1)(n-2)\cdots(n-r+1)
$$

Expressed using factorials:

$$
\boxed{^nP_r = \frac{n!}{(n-r)!}}
$$

**Special values**: $^nP_n = n!$, $^nP_0 = 1$, $0! = 1$.

### 1.2.3 Combinations — Order Does Not Matter

**Definition**: Selecting $r$ objects ($r \le n$) from $n$ distinct objects without considering the order. Denoted by $^nC_r$, $C(n,r)$, or $\binom{n}{r}$.

**Derivation**: Number of permutations divided by the number of internal arrangements:

$$
\boxed{^nC_r = \binom{n}{r} = \frac{^nP_r}{r!} = \frac{n!}{r!\,(n-r)!}}
$$

**Properties**:

- Symmetry: $\displaystyle\binom{n}{r} = \binom{n}{n-r}$
- Boundary values: $\displaystyle\binom{n}{0} = \binom{n}{n} = 1$, $\displaystyle\binom{n}{1} = \binom{n}{n-1} = n$

### 1.2.4 How to Choose? (**Syllabus 11.1 Key Point**)

Ask yourself: **If I swap any two selected elements, does the result change?**

| Scenario | Does order matter? | Use | Example |
|:----|:---------:|:----|:-----|
| Queuing, rankings, passwords, rankings | ✅ Yes | **Permutation** $^nP_r$ | Choose 3 out of 6 people to stand in a row |
| Committees, subject selection, lottery draws, team formation | ❌ No | **Combination** $^nC_r$ | Choose 3 out of 6 people to form a committee |

### 1.2.5 Worked Examples

**Example 1** (Permutation — everyday context): From 6 different books, choose 4 to arrange on a shelf (left to right). How many arrangements?

$$
^6P_4 = \frac{6!}{(6-4)!} = \frac{6!}{2!} = 6 \times 5 \times 4 \times 3 = 360
$$

Answer: $360$ ways.

---

**Example 2** (Combination — everyday context): From 7 men and 5 women, select a committee of 4 that must include at least 2 women. How many ways?

- $2$ women $2$ men: $\displaystyle\binom{5}{2} \times \binom{7}{2} = 10 \times 21 = 210$
- $3$ women $1$ man: $\displaystyle\binom{5}{3} \times \binom{7}{1} = 10 \times 7 = 70$
- $4$ women $0$ men: $\displaystyle\binom{5}{4} \times \binom{7}{0} = 5 \times 1 = 5$

Total: $210 + 70 + 5 = 285$.

> **Verification by complement**: Total $\displaystyle\binom{12}{4}=495$, subtract "at most 1 woman" ($0$ women $4$ men $= \binom{5}{0}\binom{7}{4}=35$, $1$ woman $3$ men $= \binom{5}{1}\binom{7}{3}=5\times35=175$, total $210$), $495 - 210 = 285$ ✓

---

**Example 3** (Algebraic context — combinatorial identity): Prove that $\displaystyle\binom{n}{r} + \binom{n}{r-1} = \binom{n+1}{r}$, and use this to compute $\displaystyle\binom{8}{3} + \binom{8}{2}$.

**Proof**:

$$
\begin{aligned}
\binom{n}{r} + \binom{n}{r-1}
&= \frac{n!}{r!(n-r)!} + \frac{n!}{(r-1)!(n-r+1)!} \\[4pt]
&= \frac{n!}{r!(n-r+1)!}\Big[(n-r+1) + r\Big] \\[4pt]
&= \frac{n! \cdot (n+1)}{r!(n-r+1)!}
= \frac{(n+1)!}{r!(n+1-r)!}
= \binom{n+1}{r}
\end{aligned}
$$

**Application**:

$$
\binom{8}{3} + \binom{8}{2} = \binom{9}{3} = \frac{9 \times 8 \times 7}{3 \times 2 \times 1} = 84
$$

### 1.2.6 ⚠️ Topics NOT Examined

According to the syllabus, the following types **will not appear**:

| Not Examined | English Original |
|---------|---------|
| ❌ Permutations with repetition of objects | *repetition of objects* |
| ❌ Circular arrangements | *objects arranged in a circle* |
| ❌ Mixed use of permutations and combinations in the same problem | *both permutations and combinations* |

In the exam, each problem is either purely about permutations or purely about combinations.

---

## 1.3 Binomial Theorem

### 1.3.1 Binomial Expansion (**Syllabus 12.1**)

$(a+b)^n$ can be thought of as multiplying $n$ copies of $(a+b)$. When expanding, each term is the product of choosing either $a$ or $b$ from each factor. To obtain $a^{\,n-r}b^{\,r}$, we need to choose $b$ from $r$ factors and $a$ from the remaining $n-r$ factors. The number of ways to make this choice is $\binom{n}{r}$.

Summing over $r = 0, 1, \ldots, n$:

$$
\boxed{(a+b)^n = \sum_{r=0}^{n} \binom{n}{r} a^{\,n-r} b^{\,r}}
$$

**Example**: Expand $(x+3)^4$.

$$
\begin{aligned}
(x+3)^4 &= \binom{4}{0}x^4(3)^0 + \binom{4}{1}x^3(3)^1 + \binom{4}{2}x^2(3)^2 + \binom{4}{3}x^1(3)^3 + \binom{4}{4}x^0(3)^4 \\
&= 1 \cdot x^4 + 4 \cdot 3x^3 + 6 \cdot 9x^2 + 4 \cdot 27x + 1 \cdot 81 \\
&= x^4 + 12x^3 + 54x^2 + 108x + 81
\end{aligned}
$$

Note that each coefficient has been **simplified** (e.g., $4 \times 3 = 12$, $6 \times 9 = 54$), as explicitly required by the syllabus.

### 1.3.2 General Term and Specific Terms (**Syllabus 12.2**)

The $(r+1)$th term in the expansion (counting from $r=0$):

$$
\boxed{T_{r+1} = \binom{n}{r} a^{\,n-r} b^{\,r}}
$$

Common question types:

| Type | Method |
|:----|:----|
| Find the coefficient of $x^k$ | Set the exponent of $x$ in the general term $= k$, solve for $r$ |
| Find the constant term (independent of $x$) | Set the exponent of $x$ $= 0$, solve for $r$ |
| Find the coefficient of $x^p y^q$ | Match the exponents of $x$ and $y$ respectively |

> **⚠️ Important distinction**:
> - **Binomial coefficient** = $\binom{n}{r}$ (depends only on $n$ and $r$)
> - **Full coefficient** = $\binom{n}{r}$ × constant factors and signs from $a$ and $b$
>
> For example, in $(2x-3)^5$, for $r=2$: binomial coefficient $\binom{5}{2}=10$, full coefficient $= 10 \cdot (2)^3 \cdot (-3)^2 = 720$

### 1.3.3 Worked Examples

**Example 1** (Finding the coefficient of a specified power): Find the coefficient of $x$ in the expansion of $\left(2x + \dfrac{1}{x}\right)^7$.

**Solution**:

$$
T_{r+1} = \binom{7}{r} (2x)^{7-r} \left(\frac{1}{x}\right)^{\!r}
= \binom{7}{r} 2^{7-r} x^{7-r} \cdot x^{-r}
= \binom{7}{r} 2^{7-r} x^{7-2r}
$$

Set $7-2r = 1$, giving $r = 3$.

$$
T_4 = \binom{7}{3} 2^{4} x = 35 \times 16 \times x = 560x
$$

Therefore, the coefficient of $x$ is $560$.

---

**Example 2** (Finding the constant term — typical syllabus question): Find the constant term in the expansion of $\left(x^2 - \dfrac{2}{x}\right)^6$.

**Solution**:

$$
\begin{aligned}
T_{r+1} &= \binom{6}{r} (x^2)^{6-r} \left(-\frac{2}{x}\right)^{\!r} \\
&= \binom{6}{r} (-2)^r x^{12-2r} \cdot x^{-r} \\
&= \binom{6}{r} (-2)^r x^{12-3r}
\end{aligned}
$$

Set $12 - 3r = 0$, giving $r = 4$.

$$
T_5 = \binom{6}{4} (-2)^4 = 15 \times 16 = 240
$$

Thus the constant term is $240$.

---

**Example 3** (Coefficient in the product of two binomials): Find the coefficient of $x^2$ in the expansion of $(1+x)^5 (2-x)^4$.

**Solution**:

$(1+x)^5$ general term: $\displaystyle\binom{5}{r} x^r$
$(2-x)^4$ general term: $\displaystyle\binom{4}{k} 2^{4-k} (-1)^k x^k$

We need $r + k = 2$:

| $r$ | $k$ | Calculation | Contribution |
|:--:|:--:|:----|:----:|
| $0$ | $2$ | $\binom{5}{0} \cdot \binom{4}{2} 2^{2} (-1)^2 = 1 \times 6 \times 4 \times 1$ | $24$ |
| $1$ | $1$ | $\binom{5}{1} \cdot \binom{4}{1} 2^{3} (-1)^1 = 5 \times 4 \times 8 \times (-1)$ | $-160$ |
| $2$ | $0$ | $\binom{5}{2} \cdot \binom{4}{0} 2^{4} (-1)^0 = 10 \times 1 \times 16 \times 1$ | $160$ |

Sum: $24 + (-160) + 160 = 24$.

Answer: The coefficient of $x^2$ is $24$.

---

### 1.3.4 Properties of Binomial Coefficients (Pascal's Triangle)

**Symmetry**:

$$
\boxed{\binom{n}{r} = \binom{n}{n-r}}
$$

**Pascal's Rule** (Recurrence relation):

$$
\boxed{\binom{n}{r} + \binom{n}{r-1} = \binom{n+1}{r}}
$$

**Pascal's Triangle**:

```
n=0:        1
n=1:       1 1
n=2:      1 2 1
n=3:     1 3 3 1
n=4:    1 4 6 4 1
n=5:   1 5 10 10 5 1
```

> **Exam tip**: For $n \le 5$, you can write coefficients directly using Pascal's Triangle; for $n \ge 6$, use the combination formula $\binom{n}{r}$.

> **Not examined** (syllabus explicitly states): Greatest term and properties of coefficients are **not** required.

---

## Chapter Formula Reference Table

| Topic | Formula | Conditions |
|:----|:----|:----|
| AP $n$th term | $a_n = a + (n-1)d$ | — |
| AP sum of first $n$ terms | $S_n = \dfrac{n}{2}[2a + (n-1)d]$ | — |
| GP $n$th term | $a_n = a r^{\,n-1}$ | — |
| GP sum of first $n$ terms | $S_n = a\dfrac{1-r^n}{1-r}$ | $r \neq 1$ |
| GP sum to infinity | $S_\infty = \dfrac{a}{1-r}$ | $\|r\| < 1$ |
| Permutations | $^nP_r = \dfrac{n!}{(n-r)!}$ | Order matters |
| Combinations | $\displaystyle\binom{n}{r} = \dfrac{n!}{r!(n-r)!}$ | Order does not matter |
| Binomial theorem | $(a+b)^n = \displaystyle\sum_{r=0}^{n}\binom{n}{r}a^{n-r}b^{r}$ | $n \in \mathbb{Z}^+$ |
| General term | $T_{r+1} = \displaystyle\binom{n}{r}a^{n-r}b^{r}$ | For finding specific terms |

---
---
# Chapter 2: Vectors and Rates of Change

## Syllabus Mapping

This chapter covers the following sections of the Cambridge IGCSE Additional Mathematics (0606) 2028–2030 syllabus:

| Syllabus Ref | Content | Description |
|---------|------|------|
| **13.1** | Understand and use vector notation | Column vectors, $\mathbf{i}$-$\mathbf{j}$ form, $\overrightarrow{AB}$, $p$等形式 |
| **13.2** | Position vectors and unit vectors | Find unit vectors $\hat{\mathbf{a}} = \frac{\mathbf{a}}{|\mathbf{a}|}$ |
| **13.3** | Magnitude, addition, subtraction and scalar multiplication of vectors | Including equal vectors, vector geometry problems (given diagrams) |
| **13.4** | Composition and resolution of velocities | Find resultant vectors, use velocity vectors to find position, collision problems |
| **14.1** | The idea of the derivative (introduction to rates of change) | Intuitive understanding of limits; differentiation from first principles is not required |

---

## Introduction

In the real world, many quantities have not only magnitude but also direction. From correcting for wind speed when flying an aeroplane, to determining whether two ships at sea might collide, to analysing the trajectory of a projectile — the mathematical language for all these problems is **vectors**.

This chapter builds a complete knowledge system for two-dimensional vectors from the ground up. We first learn the basic representation of vectors and rules of operation (including how to determine perpendicular vectors). Then we apply these tools to geometry problems and kinematics problems (composition of velocities, collision detection). Finally, we shift perspective from "static vectors" to "dynamic rates of change" — when a position vector changes over time, its rate of change is velocity, and the rate of change of velocity is acceleration. Conversely, given acceleration, we can find velocity and position through integration. This idea directly leads to differentiation in Chapter 5 and integration in Chapter 7.

---

## 2.1 Fundamentals of Two-Dimensional Vectors

### 2.1.1 What is a Vector?

A **vector** is a quantity that has both **magnitude** and **direction**. In contrast, a **scalar** has only magnitude, not direction. For example:

- **Vectors**: displacement, velocity, force
- **Scalars**: distance, speed, mass, temperature

In a two-dimensional plane, vectors can be represented in several equivalent ways.

#### Representation 1: Column Vector

$$
\mathbf{v} = \begin{pmatrix} x \\ y \end{pmatrix}
$$

where $x$ is the horizontal component and $y$ is the vertical component. This representation is very convenient for solving systems of equations, as we can operate directly on the components.

#### Representation 2: $\mathbf{i}$-$\mathbf{j}$ Form

Define two fundamental unit vectors:

$$
\mathbf{i} = \begin{pmatrix} 1 \\ 0 \end{pmatrix}, \quad \mathbf{j} = \begin{pmatrix} 0 \\ 1 \end{pmatrix}
$$

$\mathbf{i}$ points in the positive $x$-axis direction (to the right), and $\mathbf{j}$ points in the positive $y$-axis direction (upwards). Then any vector can be written as:

$$
\mathbf{v} = x\mathbf{i} + y\mathbf{j}
$$

**Equivalence of the two representations**:

$$
x\mathbf{i} + y\mathbf{j} = \begin{pmatrix} x \\ y \end{pmatrix}
$$

For example, the vector $3\mathbf{i} - 2\mathbf{j}$ is the same vector as the column vector $\begin{pmatrix} 3 \\ -2 \end{pmatrix}$.

#### Representation 3: Directed Line Segment

The vector from point $A$ to point $B$ is denoted by $\overrightarrow{AB}$. It equals the position of the endpoint minus the position of the starting point:

$$
\overrightarrow{AB} = \mathbf{r}_B - \mathbf{r}_A
$$

> **Why "endpoint minus starting point"?** Suppose you want to walk from home $A$ to school $B$. Your displacement (from $A$ to $B$) is your final position (the school's position) minus your starting position (home's position). If $A$ is at $(1,1)$ and $B$ is at $(4,5)$, then you need to go 3 units right and 4 units up, i.e., $\overrightarrow{AB} = (3,4)$.

---

### 2.1.2 Position Vectors

Let $O$ be the origin. The **position vector** of any point $P(x, y)$ is:

$$
\mathbf{r} = \overrightarrow{OP} = \begin{pmatrix} x \\ y \end{pmatrix} = x\mathbf{i} + y\mathbf{j}
$$

The position vector tells us where point $P$ is located relative to the origin. The key distinction here is: a **point** $P(x, y)$ is a location in space, while the **vector** $\mathbf{r} = (x, y)$ is a directed line segment from the origin to that point — it contains the information of displacement.

> **Difference between a point and a vector**: A point is a location, like a coordinate on a map. A vector is a displacement, like "3 steps right, 2 steps up." The same vector can start from any point, but the same point can only be at one location.

---

### 2.1.3 Magnitude of a Vector

The magnitude (or length, or size) of the vector $\mathbf{v} = x\mathbf{i} + y\mathbf{j}$ is given by the Pythagorean theorem:

$$
|\mathbf{v}| = \sqrt{x^2 + y^2}
$$

The magnitude is always a non-negative real number. It is zero if and only if the vector is the zero vector $\mathbf{0} = \begin{pmatrix} 0 \\ 0 \end{pmatrix}$.

> **Why $\sqrt{x^2 + y^2}$?** Consider the vector $\mathbf{v}$ as the line segment from the origin $(0,0)$ to the point $(x,y)$. This segment is the hypotenuse of a right-angled triangle whose legs have lengths $|x|$ and $|y|$. By the Pythagorean theorem, the length of the hypotenuse $= \sqrt{x^2 + y^2}$.

---

### 2.1.4 Unit Vectors

A **unit vector** is a vector with magnitude 1. Given any non-zero vector $\mathbf{v}$, we can construct a unit vector $\hat{\mathbf{v}}$ in the same direction:

$$
\hat{\mathbf{v}} = \frac{\mathbf{v}}{|\mathbf{v}|}
$$

That is, we divide the original vector by its own magnitude. This operation is called **normalisation**.

> **Why is this defined this way?** Let $\hat{\mathbf{v}} = \frac{\mathbf{v}}{|\mathbf{v}|}$. Then
> $$
> |\hat{\mathbf{v}}| = \frac{|\mathbf{v}|}{|\mathbf{v}|} = 1
> $$
> The direction remains unchanged because we are dividing the original vector by a positive scalar.
>
> **Analogy**: It's like cutting a rope into unit-length pieces. If you have a 5-metre rope and cut it into 5 equal pieces, each piece is 1 metre long, with the same direction as the original.

---

### 2.1.5 Vector Addition and Subtraction

To add two vectors, we add their corresponding components separately:

$$
\begin{pmatrix} x_1 \\ y_1 \end{pmatrix} + \begin{pmatrix} x_2 \\ y_2 \end{pmatrix} = \begin{pmatrix} x_1 + x_2 \\ y_1 + y_2 \end{pmatrix}
$$

Subtraction is similar:

$$
\begin{pmatrix} x_1 \\ y_1 \end{pmatrix} - \begin{pmatrix} x_2 \\ y_2 \end{pmatrix} = \begin{pmatrix} x_1 - x_2 \\ y_1 - y_2 \end{pmatrix}
$$

**Geometric meaning — Why the "parallelogram rule"?**

Imagine two people pulling a box at the same time. One person pulls with force $\mathbf{a}$ eastwards, and the other pulls with force $\mathbf{b}$ northwards. The resultant force actually experienced by the box is $\mathbf{a} + \mathbf{b}$.

- **Addition — Parallelogram Rule**: Using the two vectors as adjacent sides, construct a parallelogram. The diagonal starting from the common origin is their sum.
- **Subtraction — Triangle Rule**: $\mathbf{a} - \mathbf{b}$ is the vector from the tip of $\mathbf{b}$ to the tip of $\mathbf{a}$.

**Useful mnemonics**:
- For displacement vectors: **endpoint minus starting point**. The vector from $A$ to $B$ is $\overrightarrow{AB} = \mathbf{r}_B - \mathbf{r}_A$
- For addition: connect head to tail, from the first start to the last end

---

### 2.1.6 Scalar Multiplication

Multiplying a vector by a scalar $c$ is equivalent to multiplying each component by $c$:

$$
c \begin{pmatrix} x \\ y \end{pmatrix} = \begin{pmatrix} cx \\ cy \end{pmatrix}
$$

Geometric effect of scalar multiplication:
- If $c > 0$, the vector is stretched ($c > 1$) or compressed ($0 < c < 1$) along its original direction
- If $c < 0$, the vector reverses direction

Magnitude after scalar multiplication:

$$
|c\mathbf{v}| = |c| \cdot |\mathbf{v}|
$$

> **Why does the magnitude multiply by $|c|$ instead of $c$?** Because if $c = -2$, the length of the vector becomes 2 times the original, and the direction reverses. Length is always positive, so we take $|c| = 2$.

---

### 2.1.7 Equal Vectors

Two vectors are equal if and only if their corresponding components are equal respectively. That is:

$$
\begin{pmatrix} x_1 \\ y_1 \end{pmatrix} = \begin{pmatrix} x_2 \\ y_2 \end{pmatrix} \iff x_1 = x_2 \quad \text{and} \quad y_1 = y_2
$$

This is called the **principle of equating like vectors** — it is the core tool for solving vector equations.

> **Why is this principle so useful?** A single vector equation actually contains two independent scalar equations (one for the $x$-component, one for the $y$-component). This allows us to solve for unknowns from two directions separately.

---

### 2.1.8 Perpendicular Vectors (Orthogonal Vectors)

#### What is Perpendicular?

Two non-zero vectors $\mathbf{u}$ and $\mathbf{v}$ are perpendicular (or orthogonal) if and only if the angle between them is $90^\circ$.

#### How to Determine Perpendicularity? — The Dot Product

The **dot product (inner product)** of two vectors is defined as:

$$
\mathbf{u} \cdot \mathbf{v} = u_x v_x + u_y v_y
$$

The dot product yields a **scalar** (not a vector), hence it is also called the "scalar product."

**Condition for perpendicularity**:

$$
\mathbf{u} \perp \mathbf{v} \iff \mathbf{u} \cdot \mathbf{v} = 0
$$

> **Why does a zero dot product imply perpendicularity?**
>
> From a geometric perspective, the dot product has an alternative equivalent definition:
> $$
> \mathbf{u} \cdot \mathbf{v} = |\mathbf{u}| |\mathbf{v}| \cos\theta
> $$
> where $\theta$ is the angle between the two vectors.
>
> Derivation of this equivalence: using the Law of Cosines. Let the angle between $\mathbf{u}$ and $\mathbf{v}$ be $\theta$. Then the magnitude of $\mathbf{u} - \mathbf{v}$ satisfies:
> $$
> |\mathbf{u} - \mathbf{v}|^2 = |\mathbf{u}|^2 + |\mathbf{v}|^2 - 2|\mathbf{u}||\mathbf{v}|\cos\theta
> $$
> Meanwhile, expanding the left side:
> $$
> |\mathbf{u} - \mathbf{v}|^2 = (u_x - v_x)^2 + (u_y - v_y)^2 = (u_x^2 + u_y^2) + (v_x^2 + v_y^2) - 2(u_x v_x + u_y v_y)
> $$
> Comparing the two expressions, we get:
> $$
> |\mathbf{u}|^2 + |\mathbf{v}|^2 - 2|\mathbf{u}||\mathbf{v}|\cos\theta = |\mathbf{u}|^2 + |\mathbf{v}|^2 - 2(u_x v_x + u_y v_y)
> $$
> Therefore $u_x v_x + u_y v_y = |\mathbf{u}||\mathbf{v}|\cos\theta$.
>
> When $\theta = 90^\circ$, $\cos 90^\circ = 0$, so the dot product is zero.

#### Horizontal and Vertical Vectors

A special case: a **horizontal vector** has zero $y$-component, i.e., $\mathbf{h} = (h_x, 0)$ ($h_x \neq 0$), and its direction is parallel to the $x$-axis. A **vertical vector** has zero $x$-component, i.e., $\mathbf{v} = (0, v_y)$ ($v_y \neq 0$), and its direction is parallel to the $y$-axis.

A horizontal vector is always perpendicular to a vertical vector. Verification using the dot product:

$$
(h_x, 0) \cdot (0, v_y) = h_x \cdot 0 + 0 \cdot v_y = 0
$$

#### Determining Perpendicularity Using Slope

If two non-zero vectors are not parallel to the axes (i.e., neither $x$ nor $y$ components are zero), we can also use slopes to determine perpendicularity. Let the slope of vector $\mathbf{u}$ be $k_1 = \frac{u_y}{u_x}$ and the slope of vector $\mathbf{v}$ be $k_2 = \frac{v_y}{v_x}$. Then:

$$
\mathbf{u} \perp \mathbf{v} \iff k_1 \cdot k_2 = -1
$$

> **Derivation**: From the condition for a zero dot product:
> $$
> u_x v_x + u_y v_y = 0 \implies u_x v_x = -u_y v_y \implies \frac{u_y}{u_x} \cdot \frac{v_y}{v_x} = -1
> $$
> i.e., $k_1 \cdot k_2 = -1$.

> **Note on the zero vector**: The zero vector $\mathbf{0} = (0, 0)$ has no fixed direction. By convention, in technical discussions it is considered to be both parallel and perpendicular to all vectors, but in practical problem-solving we generally exclude it.

---

### 📌 Worked Examples 2.1: Basic Vector Operations

**Example 1** (Vector representation, magnitude, and unit vector)

Given two points $A(1, 2)$ and $B(5, -1)$.

(a) Find the vector $\overrightarrow{AB}$ in $\mathbf{i}$-$\mathbf{j}$ form.
(b) Find $|\overrightarrow{AB}|$.
(c) Find the unit vector in the same direction as $\overrightarrow{AB}$.

**Solution approach**:
- The vector from $A$ to $B$ = position of $B$ minus position of $A$
- Magnitude = square root of the sum of squares of the components
- Unit vector = original vector divided by its magnitude

**Solution**:

(a)
$$
\overrightarrow{AB} = \mathbf{r}_B - \mathbf{r}_A = (5\mathbf{i} - \mathbf{j}) - (\mathbf{i} + 2\mathbf{j}) = (5-1)\mathbf{i} + (-1-2)\mathbf{j} = 4\mathbf{i} - 3\mathbf{j}
$$

(b)
$$
|\overrightarrow{AB}| = \sqrt{4^2 + (-3)^2} = \sqrt{16 + 9} = \sqrt{25} = 5
$$

(c) The unit vector in the same direction is:

$$
\hat{\mathbf{v}} = \frac{4\mathbf{i} - 3\mathbf{j}}{5} = \frac{4}{5}\mathbf{i} - \frac{3}{5}\mathbf{j}
$$

Verification of magnitude: $\sqrt{(4/5)^2 + (-3/5)^2} = \sqrt{16/25 + 9/25} = \sqrt{25/25} = 1$. ✓

---

**Example 2** (Vector addition, scalar multiplication, and equal vectors — solving systems of equations)

Given $\mathbf{a} = 2\mathbf{i} + 3\mathbf{j}$, $\mathbf{b} = -\mathbf{i} + 2\mathbf{j}$. Find:

(a) $\mathbf{a} + \mathbf{b}$
(b) $2\mathbf{a} - 3\mathbf{b}$
(c) Real numbers $p$ and $q$ such that $p\mathbf{a} + q\mathbf{b} = 7\mathbf{i} + 8\mathbf{j}$

**Solution approach**:
- Addition and scalar multiplication operate on components separately
- For part (c), first expand the left side, then use the principle of equating like vectors (coefficients of $\mathbf{i}$ and $\mathbf{j}$ must be equal respectively) to set up a system of equations

**Solution**:

(a)
$$
\mathbf{a} + \mathbf{b} = (2\mathbf{i} + 3\mathbf{j}) + (-\mathbf{i} + 2\mathbf{j}) = (2-1)\mathbf{i} + (3+2)\mathbf{j} = \mathbf{i} + 5\mathbf{j}
$$

(b)
$$
2\mathbf{a} - 3\mathbf{b} = 2(2\mathbf{i} + 3\mathbf{j}) - 3(-\mathbf{i} + 2\mathbf{j}) = (4\mathbf{i} + 6\mathbf{j}) + (3\mathbf{i} - 6\mathbf{j}) = 7\mathbf{i} + 0\mathbf{j} = 7\mathbf{i}
$$

(c) Let $p\mathbf{a} + q\mathbf{b} = 7\mathbf{i} + 8\mathbf{j}$, i.e.:

$$
p(2\mathbf{i} + 3\mathbf{j}) + q(-\mathbf{i} + 2\mathbf{j}) = 7\mathbf{i} + 8\mathbf{j}
$$

First expand the brackets:

$$
2p\mathbf{i} + 3p\mathbf{j} - q\mathbf{i} + 2q\mathbf{j} = 7\mathbf{i} + 8\mathbf{j}
$$

Combine the coefficients of $\mathbf{i}$ and $\mathbf{j}$:

$$
(2p - q)\mathbf{i} + (3p + 2q)\mathbf{j} = 7\mathbf{i} + 8\mathbf{j}
$$

Using the principle of equating like vectors, the coefficients of $\mathbf{i}$ must be equal, and the coefficients of $\mathbf{j}$ must be equal:

$$
\begin{cases}
2p - q = 7 \quad \text{(① equate }\mathbf{i}\text{ coefficients)} \\[4pt]
3p + 2q = 8 \quad \text{(② equate }\mathbf{j}\text{ coefficients)}
\end{cases}
$$

Solve this system. From ①, $q = 2p - 7$. Substituting into ②:

$$
3p + 2(2p - 7) = 8 \implies 3p + 4p - 14 = 8 \implies 7p = 22 \implies p = \frac{22}{7}
$$

Then $q = 2 \times \frac{22}{7} - 7 = \frac{44}{7} - \frac{49}{7} = -\frac{5}{7}$.

Therefore $p = \frac{22}{7}$, $q = -\frac{5}{7}$. ✓

---

**Example 3** (Position vectors, displacement, and determining perpendicular vectors)

Three points $P$, $Q$, $R$ have position vectors $\mathbf{p} = 3\mathbf{i} + \mathbf{j}$, $\mathbf{q} = 5\mathbf{i} - 2\mathbf{j}$, $\mathbf{r} = -2\mathbf{i} + 4\mathbf{j}$ respectively.

(a) Find $\overrightarrow{PQ}$ and $\overrightarrow{PR}$.
(b) Given $\overrightarrow{PS} = 2\overrightarrow{PQ}$, find the position vector of $S$.
(c) Determine whether $\overrightarrow{PQ}$ is perpendicular to $\overrightarrow{PR}$.

**Solution approach**:
- $\overrightarrow{PQ} = \mathbf{q} - \mathbf{p}$ (endpoint minus starting point)
- $\overrightarrow{PS} = \mathbf{s} - \mathbf{p}$, substitute the given condition to solve for $\mathbf{s}$
- Perpendicularity check: compute the dot product; if zero, they are perpendicular

**Solution**:

(a)
$$
\overrightarrow{PQ} = \mathbf{q} - \mathbf{p} = (5\mathbf{i} - 2\mathbf{j}) - (3\mathbf{i} + \mathbf{j}) = 2\mathbf{i} - 3\mathbf{j}
$$

$$
\overrightarrow{PR} = \mathbf{r} - \mathbf{p} = (-2\mathbf{i} + 4\mathbf{j}) - (3\mathbf{i} + \mathbf{j}) = -5\mathbf{i} + 3\mathbf{j}
$$

(b) Let the position vector of $S$ be $\mathbf{s}$. Since $\overrightarrow{PS} = \mathbf{s} - \mathbf{p}$ and $\overrightarrow{PS} = 2\overrightarrow{PQ}$:

$$
\mathbf{s} - \mathbf{p} = 2(2\mathbf{i} - 3\mathbf{j}) = 4\mathbf{i} - 6\mathbf{j}
$$

Therefore:

$$
\mathbf{s} = \mathbf{p} + (4\mathbf{i} - 6\mathbf{j}) = (3\mathbf{i} + \mathbf{j}) + (4\mathbf{i} - 6\mathbf{j}) = 7\mathbf{i} - 5\mathbf{j}
$$

So $S$ has coordinates $(7, -5)$.

(c) Compute the dot product:

$$
\overrightarrow{PQ} \cdot \overrightarrow{PR} = (2)(-5) + (-3)(3) = -10 - 9 = -19 \neq 0
$$

Since the dot product is non-zero, $\overrightarrow{PQ}$ and $\overrightarrow{PR}$ are **not perpendicular**.

> **Verification using the slope method**:
> $k_{PQ} = \dfrac{-3}{2} = -1.5$
> $k_{PR} = \dfrac{3}{-5} = -0.6$
> $k_{PQ} \cdot k_{PR} = (-1.5)(-0.6) = 0.9 \neq -1$
> This also shows they are not perpendicular. ✓

---

## 2.2 Practical Applications of Vectors

### 2.2.1 Vector Geometry — In-Depth Analysis

Vectors are a powerful tool for solving plane geometry problems. By converting geometric relationships into vector equations, we can use algebraic methods to obtain precise solutions, avoiding the imprecision of drawing diagrams.

#### Core Idea

**The essence of vector geometry**: using vector operations (addition, subtraction, scalar multiplication) to represent geometric relationships.

| Geometric Relationship | Vector Expression |
|:---|:---|
| Line segment from $A$ to $B$ | $\overrightarrow{AB} = \mathbf{r}_B - \mathbf{r}_A$ |
| Midpoint $M$ of $A$ and $B$ | $\mathbf{r}_M = \dfrac{\mathbf{r}_A + \mathbf{r}_B}{2}$ |
| $P$ divides $AB$ in the ratio $m:n$ | $\mathbf{r}_P = \dfrac{n\mathbf{r}_A + m\mathbf{r}_B}{m+n}$ |
| $AB \parallel CD$ | $\overrightarrow{AB} = k \cdot \overrightarrow{CD}$ |
| $AB \perp CD$ | $\overrightarrow{AB} \cdot \overrightarrow{CD} = 0$ |
| $A,B,C$ are collinear | $\overrightarrow{AB} = k \cdot \overrightarrow{BC}$ (there exists $k$) |

#### Midpoint Formula — Why Does It Work?

Let $M$ be the midpoint of $AB$. The displacement from $A$ to $M$ is half of $\overrightarrow{AB}$:

$$
\mathbf{r}_M = \mathbf{r}_A + \frac{1}{2}\overrightarrow{AB} = \mathbf{r}_A + \frac{1}{2}(\mathbf{r}_B - \mathbf{r}_A) = \frac{2\mathbf{r}_A + \mathbf{r}_B - \mathbf{r}_A}{2} = \frac{\mathbf{r}_A + \mathbf{r}_B}{2}
$$

#### Section Formula — Detailed Derivation

Let point $P$ divide segment $AB$ in the ratio $AP:PB = m:n$ (i.e., from $A$ towards $B$, $AP$ occupies $m$ parts and $PB$ occupies $n$ parts).

This means $P$ is located at $\dfrac{m}{m+n}$ of the way from $A$ to $B$ (counting from $A$). Therefore:

$$
\begin{aligned}
\mathbf{r}_P &= \mathbf{r}_A + \frac{m}{m+n}\overrightarrow{AB} \\
&= \mathbf{r}_A + \frac{m}{m+n}(\mathbf{r}_B - \mathbf{r}_A) \\
&= \frac{(m+n)\mathbf{r}_A + m\mathbf{r}_B - m\mathbf{r}_A}{m+n} \\
&= \frac{n\mathbf{r}_A + m\mathbf{r}_B}{m+n}
\end{aligned}
$$

> **Memory tip**: In the section formula, the coefficient of $A$ is $n$ (the ratio on the opposite side), and the coefficient of $B$ is $m$ (the ratio on the opposite side). Cross-multiply!
>
> For example, if $AP:PB = 2:3$ ($m=2, n=3$), then:
> $$ \mathbf{r}_P = \frac{3\mathbf{r}_A + 2\mathbf{r}_B}{5} $$
> The coefficient of $A$ is $3$ (the opposite side $PB$ is $3$ parts), and the coefficient of $B$ is $2$ (the opposite side $AP$ is $2$ parts).

#### Parallel Vectors

Two non-zero vectors $\mathbf{a}$ and $\mathbf{b}$ are parallel (i.e., have the same or opposite direction) if and only if there exists a real number $k$ such that:

$$
\mathbf{a} = k\mathbf{b}
$$

That is, one vector is a scalar multiple of the other.

> **How to check for parallelism?** Check if the corresponding components of the two vectors are proportional:
> If $\mathbf{a} = (a_x, a_y)$ and $\mathbf{b} = (b_x, b_y)$, and $\frac{a_x}{b_x} = \frac{a_y}{b_y}$ (denominator non-zero), then they are parallel.
> Note that this ratio can be negative (indicating opposite directions).

#### Testing for Collinearity of Three Points

Three points $A$, $B$, $C$ are collinear if and only if $\overrightarrow{AB}$ is parallel to $\overrightarrow{AC}$ (or $\overrightarrow{AB}$ is parallel to $\overrightarrow{BC}$).

**Why?** If three points are collinear, then the displacements from $A$ to $B$ and from $A$ to $C$ are in the same or opposite direction, i.e., there exists a scalar $k$ such that $\overrightarrow{AC} = k \cdot \overrightarrow{AB}$.

---

### 📌 Worked Examples 2.2: Vector Geometry Applications

**Example 1** (Parallelogram and Midpoint — illustrated)

In parallelogram $ABCD$, the position vectors of $A$, $B$, $C$ are $\mathbf{a} = \mathbf{i} + 2\mathbf{j}$, $\mathbf{b} = 4\mathbf{i} + 3\mathbf{j}$, $\mathbf{c} = 6\mathbf{i} + \mathbf{j}$ respectively. Find:

(a) The position vector of $D$
(b) The position vector of $M$, the intersection point of the diagonals $AC$ and $BD$

**Solution approach**:

> First understand the structure of the parallelogram. The vertices are arranged in order $A \to B \to C \to D \to A$.
>
> **Key property of a parallelogram**: Opposite sides are parallel and equal.
> - $AB \parallel DC$ and $AB = DC$
> - $AD \parallel BC$ and $AD = BC$
>
> This means $\overrightarrow{AD} = \overrightarrow{BC}$ or $\overrightarrow{AB} = \overrightarrow{DC}$.
>
> Additionally, the diagonals of a parallelogram **bisect each other**, i.e., the midpoint of $AC$ = the midpoint of $BD$.

**Solution**:

(a) In parallelogram $ABCD$, opposite sides $AD$ and $BC$ are parallel and equal, so $\overrightarrow{AD} = \overrightarrow{BC}$.

First find $\overrightarrow{BC} = \mathbf{c} - \mathbf{b}$:

$$
\overrightarrow{BC} = (6\mathbf{i} + \mathbf{j}) - (4\mathbf{i} + 3\mathbf{j}) = 2\mathbf{i} - 2\mathbf{j}
$$

Since $\overrightarrow{AD} = \overrightarrow{BC} = 2\mathbf{i} - 2\mathbf{j}$, and $\overrightarrow{AD} = \mathbf{d} - \mathbf{a}$:

$$
\mathbf{d} = \mathbf{a} + \overrightarrow{AD} = (\mathbf{i} + 2\mathbf{j}) + (2\mathbf{i} - 2\mathbf{j}) = 3\mathbf{i}
$$

So $D$ has coordinates $(3, 0)$.

**Verification**: We can also use $\overrightarrow{AB} = \overrightarrow{DC}$.
$\overrightarrow{AB} = \mathbf{b} - \mathbf{a} = (4\mathbf{i} + 3\mathbf{j}) - (\mathbf{i} + 2\mathbf{j}) = 3\mathbf{i} + \mathbf{j}$
$\overrightarrow{DC} = \mathbf{c} - \mathbf{d}$, so $\mathbf{c} - \mathbf{d} = 3\mathbf{i} + \mathbf{j}$, giving $\mathbf{d} = \mathbf{c} - (3\mathbf{i} + \mathbf{j}) = (6\mathbf{i} + \mathbf{j}) - (3\mathbf{i} + \mathbf{j}) = 3\mathbf{i}$, consistent. ✓

(b) The diagonals of a parallelogram bisect each other. Therefore $M$ is both the midpoint of $AC$ and the midpoint of $BD$.

Using the midpoint of $AC$:

$$
\mathbf{m} = \frac{\mathbf{a} + \mathbf{c}}{2} = \frac{(\mathbf{i} + 2\mathbf{j}) + (6\mathbf{i} + \mathbf{j})}{2} = \frac{7\mathbf{i} + 3\mathbf{j}}{2} = 3.5\mathbf{i} + 1.5\mathbf{j}
$$

Verification using the midpoint of $BD$: $\frac{\mathbf{b} + \mathbf{d}}{2} = \frac{(4\mathbf{i} + 3\mathbf{j}) + 3\mathbf{i}}{2} = \frac{7\mathbf{i} + 3\mathbf{j}}{2}$, consistent. ✓

---

**Example 2** (Collinearity test and ratio — how to prove three points are collinear)

Three points $A$, $B$, $C$ have position vectors $\mathbf{a} = 2\mathbf{i} + \mathbf{j}$, $\mathbf{b} = 5\mathbf{i} + 4\mathbf{j}$, $\mathbf{c} = 8\mathbf{i} + 7\mathbf{j}$ respectively.

(a) Prove that $A$, $B$, $C$ are collinear.
(b) Find the ratio $AB:BC$.

**Solution approach**:

> Standard method for proving three points are collinear:
> 1. Compute $\overrightarrow{AB}$ and $\overrightarrow{BC}$ (or $\overrightarrow{AB}$ and $\overrightarrow{AC}$)
> 2. Determine whether they are parallel (i.e., whether there exists a scalar $k$ such that one equals the other multiplied by $k$)
> 3. If they are parallel and share a common point ($B$ is the common point of $\overrightarrow{AB}$ and $\overrightarrow{BC}$), then the three points are collinear

**Solution**:

(a) Compute the vectors:

$$
\overrightarrow{AB} = \mathbf{b} - \mathbf{a} = (5\mathbf{i} + 4\mathbf{j}) - (2\mathbf{i} + \mathbf{j}) = 3\mathbf{i} + 3\mathbf{j}
$$

$$
\overrightarrow{BC} = \mathbf{c} - \mathbf{b} = (8\mathbf{i} + 7\mathbf{j}) - (5\mathbf{i} + 4\mathbf{j}) = 3\mathbf{i} + 3\mathbf{j}
$$

Observe that $\overrightarrow{BC} = \overrightarrow{AB}$, i.e., $\overrightarrow{BC} = 1 \cdot \overrightarrow{AB}$. There exists a scalar $k = 1$ such that $\overrightarrow{BC} = k\overrightarrow{AB}$, so $\overrightarrow{AB} \parallel \overrightarrow{BC}$. Since both vectors pass through point $B$, $A$, $B$, $C$ are collinear.

> **Note**: We can also verify the relationship between $\overrightarrow{AC}$ and $\overrightarrow{AB}$.
> $\overrightarrow{AC} = \mathbf{c} - \mathbf{a} = (8\mathbf{i} + 7\mathbf{j}) - (2\mathbf{i} + \mathbf{j}) = 6\mathbf{i} + 6\mathbf{j} = 2(3\mathbf{i} + 3\mathbf{j}) = 2\overrightarrow{AB}$
> This also leads to the same conclusion of collinearity.

(b) Since $\overrightarrow{BC} = \overrightarrow{AB}$ and they have the same direction, $\overrightarrow{AB}$ and $\overrightarrow{BC}$ have equal lengths. That is, $AB = BC$, therefore $AB:BC = 1:1$.

In other words, $B$ is the midpoint of segment $AC$.

---

**Example 3** (Section formula + perpendicularity check — comprehensive application)

In $\triangle OAB$, $C$ lies on $OA$ such that $OC:CA = 2:1$, and $D$ lies on $AB$ such that $AD:DB = 3:1$. Let $\overrightarrow{OA} = \mathbf{a}$, $\overrightarrow{OB} = \mathbf{b}$.

(a) Express $\overrightarrow{OD}$ in terms of $\mathbf{a}$ and $\mathbf{b}$.
(b) Express $\overrightarrow{CD}$ in terms of $\mathbf{a}$ and $\mathbf{b}$.
(c) Given that $\mathbf{a} = 3\mathbf{i} + 2\mathbf{j}$ and $\mathbf{b} = \mathbf{i} + 6\mathbf{j}$, determine whether $\overrightarrow{OC}$ is perpendicular to $\overrightarrow{OD}$.

**Solution approach**:

> This is a classic "express vectors in terms of a basis" problem. $\mathbf{a}$ and $\mathbf{b}$ are the basis vectors; all other vectors must be expressed in terms of them.
>
> Key steps:
> 1. Determine the position of point $C$ on $OA$: $OC:CA = 2:1$ means $OC = \frac{2}{3}OA$
> 2. Determine the position of point $D$ on $AB$: $AD:DB = 3:1$ means $AD = \frac{3}{4}AB$
> 3. Use the section formula or direct addition/subtraction to express the vectors
> 4. Perpendicularity check: substitute the numerical values and compute the dot product

**Solution**:

(a) First, express the position of $D$.

Method 1 (Section formula): $D$ divides $AB$ in the ratio $AD:DB = 3:1$, i.e., from $A$ towards $B$, $D$ is located at $\frac{3}{4}$ of the way.

Using the section formula ($m=3, n=1$):

$$
\mathbf{r}_D = \frac{n\mathbf{r}_A + m\mathbf{r}_B}{m+n} = \frac{1 \cdot \mathbf{a} + 3 \cdot \mathbf{b}}{3+1} = \frac{\mathbf{a} + 3\mathbf{b}}{4}
$$

Method 2 (Direct approach): Starting from $A$, go $\frac{3}{4}$ of the way to $B$.

$$
\overrightarrow{OD} = \overrightarrow{OA} + \frac{3}{4}\overrightarrow{AB}
$$

And $\overrightarrow{AB} = \overrightarrow{OB} - \overrightarrow{OA} = \mathbf{b} - \mathbf{a}$, so:

$$
\overrightarrow{OD} = \mathbf{a} + \frac{3}{4}(\mathbf{b} - \mathbf{a}) = \mathbf{a} + \frac{3}{4}\mathbf{b} - \frac{3}{4}\mathbf{a} = \frac{1}{4}\mathbf{a} + \frac{3}{4}\mathbf{b}
$$

Note that $\frac{\mathbf{a} + 3\mathbf{b}}{4} = \frac{1}{4}\mathbf{a} + \frac{3}{4}\mathbf{b}$, both methods give the same result. ✓

(b) $C$ lies on $OA$ with $OC:CA = 2:1$, so $C$ divides $\overrightarrow{OA}$ in the ratio $2:1$ (counting from $O$). Therefore:

$$
\overrightarrow{OC} = \frac{2}{3}\overrightarrow{OA} = \frac{2}{3}\mathbf{a}
$$

Then:

$$
\overrightarrow{CD} = \overrightarrow{OD} - \overrightarrow{OC} = \left(\frac{1}{4}\mathbf{a} + \frac{3}{4}\mathbf{b}\right) - \frac{2}{3}\mathbf{a}
$$

Compute the coefficient of $\mathbf{a}$ by finding a common denominator: $\frac{1}{4} - \frac{2}{3} = \frac{3}{12} - \frac{8}{12} = -\frac{5}{12}$.

So:

$$
\overrightarrow{CD} = -\frac{5}{12}\mathbf{a} + \frac{3}{4}\mathbf{b}
$$

(c) Substitute $\mathbf{a} = 3\mathbf{i} + 2\mathbf{j}$, $\mathbf{b} = \mathbf{i} + 6\mathbf{j}$:

First find $\overrightarrow{OC}$:

$$
\overrightarrow{OC} = \frac{2}{3}(3\mathbf{i} + 2\mathbf{j}) = 2\mathbf{i} + \frac{4}{3}\mathbf{j}
$$

Then find $\overrightarrow{OD}$:

$$
\begin{aligned}
\overrightarrow{OD} &= \frac{1}{4}(3\mathbf{i} + 2\mathbf{j}) + \frac{3}{4}(\mathbf{i} + 6\mathbf{j}) \\
&= \left(\frac{3}{4} + \frac{3}{4}\right)\mathbf{i} + \left(\frac{1}{2} + \frac{9}{2}\right)\mathbf{j} \\
&= \frac{6}{4}\mathbf{i} + \frac{10}{2}\mathbf{j} \\
&= \frac{3}{2}\mathbf{i} + 5\mathbf{j}
\end{aligned}
$$

Compute the dot product:

$$
\overrightarrow{OC} \cdot \overrightarrow{OD} = \left(2\right)\left(\frac{3}{2}\right) + \left(\frac{4}{3}\right)(5) = 3 + \frac{20}{3} = \frac{9}{3} + \frac{20}{3} = \frac{29}{3} \neq 0
$$

The dot product is non-zero, so $\overrightarrow{OC}$ and $\overrightarrow{OD}$ are **not perpendicular**.

---

### 2.2.2 Composition and Resolution of Velocities

Velocity is a vector quantity. When an object is simultaneously involved in two or more motions, its resultant velocity is the vector sum of these velocities.

#### Relative Velocity Formula

Let the velocity of object $A$ relative to reference frame $C$ be $\mathbf{v}_{A/C}$, the velocity of object $A$ relative to object $B$ be $\mathbf{v}_{A/B}$, and the velocity of object $B$ relative to reference frame $C$ be $\mathbf{v}_{B/C}$. Then:

$$
\mathbf{v}_{A/C} = \mathbf{v}_{A/B} + \mathbf{v}_{B/C}
$$

> **Intuitive understanding**:
> - You are walking on a train at speed $\mathbf{v}_{A/B}$ (you relative to the train)
> - The train is moving relative to the ground at speed $\mathbf{v}_{B/C}$ (train relative to ground)
> - Your speed relative to the ground $\mathbf{v}_{A/C}$ is the sum of the two
>
> **Another example**: A boat travelling in a river.
> - The boat's speed in still water = $\mathbf{v}_{B/W}$ (boat relative to water)
> - The speed of the river current = $\mathbf{v}_{W/G}$ (water relative to ground)
> - The boat's actual speed relative to the ground = $\mathbf{v}_{B/W} + \mathbf{v}_{W/G}$

#### Resolution of Velocities

The opposite of composition: breaking a velocity vector into two perpendicular components (usually horizontal and vertical directions) is called **resolution of velocities**.

Let the magnitude of velocity $\mathbf{v}$ be $v$ (speed), and let the angle it makes with the horizontal be $\theta$. Then:

$$
\mathbf{v} = (v\cos\theta)\mathbf{i} + (v\sin\theta)\mathbf{j}
$$

where $v_x = v\cos\theta$ is the horizontal component and $v_y = v\sin\theta$ is the vertical component.

> **Derivation**: Project the velocity vector onto the $x$-axis and $y$-axis. In the right-angled triangle, the adjacent side $=$ hypotenuse $\times \cos\theta$, and the opposite side $=$ hypotenuse $\times \sin\theta$.

---

#### Collision Problems

The condition for two moving objects to collide is that at the **same time**, their position vectors are **equal**. That is:

$$
\mathbf{r}_1(t) = \mathbf{r}_2(t)
$$

For motion with constant velocity, the position vector satisfies:

$$
\mathbf{r}(t) = \mathbf{r}_0 + \mathbf{v}t
$$

where $\mathbf{r}_0$ is the initial position vector and $\mathbf{v}$ is the velocity vector. Therefore, the collision condition can be expanded to:

$$
\mathbf{r}_{01} + \mathbf{v}_1 t = \mathbf{r}_{02} + \mathbf{v}_2 t
$$

This is a vector equation in time $t$. It is equivalent to two scalar equations (one for each component) being equal, allowing us to solve for $t$ and verify consistency.

**Solution steps**:
1. Write the position vectors $\mathbf{r}_1(t)$ and $\mathbf{r}_2(t)$ for both objects.
2. Set $\mathbf{r}_1(t) = \mathbf{r}_2(t)$, obtaining two component equations.
3. Solve for $t$ from each equation. If the two $t$ values are equal and $t \geq 0$, they collide; otherwise, they do not.

> **Note**: "Collision" requires both objects to be at the same position at the same time. If two ships reach the same point at different times, that is called "meeting" rather than "colliding".

---

### 📌 Worked Examples 2.3: Composition of Velocities and Collision Problems

**Example 1** (Composition of velocities — boat and current)

A boat's speed in still water is $6\,\text{m/s}$ eastwards. The water current flows at $4\,\text{m/s}$ northwards. Find the magnitude and direction of the boat's velocity relative to the ground.

**Solution approach**:
- Boat's velocity relative to water $\mathbf{v}_{B/W}$ = east $6$ m/s
- Water's velocity relative to ground $\mathbf{v}_{W/G}$ = north $4$ m/s
- Boat's velocity relative to ground $\mathbf{v}_{B/G} = \mathbf{v}_{B/W} + \mathbf{v}_{W/G}$

**Solution**:

Let due east be the $+x$-axis and due north be the $+y$-axis.

Boat's velocity relative to water: $\mathbf{v}_{B/W} = 6\mathbf{i}$
Water current velocity relative to ground: $\mathbf{v}_{W/G} = 4\mathbf{j}$

By the velocity composition formula:

$$
\mathbf{v}_{B/G} = \mathbf{v}_{B/W} + \mathbf{v}_{W/G} = 6\mathbf{i} + 4\mathbf{j}
$$

Magnitude of the resultant velocity (speed):

$$
|\mathbf{v}_{B/G}| = \sqrt{6^2 + 4^2} = \sqrt{36 + 16} = \sqrt{52} = 2\sqrt{13} \approx 7.21\,\text{m/s}
$$

Direction of the resultant velocity: Let $\theta$ be the angle measured from due east (anticlockwise positive).

$$
\tan\theta = \frac{4}{6} = \frac{2}{3} \implies \theta = \arctan\left(\frac{2}{3}\right) \approx 33.69^\circ
$$

Therefore, the boat's velocity relative to the ground has magnitude $2\sqrt{13}\,\text{m/s}$, and direction $33.69^\circ$ north of east (i.e., rotated $33.69^\circ$ anticlockwise from due east).

> **Real-life example**: This is why, when a boat crosses a river, if it heads directly toward the opposite bank, it will be carried downstream by the current. To reach the point directly opposite, the boat must point its bow upstream at an angle.

---

**Example 2** (Resolution of velocity — initial velocity of a projectile)

A ball is thrown with an initial speed of $20\,\text{m/s}$ at an angle of $30^\circ$ above the horizontal.

(a) Find the horizontal and vertical components of the initial velocity.
(b) Write the initial velocity in vector form.

**Solution approach**:
- The magnitude of the velocity is $20$, and the direction is at an elevation of $30^\circ$
- Horizontal component $v_x = v\cos\theta$, vertical component $v_y = v\sin\theta$

**Solution**:

(a) Let the horizontal rightward direction be $+x$-axis and the vertical upward direction be $+y$-axis.

Horizontal component:

$$
v_x = v\cos\theta = 20 \times \cos 30^\circ = 20 \times \frac{\sqrt{3}}{2} = 10\sqrt{3} \approx 17.32\,\text{m/s}
$$

Vertical component:

$$
v_y = v\sin\theta = 20 \times \sin 30^\circ = 20 \times \frac{1}{2} = 10\,\text{m/s}
$$

(b) The initial velocity in vector form:

$$
\mathbf{v}_0 = 10\sqrt{3}\,\mathbf{i} + 10\,\mathbf{j}\,\text{m/s}
$$

> **Physical significance**:
> - In the absence of air resistance, the horizontal component $v_x$ remains constant throughout the motion (since no force acts horizontally)
> - The vertical component $v_y$ changes due to gravity at an acceleration of $-g$ ($g \approx 9.8\,\text{m/s}^2$)
> - Therefore, the velocity at any time $t$ is $\mathbf{v}(t) = 10\sqrt{3}\,\mathbf{i} + (10 - gt)\,\mathbf{j}$
> - This lays the foundation for kinematics problems in Chapter 10

---

**Example 3** (Collision problem — will two ships collide?)

Ship $P$ departs from point $(0, 0)$ travelling at velocity $\mathbf{v}_P = (3\mathbf{i} + 4\mathbf{j})\,\text{km/h}$. Ship $Q$ departs from point $(10, 5)\,\text{km}$ travelling at velocity $\mathbf{v}_Q = (-2\mathbf{i} + \mathbf{j})\,\text{km/h}$. Both ships depart at the same time. Determine whether they will collide.

**Solution approach**:
1. Write the position vectors of both ships (both in the form $\mathbf{r}_0 + \mathbf{v}t$)
2. Set $\mathbf{r}_P(t) = \mathbf{r}_Q(t)$
3. Obtain two component equations and solve for $t$ from each
4. If the $t$ values are consistent and $t \geq 0$, they collide; otherwise, they do not

**Solution**:

Let $t$ be the time (in hours) after departure.

$P$'s position vector (starting from the origin):

$$
\mathbf{r}_P(t) = \begin{pmatrix} 0 \\ 0 \end{pmatrix} + \begin{pmatrix} 3 \\ 4 \end{pmatrix} t = \begin{pmatrix} 3t \\ 4t \end{pmatrix}
$$

$Q$'s position vector (starting from $(10,5)$):

$$
\mathbf{r}_Q(t) = \begin{pmatrix} 10 \\ 5 \end{pmatrix} + \begin{pmatrix} -2 \\ 1 \end{pmatrix} t = \begin{pmatrix} 10 - 2t \\ 5 + t \end{pmatrix}
$$

If the two ships collide, there must exist some $t \geq 0$ such that $\mathbf{r}_P(t) = \mathbf{r}_Q(t)$, i.e.:

$$
\begin{pmatrix} 3t \\ 4t \end{pmatrix} = \begin{pmatrix} 10 - 2t \\ 5 + t \end{pmatrix}
$$

This gives two component equations:

$$
\begin{cases}
x\text{-component: } & 3t = 10 - 2t \implies 5t = 10 \implies t = 2 \\[4pt]
y\text{-component: } & 4t = 5 + t \implies 3t = 5 \implies t = \dfrac{5}{3}
\end{cases}
$$

The two $t$ values are not equal ($2 \neq \frac{5}{3}$), so there is no time that satisfies both component equations simultaneously. The two ships will not collide.

> **Why don't they collide?** Even though the $x$-coordinates are equal at $t=2$, the $y$-coordinates at $t=2$ are $4\times 2 = 8$ and $5+2=7$ respectively, which are not equal. So the two ships never arrive at the same point at the same time.

---

## 2.3 Introduction to Rates of Change (Calculus Foundation)

### 2.3.1 Why Study Rates of Change?

In the physical world, very few things remain static. A moving car — its position changes. An inflating balloon — its volume changes. A heated metal rod — its temperature changes. A **rate of change** is the mathematical tool that describes "how quickly one quantity changes with respect to another."

In sections 2.1 and 2.2, we used vectors to describe position, velocity, and acceleration. Now we ask a deeper question: **How do we precisely define "instantaneous" rate of change?**

---

### 2.3.2 From Average Rate of Change to Instantaneous Rate of Change

Let's start with a concrete kinematics example.

A particle moves along a straight line. Its displacement $s$ (in metres) as a function of time $t$ (in seconds) is:

$$
s(t) = t^2
$$

We want to find the velocity at the **instant** $t = 1$ second.

#### Step 1: Average Velocity

If we take a time interval $[1, 1 + \Delta t]$, the average velocity of the particle over this interval is:

$$
\text{Average velocity} = \frac{s(1 + \Delta t) - s(1)}{\Delta t}
$$

Substituting $s(t) = t^2$:

$$
\frac{(1 + \Delta t)^2 - 1^2}{\Delta t} = \frac{1 + 2\Delta t + (\Delta t)^2 - 1}{\Delta t} = \frac{2\Delta t + (\Delta t)^2}{\Delta t} = 2 + \Delta t
$$

#### Step 2: Let $\Delta t$ Become Smaller and Smaller

We let $\Delta t$ gradually approach 0 and observe how the average velocity changes:

| $\Delta t$ (seconds) | Average Velocity (m/s) |
|:---:|:---:|
| 0.1 | $2 + 0.1 = 2.1$ |
| 0.01 | $2 + 0.01 = 2.01$ |
| 0.001 | $2 + 0.001 = 2.001$ |
| 0.0001 | $2 + 0.0001 = 2.0001$ |
| $\to 0$ | $\to 2$ |

As $\Delta t$ gets closer and closer to 0, the average velocity gets closer and closer to **2**.

#### Step 3: The Limit

When $\Delta t$ approaches 0, the average velocity $2 + \Delta t$ approaches 2. We write:

$$
v(1) = \lim_{\Delta t \to 0} \frac{s(1 + \Delta t) - s(1)}{\Delta t} = \lim_{\Delta t \to 0} (2 + \Delta t) = 2
$$

This limiting value is the **instantaneous velocity** of the particle at $t = 1$.

> **Important understanding**: We never set $\Delta t = 0$ (that would give $0/0$, which is meaningless). We let $\Delta t$ approach 0 infinitely closely and observe what fixed value the ratio approaches. This "target of approach" is the derivative.
>
> In the language of limits: **As $\Delta t$ approaches 0, the limit of the average velocity is the instantaneous velocity.**

---

### 2.3.3 General Definition of the Derivative

In general, for a function $y = f(x)$, its **derivative** (i.e., instantaneous rate of change) at $x = a$ is defined as:

$$
f'(a) = \lim_{h \to 0} \frac{f(a + h) - f(a)}{h}
$$

where $h$ corresponds to $\Delta x$ or $\Delta t$ in the earlier example.

If this limit exists, we say that $f$ is **differentiable** at $x = a$.

**Notation for derivatives**:
- Leibniz notation: $\dfrac{dy}{dx}$ or $\dfrac{d}{dx}f(x)$
- Lagrange notation: $f'(x)$
- Newton notation (commonly used in physics): $\dot{y}$

> In syllabus point 14.1, only an intuitive understanding of limits is required; differentiation from first principles is not required. However, we will still present a few basic derivations here to help build your intuition.

---

### 2.3.4 Derivatives from First Principles — Basic Derivations

Let's use the limit definition to derive the derivatives of some basic functions.

#### Derivation 1: $f(x) = x^2$

$$
\begin{aligned}
f'(x) &= \lim_{h \to 0} \frac{(x + h)^2 - x^2}{h} \\
&= \lim_{h \to 0} \frac{x^2 + 2xh + h^2 - x^2}{h} \\
&= \lim_{h \to 0} \frac{2xh + h^2}{h} \\
&= \lim_{h \to 0} (2x + h) \\
&= 2x
\end{aligned}
$$

Therefore $\dfrac{d}{dx}(x^2) = 2x$.

**Geometric meaning**: The slope of the tangent line to the function $y = x^2$ at any point $x$ is $2x$. At $x = 1$, the slope is $2$; at $x = 3$, the slope is $6$.

#### Derivation 2: $f(x) = x^3$

$$
\begin{aligned}
f'(x) &= \lim_{h \to 0} \frac{(x + h)^3 - x^3}{h}
\end{aligned}
$$

Expanding $(x + h)^3 = x^3 + 3x^2h + 3xh^2 + h^3$:

$$
\begin{aligned}
f'(x) &= \lim_{h \to 0} \frac{x^3 + 3x^2h + 3xh^2 + h^3 - x^3}{h} \\
&= \lim_{h \to 0} \frac{3x^2h + 3xh^2 + h^3}{h} \\
&= \lim_{h \to 0} (3x^2 + 3xh + h^2) \\
&= 3x^2
\end{aligned}
$$

Therefore $\dfrac{d}{dx}(x^3) = 3x^2$.

#### Derivation 3: $f(x) = \dfrac{1}{x}$ ($x \neq 0$)

$$
\begin{aligned}
f'(x) &= \lim_{h \to 0} \frac{\frac{1}{x + h} - \frac{1}{x}}{h}
\end{aligned}
$$

First, combine the fractions in the numerator:

$$
\frac{1}{x + h} - \frac{1}{x} = \frac{x - (x + h)}{x(x + h)} = \frac{-h}{x(x + h)}
$$

Therefore:

$$
\begin{aligned}
f'(x) &= \lim_{h \to 0} \frac{-h}{x(x + h)} \cdot \frac{1}{h} \\
&= \lim_{h \to 0} \frac{-1}{x(x + h)} \\
&= -\frac{1}{x^2}
\end{aligned}
$$

Thus $\dfrac{d}{dx}\left(\dfrac{1}{x}\right) = -\dfrac{1}{x^2}$.

---

### 2.3.5 The Power Rule

From the derivations above, we can observe a pattern:

| $f(x)$ | $f'(x)$ |
|:---:|:---:|
| $x^2$ | $2x$ |
| $x^3$ | $3x^2$ |
| $x^1$ | $1$ (i.e., $1 \cdot x^0$) |
| $\dfrac{1}{x} = x^{-1}$ | $-\dfrac{1}{x^2} = -x^{-2}$ |

This pattern is the **Power Rule**: for any real number $n$,

$$
\boxed{\frac{d}{dx}(x^n) = n x^{n-1}}
$$

> **Full derivation of the Power Rule** (using the Binomial Theorem, for positive integers $n$ only):
>
> Consider $f(x) = x^n$, where $n$ is a positive integer. Expand $(x + h)^n$ using the Binomial Theorem:
> $$
> (x + h)^n = x^n + n x^{n-1}h + \binom{n}{2}x^{n-2}h^2 + \binom{n}{3}x^{n-3}h^3 + \dots + h^n
> $$
> Therefore:
> $$
> \begin{aligned}
> f'(x) &= \lim_{h \to 0} \frac{x^n + n x^{n-1}h + \binom{n}{2}x^{n-2}h^2 + \dots + h^n - x^n}{h} \\
> &= \lim_{h \to 0} \left( n x^{n-1} + \binom{n}{2}x^{n-2}h + \binom{n}{3}x^{n-3}h^2 + \dots + h^{n-1} \right) \\
> &= n x^{n-1}
> \end{aligned}
> $$
> because all terms containing $h$ tend to 0 as $h \to 0$.

---

### 2.3.6 Rates of Change in the Context of Vectors: Kinematics

Now let's return to the context of vectors. If a particle's position vector $\mathbf{r}(t)$ changes with time, then its velocity vector and acceleration vector are the rates of change of the position vector with respect to time.

Let $\mathbf{r}(t) = x(t)\mathbf{i} + y(t)\mathbf{j}$. Then:

$$
\mathbf{v}(t) = \frac{d\mathbf{r}}{dt} = \frac{dx}{dt}\mathbf{i} + \frac{dy}{dt}\mathbf{j}
$$

$$
\mathbf{a}(t) = \frac{d\mathbf{v}}{dt} = \frac{d^2\mathbf{r}}{dt^2} = \frac{d^2x}{dt^2}\mathbf{i} + \frac{d^2y}{dt^2}\mathbf{j}
$$

That is, differentiating a vector function means differentiating each of its components separately.

---

### 2.3.7 From Acceleration to Velocity and Position (Integration Foundation)

In physics, acceleration $\mathbf{a}(t)$ is the rate of change of velocity $\mathbf{v}(t)$. If we know the acceleration and want to recover the velocity, we need to perform the inverse operation of differentiation — this is called **integration** (which will be studied in detail in Chapter 7).

The basic relationships are:

- Velocity $\mathbf{v}(t) = \int \mathbf{a}(t) \, dt + \mathbf{v}_0$ (where $\mathbf{v}_0$ is the initial velocity)
- Position $\mathbf{r}(t) = \int \mathbf{v}(t) \, dt + \mathbf{r}_0$ (where $\mathbf{r}_0$ is the initial position)

Or, using definite integrals (more suitable for problems with specific time intervals):

$$
\mathbf{v}(t) = \mathbf{v}_0 + \int_0^t \mathbf{a}(u) \, du,
\quad
\mathbf{r}(t) = \mathbf{r}_0 + \int_0^t \mathbf{v}(u) \, du
$$

The intuition to establish here is: **Differentiation** finds the rate of change (position → velocity → acceleration), while **Integration** finds the accumulated quantity (acceleration → velocity → position). They are inverse operations of each other.

---

### 📌 Worked Examples 2.4: Introduction to Rates of Change

**Example 1** (Using the limit definition to find instantaneous velocity)

A particle's displacement (in metres) as a function of time (in seconds) is $s(t) = 3t^2 - 2t + 1$.

(a) Find the average velocity from $t = 2$ to $t = 2 + h$.
(b) Use the limit to find the instantaneous velocity at $t = 2$.

**Solution approach**:
- Average velocity = $\dfrac{s(2+h) - s(2)}{h}$
- Instantaneous velocity = $\displaystyle\lim_{h \to 0}$ (average velocity)

**Solution**:

(a)
$$
\begin{aligned}
\text{Average velocity} &= \frac{s(2 + h) - s(2)}{h} \\
&= \frac{[3(2+h)^2 - 2(2+h) + 1] - [3(4) - 4 + 1]}{h} \\
&= \frac{[3(4 + 4h + h^2) - 4 - 2h + 1] - [12 - 4 + 1]}{h} \\
&= \frac{[12 + 12h + 3h^2 - 4 - 2h + 1] - 9}{h} \\
&= \frac{[9 + 10h + 3h^2] - 9}{h} \\
&= \frac{10h + 3h^2}{h} = 10 + 3h
\end{aligned}
$$

(b) The instantaneous velocity is the limit of the average velocity as $h \to 0$:

$$
v(2) = \lim_{h \to 0} (10 + 3h) = 10\,\text{m/s}
$$

Therefore, the particle's instantaneous velocity at $t = 2$ seconds is $10\,\text{m/s}$.

> **Verification**: Using the Power Rule to differentiate directly: $s'(t) = 6t - 2$, $s'(2) = 12 - 2 = 10$, consistent. ✓

---

**Example 2** (Using the limit definition to find a general derivative + verification by the Power Rule)

Use the limit definition of the derivative to find $f'(x)$ for $f(x) = 4x - x^2$.

**Solution**:

$$
\begin{aligned}
f'(x) &= \lim_{h \to 0} \frac{f(x + h) - f(x)}{h} \\
&= \lim_{h \to 0} \frac{[4(x + h) - (x + h)^2] - [4x - x^2]}{h} \\
&= \lim_{h \to 0} \frac{4x + 4h - (x^2 + 2xh + h^2) - 4x + x^2}{h} \\
&= \lim_{h \to 0} \frac{4h - 2xh - h^2}{h} \\
&= \lim_{h \to 0} (4 - 2x - h) \\
&= 4 - 2x
\end{aligned}
$$

Therefore $f'(x) = 4 - 2x$.

**Verification**: Using the Power Rule to differentiate $f(x) = 4x - x^2$ term by term:
- $\dfrac{d}{dx}(4x) = 4 \cdot 1 \cdot x^{0} = 4$
- $\dfrac{d}{dx}(-x^2) = -2x^{1} = -2x$
- Adding gives $f'(x) = 4 - 2x$, consistent with the result from the limit. ✓

---

**Example 3** (Rates of change of vectors + integration as the inverse operation)

A particle moves in a plane. Its position vector is:

$$
\mathbf{r}(t) = (t^3 - 3t)\mathbf{i} + (t^2 - 2t)\mathbf{j}
$$

where $t$ is in seconds and position is in metres.

(a) Find the velocity vector $\mathbf{v}(t)$.
(b) Find the acceleration vector $\mathbf{a}(t)$.
(c) Find the velocity and acceleration vectors at $t = 2$ seconds.
(d) Given that the particle's acceleration is $\mathbf{a}(t) = 6t\mathbf{i} + 2\mathbf{j}$, initial velocity $\mathbf{v}_0 = -3\mathbf{i} - 2\mathbf{j}$, and initial position $\mathbf{r}_0 = \mathbf{0}$, use integration to find $\mathbf{v}(t)$ and $\mathbf{r}(t)$, and verify they are consistent with parts (a) and (b).

**Solution approach**:
- Velocity = derivative of position (differentiate each component separately)
- Acceleration = derivative of velocity (differentiate each component separately)
- Integration is the inverse of differentiation: given acceleration, integrate once to get velocity (add constant), then integrate again to get position (add constant)
- Constants are determined by the initial conditions

**Solution**:

(a) Velocity is the derivative of position with respect to time; differentiate each component:

$$
\mathbf{v}(t) = \frac{d\mathbf{r}}{dt} = \frac{d}{dt}(t^3 - 3t)\,\mathbf{i} + \frac{d}{dt}(t^2 - 2t)\,\mathbf{j}
$$

Using the Power Rule:
- $\dfrac{d}{dt}(t^3) = 3t^2$
- $\dfrac{d}{dt}(-3t) = -3$
- $\dfrac{d}{dt}(t^2) = 2t$
- $\dfrac{d}{dt}(-2t) = -2$

Therefore:

$$
\mathbf{v}(t) = (3t^2 - 3)\mathbf{i} + (2t - 2)\mathbf{j}
$$

(b) Acceleration is the derivative of velocity with respect to time:

$$
\mathbf{a}(t) = \frac{d\mathbf{v}}{dt} = \frac{d}{dt}(3t^2 - 3)\,\mathbf{i} + \frac{d}{dt}(2t - 2)\,\mathbf{j}
$$

$$
\mathbf{a}(t) = (6t)\mathbf{i} + 2\mathbf{j}
$$

(c) Substitute $t = 2$:

$$
\mathbf{v}(2) = (3 \times 4 - 3)\mathbf{i} + (4 - 2)\mathbf{j} = 9\mathbf{i} + 2\mathbf{j}\,\text{m/s}
$$

Magnitude of velocity: $|\mathbf{v}(2)| = \sqrt{9^2 + 2^2} = \sqrt{81 + 4} = \sqrt{85} \approx 9.22\,\text{m/s}$

$$
\mathbf{a}(2) = (6 \times 2)\mathbf{i} + 2\mathbf{j} = 12\mathbf{i} + 2\mathbf{j}\,\text{m/s}^2
$$

Magnitude of acceleration: $|\mathbf{a}(2)| = \sqrt{12^2 + 2^2} = \sqrt{144 + 4} = \sqrt{148} = 2\sqrt{37} \approx 12.17\,\text{m/s}^2$

(d) Given $\mathbf{a}(t) = (6t)\mathbf{i} + 2\mathbf{j}$, integrate the acceleration to find velocity:

$$
\mathbf{v}(t) = \int \mathbf{a}(t) \, dt = \left(\int 6t \, dt\right)\mathbf{i} + \left(\int 2 \, dt\right)\mathbf{j}
$$

$$
= (3t^2 + C_1)\mathbf{i} + (2t + C_2)\mathbf{j}
$$

From $\mathbf{v}_0 = \mathbf{v}(0) = -3\mathbf{i} - 2\mathbf{j}$, substituting $t = 0$ gives $C_1 = -3$, $C_2 = -2$. So:

$$
\mathbf{v}(t) = (3t^2 - 3)\mathbf{i} + (2t - 2)\mathbf{j}
$$

This is consistent with part (a). ✓

Now integrate the velocity to find position:

$$
\mathbf{r}(t) = \int \mathbf{v}(t) \, dt = \left(\int (3t^2 - 3) \, dt\right)\mathbf{i} + \left(\int (2t - 2) \, dt\right)\mathbf{j}
$$

$$
= (t^3 - 3t + D_1)\mathbf{i} + (t^2 - 2t + D_2)\mathbf{j}
$$

From $\mathbf{r}_0 = \mathbf{r}(0) = \mathbf{0}$, substituting $t = 0$ gives $D_1 = 0$, $D_2 = 0$. So:

$$
\mathbf{r}(t) = (t^3 - 3t)\mathbf{i} + (t^2 - 2t)\mathbf{j}
$$

This is consistent with the original position function. ✓

---

## 2.4 Practice Problems

The following practice problems are written to examination difficulty, covering all the knowledge points in this chapter. The relevant syllabus reference number is indicated at the start of each problem set.

---

**Problem Set 13.1–13.3: Vector Basics and Geometry**

**1.** Given $\mathbf{a} = 2\mathbf{i} - \mathbf{j}$, $\mathbf{b} = \mathbf{i} + 3\mathbf{j}$.

(a) Find $\mathbf{a} + 2\mathbf{b}$.
(b) Find $|2\mathbf{a} - \mathbf{b}|$.
(c) Find the unit vector in the same direction as $3\mathbf{a} + \mathbf{b}$.

---

**2.** In $\triangle ABC$, $P$ is the midpoint of $BC$, and $Q$ is the midpoint of $CA$. Let $\overrightarrow{AB} = \mathbf{p}$, $\overrightarrow{AC} = \mathbf{q}$.

(a) Express $\overrightarrow{BC}$ in terms of $\mathbf{p}$ and $\mathbf{q}$.
(b) Express $\overrightarrow{PQ}$ in terms of $\mathbf{p}$ and $\mathbf{q}$.
(c) Prove that $PQ \parallel AB$ and $PQ = \frac{1}{2} AB$.

---

**3.** Three points $A$, $B$, $C$ have position vectors $\mathbf{a} = 3\mathbf{i} + 2\mathbf{j}$, $\mathbf{b} = 5\mathbf{i} + 6\mathbf{j}$, $\mathbf{c} = 9\mathbf{i} + 14\mathbf{j}$ respectively.

(a) Prove that $A$, $B$, $C$ are collinear.
(b) Find the ratio $AB:BC$.

---

**Problem Set 13.3–13.4: Vector Geometry and Motion**

**4.** In $\triangle OAB$, $P$ lies on $OA$ such that $OP:PA = 1:2$, and $Q$ lies on $AB$ such that $AQ:QB = 2:3$. Let $\overrightarrow{OA} = \mathbf{a}$, $\overrightarrow{OB} = \mathbf{b}$.

(a) Express $\overrightarrow{OP}$ in terms of $\mathbf{a}$ and $\mathbf{b}$.
(b) Express $\overrightarrow{OQ}$ in terms of $\mathbf{a}$ and $\mathbf{b}$.
(c) Express $\overrightarrow{PQ}$ in terms of $\mathbf{a}$ and $\mathbf{b}$.

---

**5.** Ship $A$ departs from point $(0, 5)$ at velocity $\mathbf{v}_A = (2\mathbf{i} + 3\mathbf{j})\,\text{km/h}$. Ship $B$ departs from point $(10, 0)$ at velocity $\mathbf{v}_B = (-3\mathbf{i} + 4\mathbf{j})\,\text{km/h}$. Both ships depart at the same time.

(a) Write the position vectors $\mathbf{r}_A(t)$ and $\mathbf{r}_B(t)$.
(b) Determine whether the two ships will collide.

---

**6.** A boat's speed in still water is $10\,\text{m/s}$, heading due north. The water current flows at $6\,\text{m/s}$ due east.

(a) Find the resultant velocity vector of the boat relative to the ground.
(b) Find the magnitude and direction (angle from due north) of the resultant velocity.

---

**Problem Set 14.1: Introduction to Rates of Change**

**7.** A particle's displacement $s$ (metres) as a function of time $t$ (seconds) is $s(t) = 4t^2 + 3t$.

(a) Find the average velocity from $t = 1$ to $t = 1 + h$.
(b) Use the limit to find the instantaneous velocity at $t = 1$.

---

**8.** A particle moves in a plane. Its position vector is:

$$
\mathbf{r}(t) = (2t^2 + t)\mathbf{i} + (3t - 1)\mathbf{j}
$$

(a) Find the velocity vector $\mathbf{v}(t)$.
(b) Find the acceleration vector $\mathbf{a}(t)$.
(c) Find the magnitude of the velocity at $t = 2$.

---

**Comprehensive Problem**

**9.** In parallelogram $ABCD$, the position vectors of $A$, $B$, $C$ are $\mathbf{a} = 2\mathbf{i} + \mathbf{j}$, $\mathbf{b} = 5\mathbf{i} + 3\mathbf{j}$, $\mathbf{c} = 4\mathbf{i} + 6\mathbf{j}$ respectively.

(a) Find the position vector of $D$.
(b) Determine whether $\overrightarrow{AB}$ is perpendicular to $\overrightarrow{AD}$.
(c) Find the area of parallelogram $ABCD$.

> Hint: The area of a parallelogram $= |\overrightarrow{AB}| \times |\overrightarrow{AD}| \times \sin\theta$, where $\theta$ is the angle between the two sides. Alternatively, use the determinant formula: Area $= |x_1 y_2 - x_2 y_1|$, where $\overrightarrow{AB} = (x_1, y_1)$, $\overrightarrow{AD} = (x_2, y_2)$.

---

## Answers to Practice Problems

**1.**

(a) $\mathbf{a} + 2\mathbf{b} = (2\mathbf{i} - \mathbf{j}) + 2(\mathbf{i} + 3\mathbf{j}) = (2\mathbf{i} - \mathbf{j}) + (2\mathbf{i} + 6\mathbf{j}) = 4\mathbf{i} + 5\mathbf{j}$

(b) $2\mathbf{a} - \mathbf{b} = 2(2\mathbf{i} - \mathbf{j}) - (\mathbf{i} + 3\mathbf{j}) = (4\mathbf{i} - 2\mathbf{j}) - (\mathbf{i} + 3\mathbf{j}) = 3\mathbf{i} - 5\mathbf{j}$

$|2\mathbf{a} - \mathbf{b}| = \sqrt{3^2 + (-5)^2} = \sqrt{9 + 25} = \sqrt{34}$

(c) $3\mathbf{a} + \mathbf{b} = 3(2\mathbf{i} - \mathbf{j}) + (\mathbf{i} + 3\mathbf{j}) = (6\mathbf{i} - 3\mathbf{j}) + (\mathbf{i} + 3\mathbf{j}) = 7\mathbf{i}$

$|7\mathbf{i}| = 7$, so the unit vector $= \frac{7\mathbf{i}}{7} = \mathbf{i}$

---

**2.**

(a) $\overrightarrow{BC} = \overrightarrow{BA} + \overrightarrow{AC} = -\overrightarrow{AB} + \overrightarrow{AC} = -\mathbf{p} + \mathbf{q}$

(b) $P$ is the midpoint of $BC$, so $\mathbf{r}_P = \frac{\mathbf{r}_B + \mathbf{r}_C}{2}$. $Q$ is the midpoint of $CA$, so $\mathbf{r}_Q = \frac{\mathbf{r}_C + \mathbf{r}_A}{2}$.

$$
\begin{aligned}
\overrightarrow{PQ} &= \mathbf{r}_Q - \mathbf{r}_P \\
&= \frac{\mathbf{r}_C + \mathbf{r}_A}{2} - \frac{\mathbf{r}_B + \mathbf{r}_C}{2} \\
&= \frac{\mathbf{r}_A - \mathbf{r}_B}{2} \\
&= \frac{1}{2}\overrightarrow{BA} = -\frac{1}{2}\overrightarrow{AB} = -\frac{1}{2}\mathbf{p}
\end{aligned}
$$

(c) From (b), $\overrightarrow{PQ} = -\frac{1}{2}\mathbf{p} = -\frac{1}{2}\overrightarrow{AB}$, so $\overrightarrow{PQ} \parallel \overrightarrow{AB}$ and $|\overrightarrow{PQ}| = \frac{1}{2}|\overrightarrow{AB}|$, i.e., $PQ = \frac{1}{2}AB$. ✓

> This property is called the **Midpoint Theorem**: the line segment joining the midpoints of two sides of a triangle is parallel to the third side and equal to half its length.

---

**3.**

(a)
$$
\overrightarrow{AB} = \mathbf{b} - \mathbf{a} = (5\mathbf{i} + 6\mathbf{j}) - (3\mathbf{i} + 2\mathbf{j}) = 2\mathbf{i} + 4\mathbf{j}
$$

$$
\overrightarrow{BC} = \mathbf{c} - \mathbf{b} = (9\mathbf{i} + 14\mathbf{j}) - (5\mathbf{i} + 6\mathbf{j}) = 4\mathbf{i} + 8\mathbf{j}
$$

$\overrightarrow{BC} = 2(2\mathbf{i} + 4\mathbf{j}) = 2\overrightarrow{AB}$. There exists $k = 2$ such that $\overrightarrow{BC} = k\overrightarrow{AB}$, so $A$, $B$, $C$ are collinear.

(b) $|\overrightarrow{AB}| = \sqrt{2^2 + 4^2} = \sqrt{4 + 16} = \sqrt{20} = 2\sqrt{5}$

$|\overrightarrow{BC}| = \sqrt{4^2 + 8^2} = \sqrt{16 + 64} = \sqrt{80} = 4\sqrt{5}$

So $AB:BC = 2\sqrt{5}:4\sqrt{5} = 1:2$

---

**4.**

(a) $OP:PA = 1:2$, so $OP:OA = 1:3$, i.e., $\overrightarrow{OP} = \frac{1}{3}\mathbf{a}$

(b) $AQ:QB = 2:3$, so $AQ:AB = 2:5$, $Q$ is $\frac{2}{5}$ of the way from $A$ to $B$.

$$
\begin{aligned}
\overrightarrow{OQ} &= \overrightarrow{OA} + \frac{2}{5}\overrightarrow{AB} \\
&= \mathbf{a} + \frac{2}{5}(\mathbf{b} - \mathbf{a}) \\
&= \mathbf{a} + \frac{2}{5}\mathbf{b} - \frac{2}{5}\mathbf{a} \\
&= \frac{3}{5}\mathbf{a} + \frac{2}{5}\mathbf{b}
\end{aligned}
$$

(c)
$$
\overrightarrow{PQ} = \overrightarrow{OQ} - \overrightarrow{OP} = \left(\frac{3}{5}\mathbf{a} + \frac{2}{5}\mathbf{b}\right) - \frac{1}{3}\mathbf{a} = \left(\frac{3}{5} - \frac{1}{3}\right)\mathbf{a} + \frac{2}{5}\mathbf{b}
$$

Common denominator: $\frac{3}{5} - \frac{1}{3} = \frac{9}{15} - \frac{5}{15} = \frac{4}{15}$

So $\overrightarrow{PQ} = \frac{4}{15}\mathbf{a} + \frac{2}{5}\mathbf{b}$

---

**5.**

(a)
$$
\mathbf{r}_A(t) = \begin{pmatrix} 0 \\ 5 \end{pmatrix} + \begin{pmatrix} 2 \\ 3 \end{pmatrix} t = \begin{pmatrix} 2t \\ 5 + 3t \end{pmatrix}
$$

$$
\mathbf{r}_B(t) = \begin{pmatrix} 10 \\ 0 \end{pmatrix} + \begin{pmatrix} -3 \\ 4 \end{pmatrix} t = \begin{pmatrix} 10 - 3t \\ 4t \end{pmatrix}
$$

(b) Set $\mathbf{r}_A(t) = \mathbf{r}_B(t)$:

$$
\begin{cases}
2t = 10 - 3t \implies 5t = 10 \implies t = 2 \\[4pt]
5 + 3t = 4t \implies 5 = t \implies t = 5
\end{cases}
$$

The two $t$ values are not equal ($2 \neq 5$), so the two ships will not collide.

---

**6.**

(a) Let due north be the $+y$-axis and due east be the $+x$-axis.

Boat's velocity relative to water: $\mathbf{v}_{B/W} = 10\mathbf{j}$
Water's velocity relative to ground: $\mathbf{v}_{W/G} = 6\mathbf{i}$

Resultant velocity: $\mathbf{v}_{B/G} = 6\mathbf{i} + 10\mathbf{j}$

(b) Magnitude: $|\mathbf{v}_{B/G}| = \sqrt{6^2 + 10^2} = \sqrt{36 + 100} = \sqrt{136} = 2\sqrt{34} \approx 11.66\,\text{m/s}$

Direction: Let $\theta$ be the angle from due north.

$$
\tan\theta = \frac{6}{10} = 0.6 \implies \theta = \arctan(0.6) \approx 30.96^\circ
$$

So the direction is $30.96^\circ$ east of north (or $59.04^\circ$ north of east).

---

**7.**

(a)
$$
\begin{aligned}
\frac{s(1+h) - s(1)}{h} &= \frac{[4(1+h)^2 + 3(1+h)] - [4 + 3]}{h} \\
&= \frac{[4(1 + 2h + h^2) + 3 + 3h] - 7}{h} \\
&= \frac{4 + 8h + 4h^2 + 3 + 3h - 7}{h} \\
&= \frac{11h + 4h^2}{h} = 11 + 4h
\end{aligned}
$$

(b) $v(1) = \displaystyle\lim_{h \to 0} (11 + 4h) = 11\,\text{m/s}$

Verification: $s'(t) = 8t + 3$, $s'(1) = 8 + 3 = 11$ ✓

---

**8.**

(a) $\mathbf{v}(t) = \dfrac{d\mathbf{r}}{dt} = (4t + 1)\mathbf{i} + 3\mathbf{j}$

(b) $\mathbf{a}(t) = \dfrac{d\mathbf{v}}{dt} = 4\mathbf{i}$

(c) $\mathbf{v}(2) = (4 \times 2 + 1)\mathbf{i} + 3\mathbf{j} = 9\mathbf{i} + 3\mathbf{j}$

$|\mathbf{v}(2)| = \sqrt{9^2 + 3^2} = \sqrt{81 + 9} = \sqrt{90} = 3\sqrt{10} \approx 9.49\,\text{m/s}$

---

**9.**

(a) In parallelogram $ABCD$, $\overrightarrow{AD} = \overrightarrow{BC}$.

$$
\overrightarrow{BC} = \mathbf{c} - \mathbf{b} = (4\mathbf{i} + 6\mathbf{j}) - (5\mathbf{i} + 3\mathbf{j}) = -\mathbf{i} + 3\mathbf{j}
$$

So $\mathbf{d} = \mathbf{a} + \overrightarrow{BC} = (2\mathbf{i} + \mathbf{j}) + (-\mathbf{i} + 3\mathbf{j}) = \mathbf{i} + 4\mathbf{j}$

(b) $\overrightarrow{AB} = \mathbf{b} - \mathbf{a} = (5\mathbf{i} + 3\mathbf{j}) - (2\mathbf{i} + \mathbf{j}) = 3\mathbf{i} + 2\mathbf{j}$

$\overrightarrow{AD} = \mathbf{d} - \mathbf{a} = (\mathbf{i} + 4\mathbf{j}) - (2\mathbf{i} + \mathbf{j}) = -\mathbf{i} + 3\mathbf{j}$

Dot product: $\overrightarrow{AB} \cdot \overrightarrow{AD} = (3)(-1) + (2)(3) = -3 + 6 = 3 \neq 0$

So $\overrightarrow{AB}$ and $\overrightarrow{AD}$ are **not perpendicular**.

(c) Method 1 (using the determinant formula for cross product):

$$
\text{Area} = |x_1 y_2 - x_2 y_1|
$$

where $\overrightarrow{AB} = (3, 2)$, $\overrightarrow{AD} = (-1, 3)$.

$$
\text{Area} = |3 \times 3 - 2 \times (-1)| = |9 + 2| = 11
$$

Method 2 (using $|\overrightarrow{AB}| \cdot |\overrightarrow{AD}| \cdot \sin\theta$):

$$
|\overrightarrow{AB}| = \sqrt{3^2 + 2^2} = \sqrt{13}, \quad |\overrightarrow{AD}| = \sqrt{(-1)^2 + 3^2} = \sqrt{10}
$$

From the dot product $\overrightarrow{AB} \cdot \overrightarrow{AD} = |\overrightarrow{AB}||\overrightarrow{AD}|\cos\theta$:

$$
3 = \sqrt{13} \cdot \sqrt{10} \cdot \cos\theta \implies \cos\theta = \frac{3}{\sqrt{130}}
$$

$$
\sin\theta = \sqrt{1 - \cos^2\theta} = \sqrt{1 - \frac{9}{130}} = \sqrt{\frac{121}{130}} = \frac{11}{\sqrt{130}}
$$

$$
\text{Area} = \sqrt{13} \cdot \sqrt{10} \cdot \frac{11}{\sqrt{130}} = \sqrt{130} \cdot \frac{11}{\sqrt{130}} = 11
$$

The area of the parallelogram is $11$ square units. ✓

---

## Chapter Summary

### Syllabus Coverage Checklist

| Syllabus Ref | Content | Section | Worked Examples | Practice Problems |
|:---:|------|:---:|:---:|:---:|
| 13.1 | Vector notation | 2.1.1 | 2.1(1) | 1 |
| 13.2 | Position vectors and unit vectors | 2.1.2, 2.1.4 | 2.1(1) | 1(c) |
| 13.3 | Magnitude, addition/subtraction, scalar multiplication, vector geometry | 2.1.3, 2.1.5–2.1.8, 2.2.1 | 2.1, 2.2 | 1–4, 9 |
| 13.4 | Composition and resolution of velocities, collision problems | 2.2.2 | 2.3 | 5, 6 |
| 14.1 | Rates of change and the idea of limits | 2.3 | 2.4 | 7, 8 |

### Quick Reference Formula Table

**Vector Part**:

| Concept | Formula |
|:---|:---|
| Vector representation | $\mathbf{v} = x\mathbf{i} + y\mathbf{j} = \begin{pmatrix} x \\ y \end{pmatrix}$ |
| Magnitude | $|\mathbf{v}| = \sqrt{x^2 + y^2}$ |
| Unit vector | $\hat{\mathbf{v}} = \dfrac{\mathbf{v}}{|\mathbf{v}|}$ |
| Displacement | $\overrightarrow{AB} = \mathbf{r}_B - \mathbf{r}_A$ |
| Midpoint | $\mathbf{r}_M = \dfrac{\mathbf{r}_A + \mathbf{r}_B}{2}$ |
| Section formula ($AP:PB = m:n$) | $\mathbf{r}_P = \dfrac{n\mathbf{r}_A + m\mathbf{r}_B}{m+n}$ |
| Parallel condition | $\mathbf{a} = k\mathbf{b}$ (there exists scalar $k$) |
| Perpendicular condition (dot product) | $\mathbf{u} \cdot \mathbf{v} = u_x v_x + u_y v_y = 0$ |
| Perpendicularity using slope | $k_1 \cdot k_2 = -1$ |
| Composition of velocities | $\mathbf{v}_{A/C} = \mathbf{v}_{A/B} + \mathbf{v}_{B/C}$ |
| Resolution of velocity | $\mathbf{v} = (v\cos\theta)\mathbf{i} + (v\sin\theta)\mathbf{j}$ |
| Constant velocity motion | $\mathbf{r}(t) = \mathbf{r}_0 + \mathbf{v}t$ |
| Collision condition | $\mathbf{r}_1(t) = \mathbf{r}_2(t)$ |

**Rates of Change Part**:

| Concept | Formula |
|:---|:---|
| Definition of derivative | $f'(a) = \displaystyle\lim_{h \to 0} \dfrac{f(a + h) - f(a)}{h}$ |
| Power Rule | $\dfrac{d}{dx}(x^n) = n x^{n-1}$ |
| Velocity (vector) | $\mathbf{v}(t) = \dfrac{d\mathbf{r}}{dt} = \dfrac{dx}{dt}\mathbf{i} + \dfrac{dy}{dt}\mathbf{j}$ |
| Acceleration (vector) | $\mathbf{a}(t) = \dfrac{d\mathbf{v}}{dt} = \dfrac{d^2x}{dt^2}\mathbf{i} + \dfrac{d^2y}{dt^2}\mathbf{j}$ |
| Integration to find velocity | $\mathbf{v}(t) = \int \mathbf{a}(t) \, dt + \mathbf{v}_0$ |
| Integration to find position | $\mathbf{r}(t) = \int \mathbf{v}(t) \, dt + \mathbf{r}_0$ |

### Learning Roadmap

Starting from this chapter, subsequent chapters will deepen your understanding as follows:

- **Chapter 5 (Differentiation)**: Systematic study of differentiation rules (chain rule, product rule, quotient rule), and using derivatives to find tangents, normals, and stationary points
- **Chapter 7 (Integration)**: Learning the inverse operation of differentiation — integration — to master the complete method of finding velocity and position from acceleration
- **Chapter 10 (Comprehensive Applications)**: Combining vectors and calculus to solve complete kinematics problems

---
---

# Chapter 3: Quadratic Functions (Including Polynomial Factors)

## Chapter Introduction

Quadratic functions are a core tool that runs throughout IGCSE Additional Mathematics (0606). From solving equations to finding extreme values, from inequalities to curve analysis, knowledge of quadratic functions is ubiquitous. This chapter organically integrates the conceptual system of quadratic functions with polynomial factorisation, forming a complete logical chain from "factors" to "functions" to "graphs."

**Syllabus Mapping**:

| Syllabus Ref | Content | Corresponding Section |
|:---:|:---|:---:|
| **3.1** | Remainder Theorem and Factor Theorem | §3.1.1, §3.1.2 |
| **3.2** | Factorising polynomials (cubic → linear × quadratic) | §3.1.3 |
| **3.3** | Solving cubic equations | §3.1.4 |
| **2.1** | Completing the square or differentiation to find stationary values of quadratic functions | §3.4, §3.7 |
| **2.2** | Using stationary values to sketch graphs or find ranges | §3.4 |
| **2.3** | Discriminant and conditions for roots, relative position of a line and a curve | §3.2 |
| **2.4** | Solving quadratic equations (factorisation, formula, completing the square) | §3.3 |
| **2.5** | Quadratic inequalities (algebraic or graphical methods) | §3.5 |
| **4.4** | Graphs of products of three linear factors and absolute value graphs | §3.6.1, §3.6.2 |
| **4.5** | Graphical solution of cubic inequalities | §3.6.3 |

---

## 3.1 Factorisation of Polynomials

### 3.1.1 The Remainder Theorem

**Statement of the Theorem**: When a polynomial $f(x)$ is divided by a linear factor $(x - a)$, the remainder is equal to $f(a)$.

**Complete Derivation**:

Let $f(x)$ be divided by $(x - a)$, yielding a quotient $q(x)$ and a remainder $R$. Since the divisor $(x - a)$ is of degree 1, the degree of the remainder $R$ must be lower than the degree of the divisor, so $R$ can only be a constant. Therefore, we have the identity:

$$
f(x) = (x - a) \cdot q(x) + R
$$

This identity holds for **all** values of $x$ — this is a fundamental property of polynomial identities.

Now, we cleverly choose to substitute $x = a$. We choose $x = a$ because it makes the factor $(x - a)$ equal to zero, thereby eliminating the term containing $q(x)$:

$$
f(a) = (a - a) \cdot q(a) + R = 0 \cdot q(a) + R = R
$$

Therefore $R = f(a)$. This is the entirety of the Remainder Theorem.

**Why is this theorem so useful?**

To find the remainder, we do not need to perform long division — we simply substitute $x = a$ into the original polynomial and evaluate. This greatly simplifies the calculation, especially when the polynomial is of a higher degree.

**Generalised Form**:

If the divisor is $(ax + b)$, then set $ax + b = 0$ to obtain $x = -\frac{b}{a}$, and the remainder is:

$$
R = f\!\left(-\frac{b}{a}\right)
$$

The reasoning is exactly the same — find the value of $x$ that makes the divisor zero, then substitute.

---

**Example 1**: Find the remainder when $f(x) = 2x^3 - 3x^2 + 4x - 5$ is divided by $x - 2$.

**Detailed solution**:

The divisor is $x - 2$; set $x - 2 = 0$ to get $x = 2$. By the Remainder Theorem, the remainder $R = f(2)$.

Substitute and calculate term by term:

$$
\begin{aligned}
f(2) &= 2(2)^3 - 3(2)^2 + 4(2) - 5 \\
&\text{(first compute powers: $2^3 = 8$, $2^2 = 4$)} \\
&= 2 \times 8 - 3 \times 4 + 8 - 5 \\
&\text{(then multiply: $2 \times 8 = 16$, $3 \times 4 = 12$)} \\
&= 16 - 12 + 8 - 5 \\
&= 7
\end{aligned}
$$

So the remainder is $7$.

---

**Example 2**: When $f(x) = x^3 + kx^2 - 2x + 3$ is divided by $x + 1$, the remainder is $5$. Find the value of the constant $k$.

**Detailed solution**:

The divisor is $x + 1$; set $x + 1 = 0$ to get $x = -1$. Note the sign: the solution of $x + 1 = 0$ is $x = -1$, not $x = 1$. This is a common mistake.

By the Remainder Theorem, the remainder equals $f(-1)$. The problem states the remainder is $5$, so $f(-1) = 5$.

Substitute and calculate:

$$
\begin{aligned}
f(-1) &= (-1)^3 + k(-1)^2 - 2(-1) + 3 = 5 \\
&\text{(compute term by term: $(-1)^3 = -1$, $(-1)^2 = 1$, $-2(-1) = 2$)} \\
-1 + k + 2 + 3 &= 5 \\
k + 4 &= 5 \\
k &= 1
\end{aligned}
$$

So $k = 1$.

---

**Example 3**: Find the remainder when $f(x) = 6x^3 + x^2 - 8x + 2$ is divided by $2x - 1$.

**Detailed solution**:

The divisor is $2x - 1$, not of the simple form $(x - a)$. Set $2x - 1 = 0$, giving $x = \frac{1}{2}$.

When substituting $x = \frac{1}{2}$, pay careful attention to the fraction arithmetic:

$$
\begin{aligned}
f\!\left(\frac{1}{2}\right) &= 6\left(\frac{1}{2}\right)^3 + \left(\frac{1}{2}\right)^2 - 8\left(\frac{1}{2}\right) + 2 \\
&= 6 \times \frac{1}{8} + \frac{1}{4} - 4 + 2 \\
&= \frac{6}{8} + \frac{1}{4} - 2 \\
&= \frac{3}{4} + \frac{1}{4} - 2 \\
&= 1 - 2 = -1
\end{aligned}
$$

So the remainder is $-1$.

---

**Example 4**: Find the remainder when $f(x) = 4x^4 - 3x^3 + 2x^2 - x + 5$ is divided by $x - 1$.

**Detailed solution**:

Set $x - 1 = 0$ to get $x = 1$. The remainder $R = f(1)$.

$$
\begin{aligned}
f(1) &= 4(1)^4 - 3(1)^3 + 2(1)^2 - 1 + 5 \\
&= 4 - 3 + 2 - 1 + 5 \\
&= 7
\end{aligned}
$$

The remainder is $7$. Even with a higher-degree polynomial, the Remainder Theorem still applies.

---

**Example 5**: Find the remainder when $f(x) = x^4 - 2x^3 + 3x^2 - 4x + 2$ is divided by $x + 2$.

**Detailed solution**:

Set $x + 2 = 0$ to get $x = -2$.

$$
\begin{aligned}
f(-2) &= (-2)^4 - 2(-2)^3 + 3(-2)^2 - 4(-2) + 2 \\
&= 16 - 2(-8) + 3(4) + 8 + 2 \\
&= 16 + 16 + 12 + 8 + 2 \\
&= 54
\end{aligned}
$$

The remainder is $54$.

---

**Example 6**: Find the remainder when $f(x) = 8x^3 - 4x^2 + 2x - 1$ is divided by $2x + 3$.

**Detailed solution**:

Set $2x + 3 = 0$ to get $x = -\frac{3}{2}$. The remainder $R = f\!\left(-\frac{3}{2}\right)$.

$$
\begin{aligned}
f\!\left(-\frac{3}{2}\right) &= 8\left(-\frac{3}{2}\right)^3 - 4\left(-\frac{3}{2}\right)^2 + 2\left(-\frac{3}{2}\right) - 1 \\
&= 8\left(-\frac{27}{8}\right) - 4\left(\frac{9}{4}\right) - 3 - 1 \\
&= -27 - 9 - 3 - 1 = -40
\end{aligned}
$$

The remainder is $-40$.

---

### 3.1.2 The Factor Theorem

**Statement of the Theorem**: If $f(a) = 0$, then $(x - a)$ is a factor of $f(x)$. Conversely, if $(x - a)$ is a factor of $f(x)$, then $f(a) = 0$.

**Derivation**:

The Factor Theorem is a direct corollary of the Remainder Theorem. By the Remainder Theorem, the remainder when $f(x)$ is divided by $(x - a)$ equals $f(a)$. If $f(a) = 0$, this means the remainder is zero — that is, $(x - a)$ **exactly divides** $f(x)$ with no remainder, so $(x - a)$ is a factor of $f(x)$.

Conversely, if $(x - a)$ is a factor of $f(x)$, then $f(x) = (x - a) \cdot q(x)$. Substituting $x = a$ gives $f(a) = 0$.

**Practical significance**:

To determine whether $(x - a)$ is a factor of $f(x)$, we only need to check whether $f(a) = 0$. This is much faster than performing long division. Moreover, the Factor Theorem is the **starting point for factorising cubic polynomials** — by testing roots to find a zero, we have found a linear factor.

**Root-testing strategy**:

For polynomials with integer coefficients, possible rational roots are $\pm \frac{\text{factors of the constant term}}{\text{factors of the leading coefficient}}$. For cubic polynomials, we usually start by testing the simplest values: $\pm 1, \pm 2, \pm 3$.

---

**Example 1**: Show that $(x - 2)$ is a factor of $f(x) = x^3 - 3x^2 - 4x + 12$.

**Detailed solution**:

To prove that $(x - 2)$ is a factor, by the Factor Theorem, we only need to show that $f(2) = 0$.

$$
\begin{aligned}
f(2) &= 2^3 - 3(2)^2 - 4(2) + 12 \\
&= 8 - 12 - 8 + 12 = 0
\end{aligned}
$$

Since $f(2) = 0$, $(x - 2)$ is a factor of $f(x)$. ✓

---

**Example 2**: The polynomial $f(x) = 2x^3 + ax^2 + bx - 6$ has factors $(x - 1)$ and $(x + 2)$. Find the values of $a$ and $b$.

**Detailed solution**:

By the Factor Theorem:
- $(x - 1)$ is a factor $\Rightarrow$ $f(1) = 0$
- $(x + 2)$ is a factor $\Rightarrow$ $f(-2) = 0$

From $f(1) = 0$:

$$
2 + a + b - 6 = 0 \;\Rightarrow\; a + b = 4 \tag{1}
$$

From $f(-2) = 0$:

$$
-16 + 4a - 2b - 6 = 0 \;\Rightarrow\; 4a - 2b = 22 \tag{2}
$$

Solve (1) and (2) simultaneously. From (1), $b = 4 - a$. Substitute into (2):

$$
4a - 2(4 - a) = 22 \;\Rightarrow\; 4a - 8 + 2a = 22 \;\Rightarrow\; 6a = 30 \;\Rightarrow\; a = 5
$$

Therefore $b = 4 - 5 = -1$.

---

**Example 3**: Given that $x - 2$ is a factor of $f(x) = x^3 - px^2 + 5x - 2$, find the value of $p$ and fully factorise $f(x)$.

**Detailed solution**:

By the Factor Theorem, $f(2) = 0$:

$$
8 - 4p + 10 - 2 = 16 - 4p = 0 \;\Rightarrow\; p = 4
$$

So $f(x) = x^3 - 4x^2 + 5x - 2$.

Use synthetic division by $(x - 2)$:

$$
\begin{array}{r|rrrr}
2 & 1 & -4 & 5 & -2 \\
  &   & 2  & -4 & 2 \\
\hline
  & 1 & -2 & 1 & 0
\end{array}
$$

The quotient is $x^2 - 2x + 1 = (x - 1)^2$.

Therefore:

$$
\boxed{f(x) = (x - 2)(x - 1)^2}
$$

---

**Example 4**: Given that $x - 3$ is a factor of $f(x) = 2x^3 - 7x^2 + 2x + 3$, factorise $f(x)$.

**Detailed solution**:

Synthetic division:

$$
\begin{array}{r|rrrr}
3 & 2 & -7 & 2 & 3 \\
  &   & 6  & -3 & -3 \\
\hline
  & 2 & -1 & -1 & 0
\end{array}
$$

The quotient is $2x^2 - x - 1$.

Factorise the quadratic: $2x^2 - x - 1 = 2x^2 - 2x + x - 1 = 2x(x - 1) + 1(x - 1) = (2x + 1)(x - 1)$.

Therefore:

$$
\boxed{f(x) = (x - 3)(2x + 1)(x - 1)}
$$

---

**Example 5**: The polynomial $f(x) = 3x^3 + kx^2 - 4x + 4$ has a factor $(x + 1)$. Find the value of $k$.

**Detailed solution**:

$(x + 1)$ is a factor $\Rightarrow$ $f(-1) = 0$.

$$
f(-1) = -3 + k + 4 + 4 = k + 5 = 0 \;\Rightarrow\; k = -5
$$

---

**Example 6**: Given that $x - 1$ and $x - 2$ are both factors of $f(x) = x^3 + ax^2 + bx + c$, and that when $f(x)$ is divided by $x + 1$, the remainder is $-12$, find the values of $a, b, c$ and write $f(x)$ in fully factorised form.

**Detailed solution**:

From the given conditions:

$$
\begin{aligned}
f(1) &= 1 + a + b + c = 0 &\Rightarrow\quad a + b + c = -1 \tag{1}\\
f(2) &= 8 + 4a + 2b + c = 0 &\Rightarrow\quad 4a + 2b + c = -8 \tag{2}\\
f(-1) &= -1 + a - b + c = -12 &\Rightarrow\quad a - b + c = -11 \tag{3}
\end{aligned}
$$

(2) − (1): $3a + b = -7 \tag{4}$
(1) − (3): $2b = 10 \Rightarrow b = 5$

Substitute into (4): $3a + 5 = -7 \Rightarrow 3a = -12 \Rightarrow a = -4$

Substitute into (1): $-4 + 5 + c = -1 \Rightarrow c = -2$

So $f(x) = x^3 - 4x^2 + 5x - 2$.

Verification:
- $f(1) = 1 - 4 + 5 - 2 = 0$ ✓
- $f(2) = 8 - 16 + 10 - 2 = 0$ ✓
- $f(-1) = -1 - 4 - 5 - 2 = -12$ ✓

Divide by $(x - 1)$ using synthetic division:

$$
\begin{array}{r|rrrr}
1 & 1 & -4 & 5 & -2 \\
  &   & 1  & -3 & 2 \\
\hline
  & 1 & -3 & 2 & 0
\end{array}
$$

The quotient is $x^2 - 3x + 2 = (x - 1)(x - 2)$.

So $f(x) = (x - 1)^2(x - 2)$.

---

### 3.1.3 Factorising Cubic Polynomials

Factorising a cubic polynomial $f(x) = ax^3 + bx^2 + cx + d$ is like unlocking a "three-layer lock": first find a key (a linear factor), open the first lock to reveal a quadratic lock, then use familiar quadratic factorisation methods to open it.

**Standard Procedure**:

**Step 1: Test roots — Use the Factor Theorem to find a linear factor**

Test $x = \pm 1, \pm 2, \pm 3, \dots$ and fractions $\pm \frac{\text{factors of the constant term}}{\text{factors of the leading coefficient}}$. Find $p$ such that $f(p) = 0$; then $(x - p)$ is a factor.

**Step 2: Synthetic division — Find the quadratic quotient**

Divide $f(x)$ by $(x - p)$ to obtain a quadratic $Ax^2 + Bx + C$.

**Step 3: Factorise the quadratic**

Use factorisation, the quadratic formula, or completing the square to factor $Ax^2 + Bx + C$.

**Step 4: Complete factorisation**

Write $f(x) = (x - p) \times (\text{factorisation of the quadratic})$.

---

#### Detailed Explanation of Synthetic Division

Synthetic division is a concise format for polynomial division that only uses coefficients, without writing variables.

**Steps** (using $f(x) = a_3 x^3 + a_2 x^2 + a_1 x + a_0$ divided by $(x - p)$ as an example):

```
p |  a₃   a₂   a₁   a₀
  |      p·b₂ p·b₁ p·b₀
  ------------------------
     b₂   b₁   b₀   R
```

where:
- $b_2 = a_3$ (bring down the leading coefficient)
- $b_1 = a_2 + p \cdot b_2$
- $b_0 = a_1 + p \cdot b_1$
- $R = a_0 + p \cdot b_0$ (remainder)

The quotient is $b_2 x^2 + b_1 x + b_0$, and the remainder is $R$.

---

**Example 1**: Factorise $f(x) = x^3 - 6x^2 + 11x - 6$.

**Detailed solution**:

**Step 1: Test roots**. Start with the simplest value $x = 1$:

$$
f(1) = 1 - 6 + 11 - 6 = 0
$$

So $(x - 1)$ is a factor.

**Step 2: Synthetic division**.

```
    1 |  1   -6   11   -6
      |      1   -5    6
      -------------------
         1   -5    6    0
```

**Detailed process explanation**:
- Place the coefficients $1, -6, 11, -6$ in order.
- The number $1$ on the far left comes from the root $x = 1$ of $(x - 1)$.
- **Bring down**: Write the leading coefficient $1$ directly below.
- **Step 1**: $1 \times 1 = 1$, write it in the second position of the second row. $-6 + 1 = -5$, write it below.
- **Step 2**: $(-5) \times 1 = -5$, write it in the third position of the second row. $11 + (-5) = 6$, write it below.
- **Step 3**: $6 \times 1 = 6$, write it in the fourth position of the second row. $-6 + 6 = 0$, write it below.

The numbers in the third row — $1, -5, 6, 0$ — mean:
- $1, -5, 6$ are the coefficients of the quotient: $1x^2 - 5x + 6$
- The final $0$ is the remainder — a remainder of $0$ confirms exact divisibility, verifying that $(x - 1)$ is indeed a factor.

**Step 3: Factorise the quadratic**.

$$
x^2 - 5x + 6 = (x - 2)(x - 3)
$$

Find two numbers whose product is $6$ and sum is $-5$: they are $-2$ and $-3$.

**Step 4: Complete factorisation**.

$$
\boxed{f(x) = (x - 1)(x - 2)(x - 3)}
$$

---

**Example 2**: Factorise $f(x) = 2x^3 - 3x^2 - 11x + 6$.

**Detailed solution**:

**Step 1: Test roots**.

The leading coefficient is $2$ and the constant term is $6$. Possible rational roots are $\pm 1, \pm 2, \pm 3, \pm 6, \pm \frac{1}{2}, \pm \frac{3}{2}$.

Test $x = 2$: $f(2) = 16 - 12 - 22 + 6 = -12 \neq 0$.
Test $x = -2$:

$$
f(-2) = -16 - 12 + 22 + 6 = 0
$$

So $(x + 2)$ is a factor (note $x = -2$ corresponds to $x + 2 = 0$).

**Step 2: Synthetic division**.

```
    -2 |  2   -3   -11    6
       |     -4    14    -6
       --------------------
          2   -7     3    0
```

**Process explanation**:
- The number on the far left is $-2$ (the value of the root).
- Bring down $2$.
- $2 \times (-2) = -4$, $-3 + (-4) = -7$.
- $(-7) \times (-2) = 14$, $-11 + 14 = 3$.
- $3 \times (-2) = -6$, $6 + (-6) = 0$.

The quotient is $2x^2 - 7x + 3$.

**Step 3: Factorise $2x^2 - 7x + 3$**.

$a \times c = 2 \times 3 = 6$. Find two numbers whose product is $6$ and sum is $-7$: $(-1) \times (-6) = 6$, $(-1) + (-6) = -7$.

Split and group:

$$
\begin{aligned}
2x^2 - 7x + 3 &= 2x^2 - x - 6x + 3 \\
&= x(2x - 1) - 3(2x - 1) \\
&= (2x - 1)(x - 3)
\end{aligned}
$$

**Step 4: Complete factorisation**.

$$
\boxed{f(x) = (x + 2)(2x - 1)(x - 3)}
$$

---

**Example 3**: Factorise $f(x) = 3x^3 + 6x^2 - 3x - 6$.

**Detailed solution**:

**Step 0: Observation**. All coefficients are divisible by $3$, so first take out the common factor $3$:

$$
f(x) = 3(x^3 + 2x^2 - x - 2)
$$

Let $g(x) = x^3 + 2x^2 - x - 2$.

**Step 1: Test roots**. Test $x = 1$: $g(1) = 1 + 2 - 1 - 2 = 0$. So $(x - 1)$ is a factor of $g(x)$.

**Step 2: Synthetic division**.

```
    1 |  1    2   -1   -2
      |       1    3    2
      --------------------
         1    3    2    0
```

The quotient is $x^2 + 3x + 2$.

**Step 3: Factorise the quadratic**.

$$
x^2 + 3x + 2 = (x + 1)(x + 2)
$$

**Step 4: Complete factorisation**.

$$
\boxed{f(x) = 3(x - 1)(x + 1)(x + 2)}
$$

---

**Example 4**: Factorise $f(x) = 2x^3 - 9x^2 + 7x + 6$.

**Detailed solution**:

**Step 1: Test roots**.

Test $x = 1$: $f(1) = 2 - 9 + 7 + 6 = 6 \neq 0$.
Test $x = -1$: $f(-1) = -2 - 9 - 7 + 6 = -12 \neq 0$.
Test $x = 2$: $f(2) = 16 - 36 + 14 + 6 = 0$. ✓

So $(x - 2)$ is a factor.

**Step 2: Synthetic division**.

```
    2 |  2   -9    7    6
      |       4  -10   -6
      --------------------
         2   -5   -3    0
```

The quotient is $2x^2 - 5x - 3$.

**Step 3: Factorise $2x^2 - 5x - 3$**.

$a \times c = 2 \times (-3) = -6$. Find two numbers whose product is $-6$ and sum is $-5$: $(-6) \times 1 = -6$, $(-6) + 1 = -5$.

$$
2x^2 - 6x + x - 3 = 2x(x - 3) + 1(x - 3) = (2x + 1)(x - 3)
$$

**Step 4: Complete factorisation**.

$$
\boxed{f(x) = (x - 2)(2x + 1)(x - 3)}
$$

---

**Example 5**: Factorise $f(x) = 6x^3 - 7x^2 - 7x + 6$.

**Detailed solution**:

**Step 1: Test roots**.

Test $x = 1$: $f(1) = 6 - 7 - 7 + 6 = -2 \neq 0$.
Test $x = -1$: $f(-1) = -6 - 7 + 7 + 6 = 0$. ✓

So $(x + 1)$ is a factor.

**Step 2: Synthetic division**.

```
    -1 |  6   -7   -7    6
       |     -6   13   -6
       --------------------
          6  -13    6    0
```

The quotient is $6x^2 - 13x + 6$.

**Step 3: Factorise $6x^2 - 13x + 6$**.

$a \times c = 6 \times 6 = 36$. Find two numbers whose product is $36$ and sum is $-13$: $(-9) \times (-4) = 36$, $(-9) + (-4) = -13$.

$$
6x^2 - 9x - 4x + 6 = 3x(2x - 3) - 2(2x - 3) = (3x - 2)(2x - 3)
$$

**Step 4: Complete factorisation**.

$$
\boxed{f(x) = (x + 1)(3x - 2)(2x - 3)}
$$

---

**Example 6**: Factorise $f(x) = x^3 + 2x^2 - 5x - 6$.

**Detailed solution**:

**Step 1: Test roots**.

Test $x = 1$: $f(1) = 1 + 2 - 5 - 6 = -8 \neq 0$.
Test $x = -1$: $f(-1) = -1 + 2 + 5 - 6 = 0$. ✓

So $(x + 1)$ is a factor.

**Step 2: Synthetic division**.

```
    -1 |  1    2   -5   -6
       |     -1   -1    6
       --------------------
          1    1   -6    0
```

The quotient is $x^2 + x - 6$.

**Step 3: Factorise the quadratic**.

$$
x^2 + x - 6 = (x + 3)(x - 2)
$$

**Step 4: Complete factorisation**.

$$
\boxed{f(x) = (x + 1)(x + 3)(x - 2)}
$$

---

### 3.1.4 Solving Cubic Equations

The process for solving a cubic equation $ax^3 + bx^2 + cx + d = 0$ is **to factorise the cubic polynomial, then set each factor equal to zero**. This is because if the product of several factors is zero, at least one of the factors must be zero.

---

**Example 1**: Solve $x^3 - 4x^2 + x + 6 = 0$.

**Detailed solution**:

Test roots: $f(2) = 8 - 16 + 2 + 6 = 0$, so $(x - 2)$ is a factor.

Synthetic division:

```
    2 |  1   -4    1    6
      |       2   -4   -6
      --------------------
         1   -2   -3    0
```

Quotient: $x^2 - 2x - 3 = (x - 3)(x + 1)$.

So $(x - 2)(x - 3)(x + 1) = 0$.

Therefore:

$$
\boxed{x = 2,\quad x = 3,\quad x = -1}
$$

---

**Example 2**: Solve $x^3 - 5x^2 + 8x - 4 = 0$.

**Detailed solution**:

Test $x = 1$: $f(1) = 1 - 5 + 8 - 4 = 0$.

Synthetic division:

```
    1 |  1   -5    8   -4
      |       1   -4    4
      --------------------
         1   -4    4    0
```

Quotient: $x^2 - 4x + 4 = (x - 2)^2$.

So $(x - 1)(x - 2)^2 = 0$.

Therefore:

$$
\boxed{x = 1 \quad\text{or}\quad x = 2\ (\text{double root})}
$$

---

**Example 3**: Given that $x = 2$ is a root of $2x^3 - 3x^2 - 18x + k = 0$, find $k$ and solve the equation.

**Detailed solution**:

Substitute $x = 2$: $16 - 12 - 36 + k = -32 + k = 0 \Rightarrow k = 32$.

The equation is $2x^3 - 3x^2 - 18x + 32 = 0$. We know $(x - 2)$ is a factor.

Synthetic division:

```
    2 |  2   -3   -18   32
      |       4     2   -32
      ----------------------
         2    1   -16    0
```

Quotient: $2x^2 + x - 16$. Use the quadratic formula:

$$
x = \frac{-1 \pm \sqrt{1 + 128}}{4} = \frac{-1 \pm \sqrt{129}}{4}
$$

Therefore the solutions are:

$$
\boxed{x = 2,\quad x = \frac{-1 + \sqrt{129}}{4},\quad x = \frac{-1 - \sqrt{129}}{4}}
$$

---

**Example 4**: Solve $x^3 - 2x^2 - 5x + 6 = 0$.

**Detailed solution**:

Test $x = 1$: $f(1) = 1 - 2 - 5 + 6 = 0$. ✓

Synthetic division:

```
    1 |  1   -2   -5    6
      |       1   -1   -6
      --------------------
         1   -1   -6    0
```

Quotient: $x^2 - x - 6 = (x - 3)(x + 2)$.

So $(x - 1)(x - 3)(x + 2) = 0$.

Therefore:

$$
\boxed{x = 1,\quad x = 3,\quad x = -2}
$$

---

**Example 5**: Solve $2x^3 - x^2 - 13x - 6 = 0$.

**Detailed solution**:

Test $x = -1$: $f(-1) = -2 - 1 + 13 - 6 = 4 \neq 0$.
Test $x = -2$: $f(-2) = -16 - 4 + 26 - 6 = 0$. ✓

Synthetic division:

```
    -2 |  2   -1   -13   -6
       |     -4    10    6
       ---------------------
          2   -5    -3    0
```

Quotient: $2x^2 - 5x - 3 = (2x + 1)(x - 3)$.

So $(x + 2)(2x + 1)(x - 3) = 0$.

Therefore:

$$
\boxed{x = -2,\quad x = -\frac{1}{2},\quad x = 3}
$$

---

**Example 6**: Given that $x = 3$ is a root of $x^3 + 4x^2 - 11x + k = 0$, find $k$ and solve the equation.

**Detailed solution**:

Substitute $x = 3$: $27 + 36 - 33 + k = 30 + k = 0 \Rightarrow k = -30$.

The equation is $x^3 + 4x^2 - 11x - 30 = 0$. We know $(x - 3)$ is a factor.

Synthetic division:

```
    3 |  1    4   -11   -30
      |       3    21    30
      ---------------------
         1    7    10     0
```

Quotient: $x^2 + 7x + 10 = (x + 2)(x + 5)$.

So $(x - 3)(x + 2)(x + 5) = 0$.

Therefore:

$$
\boxed{x = 3,\quad x = -2,\quad x = -5}
$$

---

## 3.2 The Discriminant $\Delta$

### 3.2.1 Definition and Three Cases

For a quadratic equation $ax^2 + bx + c = 0$ ($a \neq 0$), the quadratic formula is:

$$
x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
$$

The expression under the square root, $b^2 - 4ac$, determines the nature of the roots. We define the **discriminant**:

$$
\boxed{\Delta = b^2 - 4ac}
$$

**Why does $\Delta$ determine the nature of the roots?**

| Value of $\Delta$ | $\sqrt{\Delta}$ | Nature of Roots |
|:---:|:---|:---|
| $\Delta > 0$ | $\sqrt{\Delta}$ is a positive real number | $\frac{-b \pm \text{positive}}{2a}$, two distinct real roots |
| $\Delta = 0$ | $\sqrt{\Delta} = 0$ | $\frac{-b \pm 0}{2a} = -\frac{b}{2a}$, one repeated root |
| $\Delta < 0$ | $\sqrt{\Delta}$ is not a real number | No real roots |

---

**Example 1**: Determine the nature of the roots of the following equations:
(a) $2x^2 - 3x + 1 = 0$
(b) $4x^2 - 4x + 1 = 0$
(c) $3x^2 + 2x + 5 = 0$

**Detailed solution**:

(a) $\Delta = (-3)^2 - 4(2)(1) = 9 - 8 = 1 > 0$, two distinct real roots.

(b) $\Delta = (-4)^2 - 4(4)(1) = 16 - 16 = 0$, one repeated root.

(c) $\Delta = 2^2 - 4(3)(5) = 4 - 60 = -56 < 0$, no real roots.

---

**Example 2**: The equation $x^2 + kx + 4 = 0$ has a repeated root. Find $k$.

**Detailed solution**:

$\Delta = k^2 - 16 = 0 \Rightarrow k = \pm 4$.

---

**Example 3**: The equation $2x^2 - 3x + k = 0$ has two distinct real roots. Find the range of $k$.

**Detailed solution**:

$\Delta = 9 - 8k > 0 \Rightarrow k < \frac{9}{8}$.

---

**Example 4**: The equation $x^2 - 2x + (k - 3) = 0$ has no real roots. Find the range of $k$.

**Detailed solution**:

$\Delta = (-2)^2 - 4(1)(k - 3) = 4 - 4k + 12 = 16 - 4k < 0 \Rightarrow 4k > 16 \Rightarrow k > 4$.

---

**Example 5**: The equation $kx^2 + 3x + 2 = 0$ has a repeated root. Find the value of $k$.

**Detailed solution**:

Note that $k$ is the coefficient of $x^2$, so $k \neq 0$.

$\Delta = 9 - 8k = 0 \Rightarrow k = \frac{9}{8}$.

---

**Example 6**: The equation $3x^2 - 4x + k = 0$ has two distinct real roots. Find the range of $k$.

**Detailed solution**:

$\Delta = 16 - 12k > 0 \Rightarrow k < \frac{4}{3}$.

---

### 3.2.2 Relative Position of a Line and a Curve

Substitute the line $y = mx + c$ into the curve to eliminate $y$, obtaining a quadratic equation in $x$:

| Value of $\Delta$ | Number of Intersection Points | Relative Position |
|:---:|:---:|:---|
| $\Delta > 0$ | 2 points | Intersect at two points |
| $\Delta = 0$ | 1 point | Tangent (touch) |
| $\Delta < 0$ | 0 points | No intersection |

---

**Example 1**: Determine the relative position of $y = 2x + 1$ and $y = x^2 - 3x + 4$.

After substitution: $x^2 - 5x + 3 = 0$, $\Delta = 25 - 12 = 13 > 0$, intersect at two points.

---

**Example 2**: Find $k$ such that $y = 3x + k$ is tangent to $y = x^2 - x + 2$.

After substitution: $x^2 - 4x + (2 - k) = 0$, $\Delta = 16 - 4(2 - k) = 8 + 4k = 0 \Rightarrow k = -2$.

---

**Example 3**: Find $c$ such that $y = x + c$ does not intersect $y = 2x^2 - 3x + 1$.

After substitution: $2x^2 - 4x + (1 - c) = 0$, $\Delta = 16 - 8(1 - c) = 8 + 8c < 0 \Rightarrow c < -1$.

---

**Example 4**: Find $k$ such that the line $y = 2x + k$ intersects the curve $y = x^2 - 2x + 3$ at two points.

After substitution: $x^2 - 4x + (3 - k) = 0$, $\Delta = 16 - 4(3 - k) = 4 + 4k > 0 \Rightarrow k > -1$.

---

**Example 5**: The line $y = mx + 1$ is tangent to the curve $y = x^2 - 3x + 5$. Find $m$.

After substitution: $x^2 - (m + 3)x + 4 = 0$.

$\Delta = (m + 3)^2 - 16 = 0 \Rightarrow (m + 3)^2 = 16 \Rightarrow m + 3 = \pm 4 \Rightarrow m = 1$ or $m = -7$.

---

**Example 6**: Find $c$ such that the line $y = 5x + c$ is tangent to the curve $y = x^2 + x + 2$.

After substitution: $x^2 + x + 2 = 5x + c \Rightarrow x^2 - 4x + (2 - c) = 0$.

$\Delta = 16 - 4(2 - c) = 8 + 4c = 0 \Rightarrow c = -2$.

---

## 3.3 Solving Quadratic Equations

There are three core methods for solving $ax^2 + bx + c = 0$:

| Method | When to Use | Advantages | Disadvantages |
|:---|:---|:---|:---|
| **Factorisation** | When the expression is easily factorisable | Fastest, exact answer | Not all quadratics are factorisable |
| **Quadratic Formula** | Any situation | Universal, methodical | Slightly more calculation, may involve radicals |
| **Completing the Square** | When vertex form is needed | Gives extreme value information at the same time | Slightly more steps |

---

### 3.3.1 Factorisation Method

**Core principle**: If $A \times B = 0$, then $A = 0$ or $B = 0$.

**For $x^2 + bx + c = 0$ (leading coefficient = 1)**:

Find $p, q$ such that $p + q = b$ and $pq = c$. Then $x^2 + bx + c = (x + p)(x + q)$.

Since $(x + p)(x + q) = x^2 + (p + q)x + pq$.

**For $ax^2 + bx + c = 0$ (leading coefficient ≠ 1)**:

Find $p, q$ such that $pq = ac$ and $p + q = b$. Split the middle term and factor by grouping.

---

**Example 1**: Solve $x^2 - 5x + 6 = 0$.

Find $p+q=-5$, $pq=6$: $(-2)+(-3)=-5$, $(-2)\times(-3)=6$.

$(x-2)(x-3)=0 \Rightarrow x=2$ or $x=3$.

---

**Example 2**: Solve $2x^2 - 5x - 3 = 0$.

$ac = 2\times(-3)=-6$, find $p+q=-5$, $pq=-6$: $(-6)+1=-5$, $(-6)\times1=-6$.

Split: $2x^2-6x+x-3 = 2x(x-3)+1(x-3) = (2x+1)(x-3)$.

$x=-\frac{1}{2}$ or $x=3$.

---

**Example 3**: Solve $3x^2 + 2 = 7x$.

Rearrange: $3x^2 - 7x + 2 = 0$. $ac=6$, $(-6)+(-1)=-7$, $(-6)\times(-1)=6$.

$3x^2-6x-x+2 = 3x(x-2)-1(x-2) = (3x-1)(x-2)$.

$x=\frac{1}{3}$ or $x=2$.

---

**Example 4**: Solve $x^2 + x - 12 = 0$.

Find $p+q=1$, $pq=-12$: $4+(-3)=1$, $4\times(-3)=-12$.

$(x+4)(x-3)=0 \Rightarrow x=-4$ or $x=3$.

---

**Example 5**: Solve $6x^2 - 5x - 6 = 0$.

$ac = 6\times(-6)=-36$, find $p+q=-5$, $pq=-36$: $(-9)+4=-5$, $(-9)\times4=-36$.

$6x^2-9x+4x-6 = 3x(2x-3)+2(2x-3) = (3x+2)(2x-3)$.

$x=-\frac{2}{3}$ or $x=\frac{3}{2}$.

---

**Example 6**: Solve $4x^2 + 4x = 3$.

Rearrange: $4x^2 + 4x - 3 = 0$. $ac = 4\times(-3)=-12$, find $p+q=4$, $pq=-12$: $6+(-2)=4$, $6\times(-2)=-12$.

$4x^2+6x-2x-3 = 2x(2x+3)-1(2x+3) = (2x-1)(2x+3)$.

$x=\frac{1}{2}$ or $x=-\frac{3}{2}$.

---

### 3.3.2 Quadratic Formula

**The Quadratic Formula**:

$$
\boxed{x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}}
$$

**Complete derivation** (by completing the square):

$$
\begin{aligned}
ax^2 + bx + c &= 0 \\
x^2 + \frac{b}{a}x + \frac{c}{a} &= 0 \quad (\text{divide both sides by } a) \\
x^2 + \frac{b}{a}x &= -\frac{c}{a} \quad (\text{rearrange}) \\
x^2 + \frac{b}{a}x + \left(\frac{b}{2a}\right)^2 &= \left(\frac{b}{2a}\right)^2 - \frac{c}{a} \quad (\text{complete the square}) \\
\left(x + \frac{b}{2a}\right)^2 &= \frac{b^2 - 4ac}{4a^2} \\
x + \frac{b}{2a} &= \pm \frac{\sqrt{b^2 - 4ac}}{2a} \\
x &= \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
\end{aligned}
$$

---

**Example 1**: Solve $2x^2 - 3x - 4 = 0$.

$a=2, b=-3, c=-4$.

$$
x = \frac{3 \pm \sqrt{9 + 32}}{4} = \frac{3 \pm \sqrt{41}}{4}
$$

---

**Example 2**: Solve $x^2 - 2x - 3 = 0$.

$$
x = \frac{2 \pm \sqrt{4 + 12}}{2} = \frac{2 \pm 4}{2}
$$

$x=3$ or $x=-1$.

---

**Example 3**: Solve $4x^2 - 12x + 9 = 0$.

$$
x = \frac{12 \pm \sqrt{144 - 144}}{8} = \frac{12}{8} = \frac{3}{2}\ (\text{repeated root})
$$

---

**Example 4**: Solve $x^2 - 3x - 5 = 0$.

$$
x = \frac{3 \pm \sqrt{9 + 20}}{2} = \frac{3 \pm \sqrt{29}}{2}
$$

---

**Example 5**: Solve $3x^2 + 2x - 4 = 0$.

$$
x = \frac{-2 \pm \sqrt{4 + 48}}{6} = \frac{-2 \pm \sqrt{52}}{6} = \frac{-2 \pm 2\sqrt{13}}{6} = \frac{-1 \pm \sqrt{13}}{3}
$$

---

**Example 6**: Solve $5x^2 + 2x - 1 = 0$.

$$
x = \frac{-2 \pm \sqrt{4 + 20}}{10} = \frac{-2 \pm \sqrt{24}}{10} = \frac{-2 \pm 2\sqrt{6}}{10} = \frac{-1 \pm \sqrt{6}}{5}
$$

---

### 3.3.3 Completing the Square

Completing the square rewrites $ax^2 + bx + c$ in the form $a(x + p)^2 + q$.

**Complete derivation**:

$$
\begin{aligned}
ax^2 + bx + c &= a\left(x^2 + \frac{b}{a}x\right) + c \\
&= a\left[x^2 + \frac{b}{a}x + \left(\frac{b}{2a}\right)^2 - \left(\frac{b}{2a}\right)^2\right] + c \\
&= a\left[\left(x + \frac{b}{2a}\right)^2 - \frac{b^2}{4a^2}\right] + c \\
&= a\left(x + \frac{b}{2a}\right)^2 + \left(c - \frac{b^2}{4a}\right)
\end{aligned}
$$

**Final form**:

$$
\boxed{ax^2 + bx + c = a\left(x + \frac{b}{2a}\right)^2 + \frac{4ac - b^2}{4a}}
$$

---

**Example 1**: Solve $x^2 - 6x + 5 = 0$ by completing the square.

$$
\begin{aligned}
x^2 - 6x + 5 &= 0 \\
x^2 - 6x &= -5 \\
x^2 - 6x + 9 &= -5 + 9 \quad (\text{add } (\frac{6}{2})^2=9) \\
(x - 3)^2 &= 4 \\
x - 3 &= \pm 2 \\
x &= 5 \text{ or } x = 1
\end{aligned}
$$

---

**Example 2**: Solve $2x^2 - 8x + 3 = 0$ by completing the square.

$$
\begin{aligned}
2x^2 - 8x + 3 &= 0 \\
2(x^2 - 4x) &= -3 \\
2[(x^2 - 4x + 4) - 4] &= -3 \\
2(x - 2)^2 - 8 &= -3 \\
2(x - 2)^2 &= 5 \\
(x - 2)^2 &= \frac{5}{2} \\
x &= 2 \pm \frac{\sqrt{10}}{2}
\end{aligned}
$$

---

**Example 3**: Write $f(x) = 3x^2 + 12x + 5$ in the form $a(x + p)^2 + q$.

$$
\begin{aligned}
f(x) &= 3x^2 + 12x + 5 \\
&= 3(x^2 + 4x) + 5 \\
&= 3[(x + 2)^2 - 4] + 5 \\
&= 3(x + 2)^2 - 12 + 5 \\
&= 3(x + 2)^2 - 7
\end{aligned}
$$

The vertex is $(-2, -7)$, and since $a=3>0$, the parabola opens upwards.

---

**Example 4**: Solve $x^2 - 8x + 13 = 0$ by completing the square.

$$
\begin{aligned}
x^2 - 8x + 13 &= 0 \\
x^2 - 8x &= -13 \\
x^2 - 8x + 16 &= -13 + 16 \quad (\text{add } (\frac{8}{2})^2=16) \\
(x - 4)^2 &= 3 \\
x - 4 &= \pm \sqrt{3} \\
x &= 4 \pm \sqrt{3}
\end{aligned}
$$

---

**Example 5**: Solve $2x^2 - 8x + 5 = 0$ by completing the square.

$$
\begin{aligned}
2x^2 - 8x + 5 &= 0 \\
2(x^2 - 4x) &= -5 \\
2[(x - 2)^2 - 4] &= -5 \\
2(x - 2)^2 - 8 &= -5 \\
2(x - 2)^2 &= 3 \\
(x - 2)^2 &= \frac{3}{2} \\
x &= 2 \pm \frac{\sqrt{6}}{2}
\end{aligned}
$$

---

**Example 6**: Write $f(x) = -2x^2 + 8x - 5$ in the form $a(x + p)^2 + q$.

$$
\begin{aligned}
f(x) &= -2x^2 + 8x - 5 \\
&= -2(x^2 - 4x) - 5 \\
&= -2[(x - 2)^2 - 4] - 5 \\
&= -2(x - 2)^2 + 8 - 5 \\
&= -2(x - 2)^2 + 3
\end{aligned}
$$

The vertex is $(2, 3)$, and since $a=-2<0$, the parabola opens downwards.

---

### Comparison of Three Methods — Solving the Same Equation with All Three

Solve $x^2 - 4x - 5 = 0$:

**Factorisation** (fastest):
$(x - 5)(x + 1) = 0$, $x = 5$ or $x = -1$.

**Quadratic Formula**:
$x = \frac{4 \pm \sqrt{16 + 20}}{2} = \frac{4 \pm 6}{2}$, $x = 5$ or $x = -1$.

**Completing the Square**:
$(x - 2)^2 = 9$, $x - 2 = \pm 3$, $x = 5$ or $x = -1$.

All three methods give the same result, but factorisation is the quickest — **use factorisation whenever possible**.

---

## 3.4 Completing the Square and Extreme Values

### 3.4.1 Finding Extreme Values by Completing the Square

In $f(x) = a(x + p)^2 + q$, since $(x + p)^2 \geq 0$:
- $a > 0$: $f(x) \geq q$, minimum value $q$ at $x = -p$.
- $a < 0$: $f(x) \leq q$, maximum value $q$ at $x = -p$.

**Why?** Because the minimum value of $(x + p)^2$ is $0$ (when $x = -p$), at which point $f(x) = q$.

---

**Example 1**: Find the minimum value of $f(x) = x^2 - 4x + 7$.

$f(x) = (x - 2)^2 + 3$. $a=1>0$, minimum value $3$ at $x=2$.

---

**Example 2**: Find the maximum value of $f(x) = -2x^2 + 12x - 10$.

$f(x) = -2(x - 3)^2 + 8$. $a=-2<0$, maximum value $8$ at $x=3$.

---

**Example 3**: Find the extreme values of $f(x) = x^2 - 2x - 3$ on $[0, 4]$.

$f(x) = (x - 1)^2 - 4$. The vertex $(1, -4)$ lies within the interval, so minimum is $-4$.
$f(0) = -3$, $f(4) = 5$. Maximum is $5$.

---

**Example 4**: Find the minimum value of $f(x) = x^2 + 6x + 11$.

$f(x) = (x + 3)^2 + 2$. Minimum value $2$ at $x = -3$.

---

**Example 5**: Find the maximum value of $f(x) = -x^2 + 4x + 1$.

$f(x) = -(x - 2)^2 + 5$. Maximum value $5$ at $x = 2$.

---

**Example 6**: Find the range of $f(x) = x^2 - 4x + 5$ on $[1, 5]$.

$f(x) = (x - 2)^2 + 1$, vertex $(2, 1)$ lies within the interval. $f(1)=2$, $f(5)=10$. Range: $[1, 10]$.

---

### 3.4.2 Sketching Graphs

Four key elements: direction of opening, vertex, $x$-intercepts, $y$-intercept.

---

**Example 1**: $f(x) = x^2 - 2x - 3$.
Opens upwards, vertex $(1, -4)$, $x$-intercepts $(-1,0)$ and $(3,0)$, $y$-intercept $(0,-3)$.

**Example 2**: $f(x) = -x^2 + 4x$.
Opens downwards, vertex $(2, 4)$, $x$-intercepts $(0,0)$ and $(4,0)$.

**Example 3**: $f(x) = x^2 + 2x + 3$.
Opens upwards, vertex $(-1, 2)$, $\Delta < 0$ so no $x$-intercepts, $y$-intercept $(0,3)$. Entirely above the $x$-axis.

**Example 4**: $f(x) = -2x^2 + 4x + 6$.
Opens downwards, vertex $(1, 8)$, $x$-intercepts $(-1,0)$ and $(3,0)$, $y$-intercept $(0,6)$.

---

### 3.4.3 Finding the Range

Steps: Complete the square → determine whether the vertex is within the domain → evaluate endpoints → compare.

**Example 1**: $f(x) = 2x^2 - 8x + 3$ on $\mathbb{R}$.
$f(x)=2(x-2)^2-5$, range $[-5,\infty)$.

**Example 2**: $f(x) = x^2 - 2x + 3$ on $[-1,3]$.
$f(x)=(x-1)^2+2$, vertex lies within the interval. $f(1)=2$, $f(-1)=6$, $f(3)=6$, range $[2,6]$.

**Example 3**: $f(x) = x^2 - 4x + 5$ on $[3,5]$.
$f(x)=(x-2)^2+1$, vertex $x=2$ not in the interval, function is increasing. $f(3)=2$, $f(5)=10$, range $[2,10]$.

**Example 4**: $f(x) = -x^2 + 2x + 3$ on $[-1,4]$.
$f(x)=-(x-1)^2+4$, vertex $(1,4)$ lies within the interval. $f(-1)=0$, $f(4)=-5$. Range $[-5,4]$.

---

## 3.5 Quadratic Inequalities

### 3.5.1 Algebraic Method (Sign Table Method)

**Complete steps**:

**Step 1**: Rearrange to $ax^2 + bx + c \;(>/</\geq/\leq)\;0$. If $a < 0$, multiply both sides by $-1$ and reverse the inequality sign.

**Step 2**: Solve the corresponding equation $ax^2 + bx + c = 0$ to obtain roots $x_1 \leq x_2$.

**Step 3**: Write the solution set.

**Sign Rule** (when $a > 0$):

```
Sign:    +      -      +
       ———|—————|—————>
          x₁    x₂
```

- **Greater than → outside**: $ax^2 + bx + c > 0 \Rightarrow x < x_1$ or $x > x_2$
- **Less than → inside**: $ax^2 + bx + c < 0 \Rightarrow x_1 < x < x_2$

**Why does this sign rule hold?**

Because when $a > 0$, the parabola opens upwards. Between the two roots, the parabola lies below the $x$-axis (negative values); outside the two roots, the parabola lies above the $x$-axis (positive values).

**Special cases**:

| $\Delta$ case | $>0$ | $<0$ |
|:---|:---|:---|
| $\Delta = 0$ ($a>0$) | $x \neq x_1$ | No solution |
| $\Delta < 0$ ($a>0$) | $\mathbb{R}$ (all real numbers) | No solution |

---

**Example 1**: Solve $x^2 - 5x + 6 > 0$.

$(x - 2)(x - 3) > 0$. Roots are $x = 2$ and $x = 3$. $a = 1 > 0$.

"Greater than → outside": $x < 2$ or $x > 3$.

Verification: Take $x=0$: $0-0+6=6 > 0$ ✓; take $x=2.5$: $6.25-12.5+6=-0.25 < 0$ ✓.

---

**Example 2**: Solve $2x^2 - 5x - 3 \leq 0$.

$(2x + 1)(x - 3) \leq 0$. Roots are $x = -\frac{1}{2}$ and $x = 3$. $a = 2 > 0$.

"Less than → inside" (including endpoints): $-\frac{1}{2} \leq x \leq 3$.

---

**Example 3**: Solve $x^2 + 2x + 3 > 0$.

$\Delta = 4 - 12 = -8 < 0$, $a = 1 > 0$. Always positive. Solution set: $\mathbb{R}$.

---

**Example 4**: Solve $-x^2 + 3x + 4 > 0$.

$a = -1 < 0$, multiply both sides by $-1$: $x^2 - 3x - 4 < 0$.

$(x - 4)(x + 1) < 0$. Roots are $x = -1$ and $x = 4$.

"Less than → inside": $-1 < x < 4$.

---

**Example 5**: Solve $x^2 - 4x + 4 \geq 0$.

$(x - 2)^2 \geq 0$. A square is always $\geq 0$, so the solution set is $\mathbb{R}$.

---

**Example 6**: Solve $x^2 - 4x + 4 < 0$.

$(x - 2)^2 < 0$. A square can never be less than zero, so **no solution**.

---

### 3.5.2 Graphical Method

Sketch the graph of $y = ax^2 + bx + c$, then look at the parts where the parabola is above the $x$-axis ($> 0$) or below the $x$-axis ($< 0$).

---

**Example 1**: Solve $x^2 - x - 2 < 0$ using the graphical method.

$y = x^2 - x - 2$, $a=1>0$, opens upwards. $x$-intercepts $(-1,0)$ and $(2,0)$.

The graph lies below the $x$-axis for $-1 < x < 2$. Solution set: $-1 < x < 2$.

---

**Example 2**: Given that $x^2 - 2kx + 4 > 0$ holds for all real $x$, find $k$.

$a=1>0$, so we need $\Delta < 0$: $4k^2 - 16 < 0 \Rightarrow k^2 < 4 \Rightarrow -2 < k < 2$.

---

**Example 3**: Solve $x^2 - 4 \geq 3x$.

Rearrange: $x^2 - 3x - 4 \geq 0$. $(x - 4)(x + 1) \geq 0$.

"Greater than → outside" (including endpoints): $x \leq -1$ or $x \geq 4$.

---

**Example 4**: Solve $x^2 - 3x - 10 > 0$.

$(x - 5)(x + 2) > 0$. $x < -2$ or $x > 5$.

---

**Example 5**: Solve $2x^2 + 5x - 3 \leq 0$.

$(2x - 1)(x + 3) \leq 0$. $-3 \leq x \leq \frac{1}{2}$.

---

**Example 6**: Solve $x^2 - 6x + 9 \geq 0$.

$(x - 3)^2 \geq 0$, solution set $\mathbb{R}$.

---

### 3.5.3 Inequalities with Parameters

**Example 1**: Find $k$ such that $x^2 + kx + 9 \geq 0$ holds for all $x$.

$a=1>0$, so we need $\Delta \leq 0$: $k^2 - 36 \leq 0 \Rightarrow -6 \leq k \leq 6$.

---

**Example 2**: Find $k$ such that $kx^2 + 2x + 3 > 0$ holds for all $x$.

If $k = 0$: $2x+3>0$ does not hold for all $x$, so eliminate.
If $k \neq 0$: we need $k > 0$ and $\Delta = 4 - 12k < 0 \Rightarrow k > \frac{1}{3}$.

Therefore $k > \frac{1}{3}$.

---

**Example 3**: Find $k$ such that $x^2 - 2kx + 4 > 0$ holds for all real $x$.

$\Delta = 4k^2 - 16 < 0 \Rightarrow k^2 < 4 \Rightarrow -2 < k < 2$.

---

**Example 4**: Find $k$ such that $(k-1)x^2 + 2x + 1 > 0$ holds for all $x$.

If $k-1 = 0$, i.e., $k=1$: $2x+1 > 0$, does not hold for all $x$.
If $k-1 \neq 0$: need $k-1 > 0$ and $\Delta = 4 - 4(k-1) = 8 - 4k < 0 \Rightarrow k > 2$.

Therefore $k > 2$.

---

## 3.6 Graphs of Cubic Polynomials and Inequalities

### 3.6.1 Graphs of Products of Three Linear Factors

Characteristics of the graph of $f(x) = a(x - p)(x - q)(x - r)$:

**(1) $x$-intercepts**: $x = p, q, r$ (three zeros).

**(2) $y$-intercept**: $f(0) = a(-p)(-q)(-r) = -a \cdot pqr$.

**(3) End behaviour** — determined by the leading term $ax^3$:

When $|x|$ is large, the leading term $ax^3$ dominates:

| Sign of $a$ | $x \to -\infty$ | $x \to +\infty$ |
|:---:|:---:|:---:|
| $a > 0$ | $f(x) \to -\infty$ (bottom-left) | $f(x) \to +\infty$ (top-right) |
| $a < 0$ | $f(x) \to +\infty$ (top-left) | $f(x) \to -\infty$ (bottom-right) |

**(4) Behaviour at zeros**:
- **Simple root** (factor has degree 1): The graph **crosses** the $x$-axis.
- **Double root** (factor has degree 2): The graph **touches and bounces back** (tangent to the $x$-axis).

**Sketching steps**:
1. Mark the $x$-intercepts $p, q, r$.
2. Mark the $y$-intercept.
3. Determine the end behaviour based on the sign of $a$.
4. Connect the points with a smooth S-shaped curve, crossing at simple roots and bouncing at double roots.

---

**Example 1**: Sketch the graph of $f(x) = (x + 1)(x - 1)(x - 3)$.

$x$-intercepts: $x = -1,\;1,\;3$ (three simple roots, all crossed).
$y$-intercept: $f(0) = (1)(-1)(-3) = 3$, passing through $(0, 3)$.
$a = 1 > 0$: left end goes down, right end goes up.

Behaviour: From the third quadrant → crosses $x = -1$ from bottom to top → local maximum → crosses $x = 1$ from top to bottom → local minimum → crosses $x = 3$ from bottom to top → extends to the top-right.

---

**Example 2**: Sketch the graph of $f(x) = -(x + 2)(x - 1)(x - 4)$.

$x$-intercepts: $x = -2,\;1,\;4$.
$y$-intercept: $f(0) = -(2)(-1)(-4) = -8$, passing through $(0, -8)$.
$a = -1 < 0$: left end goes up, right end goes down.

Behaviour: From the second quadrant → crosses $x = -2$ from top to bottom → local minimum → crosses $x = 1$ from bottom to top → local maximum → crosses $x = 4$ from top to bottom → extends to the bottom-right.

---

**Example 3**: Sketch the graph of $f(x) = (x - 1)^2(x + 2)$.

$x$-intercepts: $x = -2$ (simple root, crosses), $x = 1$ (double root, touches and bounces).
$y$-intercept: $f(0) = (1)^2(2) = 2$, passing through $(0, 2)$.
$a = 1 > 0$: left end goes down, right end goes up.

Behaviour: From the third quadrant → crosses $x = -2$ from bottom to top → local maximum → descends to touch the $x$-axis at $x = 1$ and bounces back → extends to the top-right.

---

**Example 4**: Sketch the graph of $f(x) = -(x + 1)(x - 2)^2$.

$x$-intercepts: $x = -1$ (simple root, crosses), $x = 2$ (double root, touches and bounces).
$y$-intercept: $f(0) = -(1)(4) = -4$, passing through $(0, -4)$.
$a = -1 < 0$: left end goes up, right end goes down.

Behaviour: From the second quadrant → crosses $x = -1$ from top to bottom → local minimum → rises to touch the $x$-axis at $x = 2$ and bounces back → extends to the bottom-right.

---

**Example 5**: Sketch the graph of $f(x) = (x + 3)(x + 1)(x - 2)$.

$x$-intercepts: $x = -3,\;-1,\;2$ (three simple roots).
$y$-intercept: $f(0) = (3)(1)(-2) = -6$, passing through $(0, -6)$.
$a = 1 > 0$: left end goes down, right end goes up.

---

**Example 6**: Sketch the graph of $f(x) = -2(x + 1)(x - 1)(x - 3)$.

$x$-intercepts: $x = -1,\;1,\;3$.
$y$-intercept: $f(0) = -2(1)(-1)(-3) = -6$, passing through $(0, -6)$.
$a = -2 < 0$: left end goes up, right end goes down.

---

### 3.6.2 Absolute Value Graphs

**Core rule** (must memorise):

$$
y = |f(x)|
$$

- **Keep** the parts where $f(x) \geq 0$ (parts **above** the $x$-axis remain **unchanged**)
- **Reflect** the parts where $f(x) < 0$ (reflect the parts **below** the $x$-axis **upwards across the $x$-axis**)

In other words: **Negative parts are folded up to the positive side**.

Therefore, in the graph of $y = |f(x)|$:
1. The graph is always **above** (or on) the $x$-axis; there can never be negative values.
2. At the zeros where $f(x) = 0$, the absolute value graph will have **sharp corners (cusps)** (because when the sign changes from positive to negative or vice versa, the slope suddenly reverses direction).
3. The parts of the original function above the $x$-axis remain unchanged; the parts below are "folded" upwards.

---

**Example 1**: Sketch the graph of $y = |(x + 1)(x - 1)(x - 3)|$.

First analyse the sign of $f(x) = (x + 1)(x - 1)(x - 3)$:

| Interval | $x<-1$ | $-1<x<1$ | $1<x<3$ | $x>3$ |
|:---:|:---:|:---:|:---:|:---:|
| $f(x)$ | $-$ | $+$ | $-$ | $+$ |

Reflect the negative parts ($x < -1$ and $1 < x < 3$) upwards across the $x$-axis.

The final graph touches the $x$-axis at $x = -1, 1, 3$ (cusps), and all other parts are above the $x$-axis.

---

**Example 2**: Sketch the graph of $y = |(x - 1)(x - 2)(x - 4)|$.

Analyse the sign of $f(x) = (x - 1)(x - 2)(x - 4)$:

$f(0) = (-1)(-2)(-4) = -8$, so at $x=0$, $f(x) < 0$.

| Interval | $x<1$ | $1<x<2$ | $2<x<4$ | $x>4$ |
|:---:|:---:|:---:|:---:|:---:|
| $f(x)$ | $-$ | $+$ | $-$ | $+$ |

Reflect the negative regions ($x<1$ and $2<x<4$) upwards. Cusps at $x=1,2,4$.

---

**Example 3**: Find the number of real roots of $|(x + 1)(x - 1)(x - 2)| = 2$.

Sign analysis: $x<-1$ ($-$), $-1<x<1$ ($+$), $1<x<2$ ($-$), $x>2$ ($+$).

After the absolute value transformation, $|f(0)| = |(1)(-1)(-2)| = 2$, so $(0,2)$ is an intersection point.

The horizontal line $y=2$ intersects the graph:
- $x<-1$: 1 intersection
- $-1<x<1$: 2 intersections
- $1<x<2$: 2 intersections
- $x>2$: 1 intersection

Total **5 intersections**, meaning the equation has 5 real roots.

---

**Example 4**: Sketch the graph of $y = |(x + 2)(x - 1)^2|$.

$f(x) = (x + 2)(x - 1)^2$.

Sign: $x<-2$ ($-$), $-2<x<1$ ($+$), $x>1$ ($+$).

Reflect the part where $x<-2$ upwards. There is a cusp at $x=-2$; at $x=1$, the graph touches smoothly (double root — the original function does not change sign here, so no reflection is needed).

---

**Example 5**: Sketch the graph of $y = |(x+1)(x-2)(x-5)|$.

Sign: $x<-1$ ($-$), $-1<x<2$ ($+$), $2<x<5$ ($-$), $x>5$ ($+$).

Reflect the $x<-1$ and $2<x<5$ parts. Cusps at $x=-1,2,5$.

---

**Example 6**: Estimate the number of real roots of $|(x+2)(x-1)(x-4)|=3$.

The parts of the graph for $x<-2$ and $1<x<4$ are reflected upwards. The horizontal line $y=3$ intersects the graph at approximately 5 points, giving approximately 5 real roots.

---

### 3.6.3 Graphical Solution of Cubic Inequalities (Syllabus 4.5)

For $f(x) \geq d$ (similarly for $>$, $\leq$, $<$), where $f(x) = a(x-p)(x-q)(x-r)$:

1. Sketch the graph of $y = f(x)$.
2. Draw the horizontal line $y = d$.
3. Find the $x$-coordinates of the intersection points (solve $f(x) = d$).
4. Read off the intervals of $x$ that satisfy the inequality.

**When $d = 0$**, the horizontal line is the $x$-axis, and the problem reduces to analysing the sign of $f(x)$.

---

**Example 1**: $f(x) = (x+1)(x-1)(x-3)$, solve $f(x) \leq 0$.

Sign table:

| Interval | $x<-1$ | $-1<x<1$ | $1<x<3$ | $x>3$ |
|:---:|:---:|:---:|:---:|:---:|
| $f(x)$ | $-$ | $+$ | $-$ | $+$ |

$f(x) \leq 0$ corresponds to intervals where the function is negative or zero (including endpoints):

$$
\boxed{x \leq -1 \quad \text{or} \quad 1 \leq x \leq 3}
$$

---

**Example 2**: $f(x) = -(x+1)(x-2)(x-5)$, solve $f(x) > 0$.

First consider $g(x) = (x+1)(x-2)(x-5)$, $a_g = 1 > 0$.

Sign of $g(x)$: $x<-1$ ($-$), $-1<x<2$ ($+$), $2<x<5$ ($-$), $x>5$ ($+$).

$f(x) = -g(x)$, so the sign of $f(x)$ is the opposite of $g(x)$:

| Interval | $x<-1$ | $-1<x<2$ | $2<x<5$ | $x>5$ |
|:---:|:---:|:---:|:---:|:---:|
| $f(x)$ | $+$ | $-$ | $+$ | $-$ |

$f(x) > 0$ corresponds to positive intervals (excluding endpoints):

$$
\boxed{x < -1 \quad \text{or} \quad 2 < x < 5}
$$

---

**Example 3**: $f(x) = (x+2)(x-1)(x-4)$, solve $f(x) \geq 8$.

Expand: $f(x) = x^3 - 3x^2 - 6x + 8$.

Solve $f(x) = 8$:

$$
x^3 - 3x^2 - 6x + 8 = 8 \Rightarrow x^3 - 3x^2 - 6x = 0 \Rightarrow x(x^2 - 3x - 6) = 0
$$

$x = 0$ or $x = \frac{3 \pm \sqrt{33}}{2}$. $\frac{3 - \sqrt{33}}{2} \approx -1.372$, $\frac{3 + \sqrt{33}}{2} \approx 4.372$.

$a = 1 > 0$, left end goes down, right end goes up. The solution set for $f(x) \geq 8$ is:

$$
\boxed{\frac{3 - \sqrt{33}}{2} \leq x \leq 0 \quad \text{or} \quad x \geq \frac{3 + \sqrt{33}}{2}}
$$

---

**Example 4**: $f(x) = (x+1)(x-2)(x-4)$, solve $f(x) \leq 0$.

Sign: $x<-1$ ($-$), $-1<x<2$ ($+$), $2<x<4$ ($-$), $x>4$ ($+$).

$\leq 0$: $x \leq -1$ or $2 \leq x \leq 4$.

---

**Example 5**: $f(x) = -(x+2)(x-1)(x-5)$, solve $f(x) \geq 0$.

$f(x) \geq 0 \iff -(x+2)(x-1)(x-5) \geq 0 \iff (x+2)(x-1)(x-5) \leq 0$.

Sign: $x<-2$ ($-$), $-2<x<1$ ($+$), $1<x<5$ ($-$), $x>5$ ($+$).

$(x+2)(x-1)(x-5) \leq 0$: $x \leq -2$ or $1 \leq x \leq 5$.

---

**Example 6**: Solve $(x+1)(x-1)(x-3) \geq 4$.

$f(x) = (x+1)(x-1)(x-3) = x^3 - 3x^2 - x + 3$.

$f(x) = 4 \Rightarrow x^3 - 3x^2 - x - 1 = 0$. This cubic is not easy to factorise. In an actual exam, the intersection coordinates would typically be given or solvable with a calculator.

---

## 3.7 Using Differentiation to Find Extreme Values of Quadratic Functions

### 3.7.1 Introduction to the Differentiation Method

Before learning differentiation, we used completing the square to find extreme values. Now, with the tool of differentiation, we can use derivatives to find extreme values, laying the foundation for solving extreme value problems of more complex functions (cubic, exponential, trigonometric, etc.) in the future.

**Core idea**: At an extreme point, the tangent line to the function is horizontal, meaning the slope is zero, i.e., **the derivative is zero**.

For a quadratic function $f(x) = ax^2 + bx + c$:

**Step 1: Differentiate**.

By the Power Rule $(x^n)' = nx^{n-1}$:

$$
f'(x) = \frac{d}{dx}(ax^2 + bx + c) = 2ax + b
$$

**Derivation process**:
- $\frac{d}{dx}(ax^2) = a \cdot 2x = 2ax$
- $\frac{d}{dx}(bx) = b \cdot 1 = b$
- $\frac{d}{dx}(c) = 0$ (the derivative of a constant is zero)

**Step 2: Set the derivative to zero to find the stationary point**.

$$
2ax + b = 0 \;\Rightarrow\; x = -\frac{b}{2a}
$$

This is exactly the $x$-coordinate of the vertex we obtained by completing the square!

**Step 3: Substitute into the original function to find the extreme value**.

$$
\begin{aligned}
f\!\left(-\frac{b}{2a}\right) &= a\left(-\frac{b}{2a}\right)^2 + b\left(-\frac{b}{2a}\right) + c \\
&= a \cdot \frac{b^2}{4a^2} - \frac{b^2}{2a} + c \\
&= -\frac{b^2}{4a} + c = \frac{4ac - b^2}{4a}
\end{aligned}
$$

**Step 4: Use the second derivative to determine the type of extreme value**.

The second derivative is the derivative of the first derivative:

$$
f''(x) = \frac{d}{dx}(2ax + b) = 2a
$$

- $f''(x) = 2a > 0$ (i.e., $a > 0$): **Minimum**. Because $f'' > 0$ means $f'$ is increasing, so $f'$ goes from negative to positive through zero, meaning the function decreases then increases.
- $f''(x) = 2a < 0$ (i.e., $a < 0$): **Maximum**.

---

**Comparison with Completing the Square**:

The differentiation method gives $x = -\frac{b}{2a}$, and completing the square gives $f(x) = a\left(x + \frac{b}{2a}\right)^2 + \frac{4ac-b^2}{4a}$, with the vertex's $x$-coordinate being $-\frac{b}{2a}$ in both cases. The two methods are completely equivalent.

---

**Example 1**: Use differentiation to find the extreme value of $f(x) = 2x^2 - 8x + 5$.

$f'(x) = 4x - 8$. Set $f'(x) = 0$: $4x = 8 \Rightarrow x = 2$.

$f''(x) = 4 > 0$, so it is a minimum.

$f(2) = 8 - 16 + 5 = -3$.

**Verification** (by completing the square): $f(x) = 2(x - 2)^2 - 3$, minimum $-3$. ✓

---

**Example 2**: Use differentiation to find the extreme value of $f(x) = -3x^2 + 12x - 7$.

$f'(x) = -6x + 12$. Set $f'(x) = 0$: $x = 2$.

$f''(x) = -6 < 0$, so it is a maximum.

$f(2) = -12 + 24 - 7 = 5$.

**Verification** (by completing the square): $f(x) = -3(x - 2)^2 + 5$, maximum $5$. ✓

---

**Example 3**: Given that $f(x) = x^2 + kx + 4$ has an extreme value at $x = 3$, find $k$ and determine its type.

$f'(x) = 2x + k$. $f'(3) = 6 + k = 0 \Rightarrow k = -6$.

$f''(x) = 2 > 0$, so it is a minimum.

$f(3) = 9 - 18 + 4 = -5$.

---

**Example 4**: Use differentiation to find the extreme value of $f(x) = 5x^2 - 20x + 3$, and compare with completing the square.

**Differentiation method**: $f'(x) = 10x - 20 = 0 \Rightarrow x = 2$. $f''(x) = 10 > 0$, minimum $f(2) = 20 - 40 + 3 = -17$.

**Completing the square**: $f(x) = 5(x-2)^2 - 17$, minimum $-17$. Both methods agree. ✓

**Comparison**: The differentiation method is more direct and does not require completing the square.

---

**Example 5**: Use differentiation to find the extreme value of $f(x) = -4x^2 + 24x - 31$.

$f'(x) = -8x + 24 = 0 \Rightarrow x = 3$. $f''(x) = -8 < 0$, maximum $f(3) = -36 + 72 - 31 = 5$.

---

**Example 6**: Given that $f(x) = 3x^2 + 2mx + 5$ has an extreme value at $x = -2$, find $m$ and the extreme value.

$f'(x) = 6x + 2m$. $f'(-2) = -12 + 2m = 0 \Rightarrow m = 6$.

$f''(x) = 6 > 0$, minimum. $f(-2) = 12 - 24 + 5 = -7$.

---

**Example 7**: Use differentiation to prove that the minimum value of $f(x) = x^2 + 4x + 7$ is $3$.

$f'(x) = 2x + 4 = 0 \Rightarrow x = -2$. $f''(x) = 2 > 0$, minimum $f(-2) = 4 - 8 + 7 = 3$. QED. ✓

---

**Example 8**: A rectangular garden has a perimeter of $40$ metres. Find the maximum area.

Let the length be $x$ metres, then the width is $20 - x$ metres.

Area $A(x) = x(20 - x) = 20x - x^2 = -x^2 + 20x$.

$A'(x) = -2x + 20 = 0 \Rightarrow x = 10$. $A''(x) = -2 < 0$, maximum.

Maximum area $A(10) = 100$ square metres.

---

**Example 9**: Find the extreme value of $f(x) = 2x^2 - 12x + 5$ and verify by completing the square.

**Differentiation method**: $f'(x) = 4x - 12 = 0 \Rightarrow x = 3$. $f''(x) = 4 > 0$, minimum $f(3) = 18 - 36 + 5 = -13$.

**Verification by completing the square**: $f(x) = 2(x-3)^2 - 13$, minimum $-13$. ✓

---

**Example 10**: Given that $f(x) = ax^2 + 6x + 2$ has an extreme value at $x = -1$, find $a$ and the extreme value.

$f'(x) = 2ax + 6$. $f'(-1) = -2a + 6 = 0 \Rightarrow a = 3$.

$f''(x) = 2a = 6 > 0$, minimum. $f(-1) = 3 - 6 + 2 = -1$.

---

**Example 11**: Use differentiation to find the extreme value of $f(x) = 4x^2 - 16x + 7$.

$f'(x) = 8x - 16 = 0 \Rightarrow x = 2$. $f''(x) = 8 > 0$, minimum $f(2) = 16 - 32 + 7 = -9$.

---

**Example 12**: Use differentiation to find the extreme value of $f(x) = -5x^2 + 30x - 41$.

$f'(x) = -10x + 30 = 0 \Rightarrow x = 3$. $f''(x) = -10 < 0$, maximum $f(3) = -45 + 90 - 41 = 4$.

---

**Example 13**: Given that $f(x) = 2x^2 + kx + 3$ has an extreme value at $x = -2$, find $k$ and the extreme value.

$f'(x) = 4x + k$. $f'(-2) = -8 + k = 0 \Rightarrow k = 8$.

$f''(x) = 4 > 0$, minimum. $f(-2) = 8 - 16 + 3 = -5$.

---

**Example 14**: Given that $f(x) = -3x^2 + mx + 1$ has an extreme value at $x = 1$, find $m$ and the extreme value.

$f'(x) = -6x + m$. $f'(1) = -6 + m = 0 \Rightarrow m = 6$.

$f''(x) = -6 < 0$, maximum. $f(1) = -3 + 6 + 1 = 4$.

---

**Example 15**: Use both differentiation and completing the square to find the extreme value of $f(x) = 3x^2 - 18x + 25$, and compare the two methods.

**Differentiation method**: $f'(x) = 6x - 18 = 0 \Rightarrow x = 3$. $f''(x) = 6 > 0$, minimum $f(3) = 27 - 54 + 25 = -2$.

**Completing the square**: $f(x) = 3(x^2 - 6x) + 25 = 3[(x-3)^2 - 9] + 25 = 3(x-3)^2 - 27 + 25 = 3(x-3)^2 - 2$. Minimum $-2$ at $x=3$. ✓

**Comparison**: Differentiation requires only three steps (differentiate → set to zero → second derivative), while completing the square requires algebraic manipulation. For quadratic functions, both are equally manageable, but for more complex functions, differentiation is more advantageous.

---

## Chapter Summary

| Topic | Core Content |
|:---|:---|
| **Remainder Theorem** | Remainder when $f(x) \div (x-a)$ is $f(a)$; $f(x) \div (ax+b)$ has remainder $f(-b/a)$ |
| **Factor Theorem** | $f(a)=0 \iff (x-a)$ is a factor |
| **Cubic factorisation procedure** | Test roots → Synthetic division → Factorise quadratic |
| **Synthetic division** | Division format using only coefficients, more concise than long division |
| **Discriminant $\Delta$** | $\Delta = b^2-4ac$; $\Delta>0$ two distinct roots, $\Delta=0$ repeated root, $\Delta<0$ no real roots |
| **Line and curve** | Substitute to eliminate $y$ → quadratic → $\Delta$ determines intersect/tangent/no intersection |
| **Three methods for solving quadratics** | Factorisation (fastest), Quadratic formula (universal), Completing the square (vertex form) |
| **Extreme values** | $a(x+p)^2+q$, $a>0$ minimum $q$, $a<0$ maximum $q$ |
| **Quadratic inequalities** | When $a>0$: "greater than → outside, less than → inside" |
| **Cubic graphs** | $a>0$ bottom-left to top-right, $a<0$ top-left to bottom-right; simple root crosses, double root bounces |
| **Absolute value graphs** | Negative parts reflected upwards across the $x$-axis, cusps at zeros |
| **Cubic inequalities** | Sketch graph → draw horizontal line $y=d$ → read intervals |
| **Differentiation for extreme values** | $f'(x)=0$ gives stationary point, $f''(x)$ determines max/min |

---

## Practice Problems

**1. Remainder Theorem**:
(a) Find the remainder when $f(x) = 5x^3 - 4x^2 + 3x - 2$ is divided by $x - 2$.
(b) The polynomial $f(x) = 2x^3 + kx^2 - 3x + 1$ has remainder $15$ when divided by $x + 2$. Find $k$.
(c) Find the remainder when $f(x) = 8x^3 - 6x^2 + 4x - 1$ is divided by $2x - 3$.

**2. Factor Theorem**:
(a) Show that $(x + 2)$ is a factor of $f(x) = x^3 + 3x^2 - 4x - 12$.
(b) The polynomial $f(x) = 3x^3 + ax^2 + bx - 10$ has factors $(x - 2)$ and $(x + 1)$. Find $a$ and $b$.
(c) Given that $x - 3$ is a factor of $f(x) = 2x^3 - 5x^2 + kx - 6$, find $k$.

**3. Factorising Cubic Polynomials**:
(a) $x^3 - 3x^2 - 10x + 24$
(b) $3x^3 + 2x^2 - 7x + 2$
(c) $4x^3 - 12x^2 - x + 3$

**4. Solving Cubic Equations**:
(a) $x^3 - 2x^2 - 5x + 6 = 0$
(b) $2x^3 - 3x^2 - 3x + 2 = 0$
(c) Given that $x = -3$ is a root of $x^3 + 3x^2 - 4x + k = 0$, find $k$ and solve the equation.

**5. Discriminant**:
(a) Determine the nature of the roots of $2x^2 - 5x + 4 = 0$.
(b) The equation $x^2 - 6x + k = 0$ has a repeated root. Find $k$.
(c) The equation $3x^2 + kx + 3 = 0$ has no real roots. Find the range of $k$.

**6. Line and Curve**:
(a) Determine the relative position of $y = 4x - 3$ and $y = x^2 - x + 2$.
(b) Find $k$ such that $y = 2x + k$ is tangent to $y = x^2 - 4x + 7$.
(c) Find $m$ such that $y = mx - 1$ intersects $y = x^2 - 2x + 4$ at two points.

**7. Solving Quadratic Equations**:
(a) $x^2 - 7x + 12 = 0$ (by factorisation)
(b) $3x^2 + 5x - 2 = 0$ (by factorisation)
(c) $2x^2 - 4x - 3 = 0$ (by quadratic formula)
(d) $x^2 - 8x + 13 = 0$ (by completing the square)
(e) $5x^2 + 2x - 1 = 0$ (by quadratic formula)
(f) $2x^2 - 8x + 5 = 0$ (by completing the square)

**8. Extreme Values and Range**:
(a) Find the minimum value of $f(x) = x^2 + 8x + 19$.
(b) Find the maximum value of $f(x) = -2x^2 + 8x - 3$.
(c) Find the range of $f(x) = x^2 - 6x + 10$ on $[1, 5]$.
(d) Find the range of $f(x) = -x^2 + 2x + 3$ on $[-1, 4]$.

**9. Quadratic Inequalities**:
(a) $x^2 - 3x - 10 > 0$
(b) $2x^2 - 7x + 3 \leq 0$
(c) $-x^2 + 5x - 6 \geq 0$
(d) Find $k$ such that $x^2 + kx + 16 > 0$ holds for all real $x$.

**10. Cubic Graphs**:
(a) Sketch the graph of $f(x) = (x - 1)(x - 3)(x - 5)$, labelling the intercepts.
(b) Sketch the graph of $f(x) = -(x + 2)(x - 1)(x - 3)$, labelling the intercepts.
(c) Sketch the graph of $f(x) = (x + 1)^2(x - 4)$, labelling the intercepts and bounce point.
(d) Sketch the graph of $y = |(x + 1)(x - 1)(x - 5)|$.
(e) Estimate the number of real roots of $|(x + 2)(x - 1)(x - 4)| = 3$.

**11. Cubic Inequalities**:
(a) Solve $(x + 1)(x - 2)(x - 4) \leq 0$.
(b) Solve $-(x + 2)(x - 1)(x - 5) > 0$.
(c) Solve $(x + 1)(x - 1)(x - 3) \geq 4$.

**12. Differentiation for Extreme Values**:
(a) Use differentiation to find the extreme value of $f(x) = 4x^2 - 16x + 7$.
(b) Use differentiation to find the extreme value of $f(x) = -5x^2 + 30x - 41$.
(c) Given that $f(x) = 2x^2 + kx + 3$ has an extreme value at $x = -2$, find $k$ and the extreme value.
(d) Given that $f(x) = -3x^2 + mx + 1$ has an extreme value at $x = 1$, find $m$ and the extreme value.
(e) Use differentiation to prove that the minimum value of $f(x) = x^2 - 10x + 28$ is $3$.
(f) Use both differentiation and completing the square to find the extreme value of $f(x) = 3x^2 - 18x + 25$, and compare the two methods.

---

<details>
<summary><strong>Click to view all answers</strong></summary>

**1. Remainder Theorem**:
(a) $f(2) = 5(8) - 4(4) + 3(2) - 2 = 40 - 16 + 6 - 2 = 28$.
(b) $f(-2) = 2(-8) + k(4) - 3(-2) + 1 = -16 + 4k + 6 + 1 = 4k - 9 = 15 \Rightarrow k = 6$.
(c) $x = \frac{3}{2}$: $f(\frac{3}{2}) = 8(\frac{27}{8}) - 6(\frac{9}{4}) + 4(\frac{3}{2}) - 1 = 27 - \frac{27}{2} + 6 - 1 = \frac{54 - 27 + 12 - 2}{2} = \frac{37}{2}$.

**2. Factor Theorem**:
(a) $f(-2) = -8 + 12 + 8 - 12 = 0$, therefore $(x+2)$ is a factor of $f(x)$. ✓
(b) $f(2) = 24 + 4a + 2b - 10 = 14 + 4a + 2b = 0 \Rightarrow 2a + b = -7$; $f(-1) = -3 + a - b - 10 = -13 + a - b = 0 \Rightarrow a - b = 13$. Solving gives $a = 2$, $b = -11$.
(c) $f(3) = 54 - 45 + 3k - 6 = 3 + 3k = 0 \Rightarrow k = -1$.

**3. Factorising Cubic Polynomials**:
(a) $f(2) = 8 - 12 - 20 + 24 = 0$. Synthetic division gives $x^2 - x - 12 = (x - 4)(x + 3)$. $f(x) = (x - 2)(x - 4)(x + 3)$.
(b) $f(1) = 3 + 2 - 7 + 2 = 0$. Synthetic division gives $3x^2 + 5x - 2 = (3x - 1)(x + 2)$. $f(x) = (x - 1)(3x - 1)(x + 2)$.
(c) $f(3) = 108 - 108 - 3 + 3 = 0$. Synthetic division gives $4x^2 - 1 = (2x + 1)(2x - 1)$. $f(x) = (x - 3)(2x + 1)(2x - 1)$.

**4. Solving Cubic Equations**:
(a) $f(1) = 0$, factorising gives $(x - 1)(x + 2)(x - 3) = 0$, solutions: $x = 1, -2, 3$.
(b) $f(-1) = 0$, factorising gives $(x + 1)(2x - 1)(x - 2) = 0$, solutions: $x = -1, \frac{1}{2}, 2$.
(c) $f(-3) = -27 + 27 + 12 + k = 12 + k = 0 \Rightarrow k = -12$. Equation: $x^3 + 3x^2 - 4x - 12 = 0$, factorising gives $(x + 3)(x + 2)(x - 2) = 0$, solutions: $x = -3, -2, 2$.

**5. Discriminant**:
(a) $\Delta = 25 - 32 = -7 < 0$, no real roots.
(b) $\Delta = 36 - 4k = 0 \Rightarrow k = 9$.
(c) $\Delta = k^2 - 36 < 0 \Rightarrow -6 < k < 6$.

**6. Line and Curve**:
(a) Substituting gives $x^2 - 5x + 5 = 0$, $\Delta = 25 - 20 = 5 > 0$, intersect at two points.
(b) Substituting gives $x^2 - 6x + (7 - k) = 0$, $\Delta = 36 - 4(7 - k) = 8 + 4k = 0 \Rightarrow k = -2$.
(c) Substituting gives $x^2 - (m + 2)x + 5 = 0$, $\Delta = (m+2)^2 - 20 > 0 \Rightarrow m < -2 - 2\sqrt{5}$ or $m > -2 + 2\sqrt{5}$.

**7. Solving Quadratic Equations**:
(a) $(x - 3)(x - 4) = 0$, $x = 3$ or $x = 4$.
(b) $(3x - 1)(x + 2) = 0$, $x = \frac{1}{3}$ or $x = -2$.
(c) $x = \frac{4 \pm \sqrt{16 + 24}}{4} = \frac{4 \pm \sqrt{40}}{4} = \frac{4 \pm 2\sqrt{10}}{4} = \frac{2 \pm \sqrt{10}}{2}$.
(d) $(x - 4)^2 = 3$, $x = 4 \pm \sqrt{3}$.
(e) $x = \frac{-2 \pm \sqrt{4 + 20}}{10} = \frac{-2 \pm \sqrt{24}}{10} = \frac{-2 \pm 2\sqrt{6}}{10} = \frac{-1 \pm \sqrt{6}}{5}$.
(f) $2(x - 2)^2 = 3$, $(x - 2)^2 = \frac{3}{2}$, $x = 2 \pm \frac{\sqrt{6}}{2}$.

**8. Extreme Values and Range**:
(a) $f(x) = (x + 4)^2 + 3$, minimum $3$.
(b) $f(x) = -2(x - 2)^2 + 5$, maximum $5$.
(c) $f(x) = (x - 3)^2 + 1$, vertex $x=3$ lies within $[1,5]$, $f(3)=1$, $f(1)=5$, $f(5)=5$, range $[1,5]$.
(d) $f(x) = -(x - 1)^2 + 4$, vertex $x=1$ lies within $[-1,4]$, $f(1)=4$, $f(-1)=0$, $f(4)=-5$, range $[-5,4]$.

**9. Quadratic Inequalities**:
(a) $(x - 5)(x + 2) > 0$, $x < -2$ or $x > 5$.
(b) $(2x - 1)(x - 3) \leq 0$, $\frac{1}{2} \leq x \leq 3$.
(c) Multiply by $-1$: $x^2 - 5x + 6 \leq 0$, $(x - 2)(x - 3) \leq 0$, $2 \leq x \leq 3$.
(d) $\Delta = k^2 - 64 < 0 \Rightarrow -8 < k < 8$.

**10. Cubic Graphs**:
(a) $x$-intercepts $1,3,5$, $y$-intercept $(-1)(-3)(-5) = -15$, $a>0$ bottom-left to top-right.
(b) $x$-intercepts $-2,1,3$, $y$-intercept $-(2)(-1)(-3) = 6$, $a<0$ top-left to bottom-right.
(c) $x$-intercepts: $-1$ (double root, bounce), $4$ (simple root, cross), $y$-intercept $(1)^2(-4) = -4$, $a>0$ bottom-left to top-right.
(d) $f(x)$ negative for $x<-1$, positive for $-1<x<1$, negative for $1<x<5$, positive for $x>5$. Reflect $x<-1$ and $1<x<5$ parts upwards.
(e) Approximately 5 real roots.

**11. Cubic Inequalities**:
(a) Sign: $x<-1$ ($-$), $-1<x<2$ ($+$), $2<x<4$ ($-$), $x>4$ ($+$). $\leq 0$: $x \leq -1$ or $2 \leq x \leq 4$.
(b) $f(x) > 0$: $x<-2$ or $1<x<5$.
(c) Need to solve $x^3 - 3x^2 - x - 1 = 0$. Non-integer roots — in an exam the intersection points would be given or solved with a calculator.

**12. Differentiation for Extreme Values**:
(a) $f'(x) = 8x - 16 = 0 \Rightarrow x = 2$, $f''(x) = 8 > 0$, minimum $f(2) = 16 - 32 + 7 = -9$.
(b) $f'(x) = -10x + 30 = 0 \Rightarrow x = 3$, $f''(x) = -10 < 0$, maximum $f(3) = -45 + 90 - 41 = 4$.
(c) $f'(x) = 4x + k$, $f'(-2) = -8 + k = 0 \Rightarrow k = 8$. $f''(x) = 4 > 0$, minimum $f(-2) = 8 - 16 + 3 = -5$.
(d) $f'(x) = -6x + m$, $f'(1) = -6 + m = 0 \Rightarrow m = 6$. $f''(x) = -6 < 0$, maximum $f(1) = -3 + 6 + 1 = 4$.
(e) $f'(x) = 2x - 10 = 0 \Rightarrow x = 5$, $f''(x) = 2 > 0$, minimum $f(5) = 25 - 50 + 28 = 3$. QED. ✓
(f) **Differentiation method**: $f'(x) = 6x - 18 = 0 \Rightarrow x = 3$, $f''(x) = 6 > 0$, minimum $f(3) = 27 - 54 + 25 = -2$.
**Completing the square**: $f(x) = 3(x^2 - 6x) + 25 = 3[(x - 3)^2 - 9] + 25 = 3(x - 3)^2 - 27 + 25 = 3(x - 3)^2 - 2$. Minimum $-2$ at $x=3$. ✓
**Comparison**: Differentiation requires only three steps (differentiate → set to zero → second derivative), while completing the square requires algebraic manipulation. For quadratic functions, both are equally manageable, but for more complex functions, differentiation is more advantageous.

</details>

---
---
# Chapter 4: Functions (Linear, Cubic, Exponential, Logarithmic)

## Syllabus Mapping

This chapter covers all content from **Topic 1: Functions** and **Topic 6: Logarithmic and Exponential Functions** of the IGCSE 0606 Additional Mathematics (2028–2030) syllabus.

| Syllabus Ref | Corresponding Section |
|---------|---------|
| **1.1** Understand functions (including vertical line test), domain, range, one-one (horizontal line test), many-one, inverse functions, composite functions; explain whether a relation is a function | §4.1, §4.4 |
| **1.2** Find the domain and range of functions (including inverse and composite functions); understand domain restrictions for the existence of inverse/composite functions; understand $\text{Domain}(gf) \subseteq \text{Domain}(f)$, $\text{Range}(gf) \subseteq \text{Range}(g)$ | §4.1, §4.4 |
| **1.3** Recognise and use function notation: $f(x)$, $f:x \mapsto$, $f^{-1}(x)$, $fg(x)$, $f^2(x)$ ($f^2$ not used for trigonometric functions) | §4.1 |
| **1.4** Understand the relationship between $y=f(x)$ and $y=|f(x)|$, where $f(x)$ can be linear, quadratic, cubic or trigonometric (of the form $a\sin bx+c$, $a\cos bx+c$, $a\tan bx+c$) | §4.5 |
| **1.5** Explain in words why a given function does not have an inverse | §4.4 |
| **1.6** Find the inverse of a one-one function (e.g., inverse of $f(x)=e^{2x}$ is $\frac12\ln x$) | §4.4 |
| **1.7** Construct and use composite functions, understanding that $fg$ is generally not equal to $gf$ | §4.4 |
| **1.8** Sketch the relationship between a function and its inverse being symmetrical about $y=x$ | §4.4 |
| **6.1** Know and use the properties and graphs of logarithmic and exponential functions (including $\ln x$ and $e^x$, asymptotes) | §4.3 |
| **6.2** Know and use the laws of logarithms (including the change of base formula) | §4.3 |
| **6.3** Solve equations of the form $a^x = b$ | §4.3 |

> **Learning path**: §4.1 (Conceptual foundations) → §4.2 (Linear and cubic) → §4.3 (Exponential and logarithmic) → §4.4 (Inverse and composite) → §4.5 (Absolute value graphs) → Practice problems

---

## 4.1 Fundamental Concepts of Functions

### 4.1.1 What is a Function?

A function is a special type of relation: it maps **each** input value $x$ in the **domain** to **exactly one** output value $y = f(x)$. We say $y$ is the **image** of $x$.

$$
f: D \to \mathbb{R}, \quad x \mapsto f(x)
$$

where $D$ is the domain, and the **range (image set)** is the set of all possible output values $f(x)$.

**Required condition for a function**: For every $x$ in the domain, there must be one and only one corresponding $y$. This is the **vertical line test** — any vertical line intersects the graph of a function at most once.

**How to explain whether a relation is a function** (Syllabus 1.1):

For each value of $x$ in the domain, the relation gives exactly one value of $y$.

- $y = x^2$ **is** a function: each $x$ corresponds to exactly one $y$.
- $x = y^2$ **is not** a function: e.g., when $x=4$, $y$ can be $2$ or $-2$, one $x$ corresponds to two $y$'s.
- $y = \pm\sqrt{x}$ **is not** a function: each positive $x$ corresponds to two $y$ values.

### 4.1.2 One–One (Injective) and Many–One Functions

- **One–one function (injective)**: Different $x$ values in the domain correspond to different $y$ values. That is: if $x_1 \neq x_2$, then $f(x_1) \neq f(x_2)$. Test method — **horizontal line test**: any horizontal line intersects the graph at most once.

- **Many–one function**: Different $x$ values can correspond to the same $y$ value. For example $f(x) = x^2$, $f(2) = f(-2) = 4$. The horizontal line $y=4$ intersects the graph at two points.

> ⚠️ **Only one–one functions have inverses**. This is because the inverse function needs to uniquely map each output value back to an input value — if the original function is many–one, the inverse would be one–many, which violates the definition of a function.

### 4.1.3 Function Notation

Function notation used in IGCSE 0606 includes:

- **$f(x)$**: The most common notation, e.g., $f(x) = 2e^x$
- **$f: x \mapsto$**: Mapping notation, e.g., $f: x \mapsto \lg x$, meaning "$f$ maps $x$ to $\lg x$"
- **$f^{-1}(x)$**: Inverse function notation
- **$fg(x)$**: Composite function notation, $fg(x) = f(g(x))$
- **$f^2(x)$**: Denotes $f(f(x))$, i.e., $f$ composed with itself

> ⚠️ **Important**: The notation $f^2(x)$ **does not apply to trigonometric functions**. For example, $\sin^2 x$ means $(\sin x)^2$, not $\sin(\sin x)$.

### 4.1.4 Finding Domain and Range

Restrictions to consider when finding the domain:

1. **Denominator not zero**: $f(x) = \dfrac{1}{g(x)} \Rightarrow g(x) \neq 0$
2. **Even root radicand non-negative**: $f(x) = \sqrt{g(x)} \Rightarrow g(x) \geq 0$
3. **Logarithm argument positive**: $f(x) = \log_a(g(x)) \Rightarrow g(x) > 0$

**Methods for finding range**:

**Method 1 — Completing the square** (for quadratic functions):
Write $f(x) = ax^2 + bx + c$ in the form $a(x-h)^2 + k$.
- If $a > 0$, minimum is $k$, range is $[k, \infty)$
- If $a < 0$, maximum is $k$, range is $(-\infty, k]$

**Method 2 — Observation** (for monotonic functions):
If the function is strictly increasing or decreasing on its domain, the range is the interval between the function values at the endpoints.

**Method 3 — Inverse function method**:
If the function has an inverse, the range of the original function equals the domain of the inverse.

---

### Worked Examples 4.1 (Domain and Range)

**Example 1** (Basic — root and denominator): Find the domain of $f(x) = \sqrt{x-2} + \dfrac{1}{x-3}$.

**Solution**:

**Step 1** (root condition): $x-2 \geq 0 \Rightarrow x \geq 2$.

**Step 2** (denominator condition): $x-3 \neq 0 \Rightarrow x \neq 3$.

**Step 3** (intersection): Domain is $[2, 3) \cup (3, \infty)$.

---

**Example 2** (Composite — separating constant to find range): Function $f(x) = \dfrac{2x+1}{x-1}$, $x \neq 1$.

(i) Find the range;
(ii) Determine whether $f$ is one–one.

**Solution**:

(i) **Separate the constant**: Rewrite the numerator in terms of the denominator.

$$
f(x) = \frac{2x+1}{x-1} = \frac{2(x-1) + 3}{x-1}
$$

The idea: the denominator is $x-1$, we want $x-1$ in the numerator to simplify. Write $2x$ as $2(x-1) + 2$, plus the $1$ from the original numerator, giving $2(x-1) + 3$.

Continuing:

$$
f(x) = \frac{2(x-1)}{x-1} + \frac{3}{x-1} = 2 + \frac{3}{x-1}
$$

Since $\dfrac{3}{x-1} \neq 0$ for all $x \neq 1$, $f(x)$ can never equal $2$.

**Range is $\mathbb{R} \setminus \{2\}$**.

(ii) Check one–one: Suppose $f(a) = f(b)$:

$$
2 + \frac{3}{a-1} = 2 + \frac{3}{b-1}
$$

Subtract 2 from both sides:

$$
\frac{3}{a-1} = \frac{3}{b-1}
$$

Take reciprocals: $a-1 = b-1 \Rightarrow a = b$.

Therefore $f$ is one–one. Geometrically, $y = 2 + \dfrac{3}{x-1}$ is a reciprocal function after translation; each horizontal line (except $y=2$) intersects exactly once.

---

**Example 3** (Semi-circular range): Given $f(x) = \sqrt{4 - x^2}$.

(i) Find the domain and range;
(ii) Determine whether $f$ has an inverse.

**Solution**:

(i) **Domain**: $4 - x^2 \geq 0 \Rightarrow x^2 \leq 4 \Rightarrow -2 \leq x \leq 2$. Domain is $[-2, 2]$.

**Range**: Let $y = \sqrt{4 - x^2}$, then $y \geq 0$ and $y^2 = 4 - x^2$, i.e., $x^2 + y^2 = 4$ ($y \geq 0$).

This is the **upper semicircle** with centre at the origin and radius $2$. The minimum $y$ occurs at $x = \pm 2$, $y = 0$; the maximum occurs at $x = 0$, $y = 2$. Therefore the range is $[0, 2]$.

(ii) $f$ is not one–one because e.g., $f(-1) = f(1) = \sqrt{3}$. The horizontal line $y = \sqrt{3}$ intersects the upper semicircle at $(\pm 1, \sqrt{3})$, two points. Therefore $f$ has no inverse.

> However, if we restrict the domain to $x \in [0, 2]$, $f$ becomes one–one, and its inverse is $f^{-1}(x) = \sqrt{4 - x^2}$ (domain $[0, 2]$).

---

**Example 4** (Logarithm and fraction composite domain): Find the domain of $f(x) = \ln(3x - 6) + \dfrac{1}{\sqrt{8 - 2x}}$.

**Solution**:

**Condition 1** (logarithm argument > 0): $3x - 6 > 0 \Rightarrow x > 2$.

**Condition 2** (denominator radicand > 0 — since denominator cannot be zero and the root is in the denominator): $8 - 2x > 0 \Rightarrow x < 4$.

**Intersection**: $x > 2$ and $x < 4$, i.e., $(2, 4)$.

---

**Example 5** (Determining whether a relation is a function — Syllabus 1.1 requirement): Determine whether each relation is a function, and explain why.

(i) $y = \pm \sqrt{x}$, $x \geq 0$
(ii) $y = x^3 - 2x + 1$
(iii) $x^2 + y^2 = 25$

**Solution**:

(i) **Not a function**. For the same $x$ (e.g., $x=4$), the relation gives two $y$ values: $y = 2$ and $y = -2$. This violates the definition that **each input corresponds to exactly one output**. The vertical line $x=4$ intersects the graph at two points.

(ii) **Is a function**. For every real number $x$, $x^3 - 2x + 1$ computes exactly one real number $y$. The vertical line test passes at every $x$.

(iii) **Not a function**. For example, when $x=0$, $y^2 = 25 \Rightarrow y = \pm 5$, one $x$ corresponds to two $y$ values. The vertical line $x=0$ intersects the circle at $(0,5)$ and $(0,-5)$, two points.

---

## 4.2 Linear Functions and Cubic Functions

### 4.2.1 Linear Functions $f(x) = mx + c$

Linear functions are the simplest type of function. Their graph is a straight line.

**Geometric meaning of slope $m$**: For each $1$ unit increase in $x$, $y$ increases by $m$ units. If $m > 0$, the line slopes upward to the right; $m < 0$, slopes downward to the right; $m = 0$, horizontal line.

**Intercept $c$**: The $y$-coordinate of the point where the line crosses the $y$-axis, i.e., the value of $f(0)$.

**Rate of change characteristic**: The rate of change of a linear function is **constant** — at any point, the instantaneous rate of change equals $m$. This is the most important property that distinguishes linear functions from other types.

Finding slope from two points $(x_1, y_1)$ and $(x_2, y_2)$:

$$
m = \frac{y_2 - y_1}{x_2 - x_1}
$$

The reasoning: the vertical change between the two points is $y_2 - y_1$, the horizontal change is $x_2 - x_1$, and the slope is the "rise over run."

**Point-slope form**: The equation of a line through point $(x_0, y_0)$ with slope $m$ is:

$$
y - y_0 = m(x - x_0)
$$

### 4.2.2 Cubic Functions $f(x) = ax^3 + bx^2 + cx + d$ ($a \neq 0$)

The graph of a cubic function has an S-shape (or inverted S-shape). Its derivative $f'(x) = 3ax^2 + 2bx + c$ is a quadratic function, which may have two zeros (corresponding to local extreme points), or only one, or no real zeros.

**Two basic forms of cubic functions**:

1. **Product of three linear factors**: $f(x) = a(x - p)(x - q)(x - r)$, intersecting the $x$-axis at $x = p, q, r$.
2. **Product of one linear factor and one quadratic factor**: $f(x) = (x - p)(Ax^2 + Bx + C)$, which may have only one real root.

**End behaviour (leading term test)**:
- If $a > 0$: as $x \to -\infty$, $f(x) \to -\infty$; as $x \to \infty$, $f(x) \to \infty$.
- If $a < 0$: as $x \to -\infty$, $f(x) \to \infty$; as $x \to \infty$, $f(x) \to -\infty$.

---

### Worked Examples 4.2 (Linear and Cubic Functions)

**Example 1** (Linear function parameter finding): Line $L$ passes through points $A(2, 5)$ and $B(4, 11)$.

(i) Find the equation of $L$;
(ii) Find the $x$-intercept and $y$-intercept of $L$.

**Solution**:

(i) **Find the slope**:

$$
m = \frac{11 - 5}{4 - 2} = \frac{6}{2} = 3
$$

**Write the equation**: Using point-slope form with $A(2, 5)$:

$$
y - 5 = 3(x - 2)
$$

Simplifying:

$$
y - 5 = 3x - 6 \Rightarrow y = 3x - 1
$$

(ii) **$y$-intercept**: Set $x = 0$, $y = 3(0) - 1 = -1$, i.e., $(0, -1)$.

**$x$-intercept**: Set $y = 0$, $0 = 3x - 1 \Rightarrow x = \dfrac{1}{3}$, i.e., $\left(\dfrac{1}{3}, 0\right)$.

---

**Example 2** (Cubic function graph and extreme values): Given $f(x) = x^3 - 3x^2 + 2$.

(i) Find $f'(x)$ and solve $f'(x) = 0$;
(ii) Determine the type of stationary points;
(iii) Find the intercepts of $f$ with the coordinate axes.

**Solution**:

(i) **Differentiate**:

$$
f'(x) = \frac{d}{dx}(x^3) - \frac{d}{dx}(3x^2) + \frac{d}{dx}(2) = 3x^2 - 6x
$$

Factorise: $f'(x) = 3x(x - 2)$.

Set $f'(x) = 0$: $3x(x-2) = 0$, giving $x = 0$ or $x = 2$.

(ii) Use the first derivative sign test to check monotonicity around each stationary point:

**At $x = 0$**:
- Take $x = -1$ (to the left): $f'(-1) = 3(-1)(-3) = 9 > 0$, increasing
- Take $x = 1$ (to the right): $f'(1) = 3(1)(-1) = -3 < 0$, decreasing
- Left to right: increasing → decreasing → **local maximum**. $f(0) = 2$.

**At $x = 2$**:
- Take $x = 1$ (to the left): $f'(1) = -3 < 0$, decreasing
- Take $x = 3$ (to the right): $f'(3) = 3(3)(1) = 9 > 0$, increasing
- Left to right: decreasing → increasing → **local minimum**. $f(2) = 8 - 12 + 2 = -2$.

(iii) **$y$-intercept**: $f(0) = 2$, i.e., $(0, 2)$.

**$x$-intercept**: Solve $x^3 - 3x^2 + 2 = 0$.

Try rational roots. Test $x = 1$: $f(1) = 1 - 3 + 2 = 0$, so $x-1$ is a factor.

Factorise by synthetic division:

$$
\begin{array}{c|ccc}
1 & 1 & -3 & 0 & 2 \\
  &   & 1  & -2 & -2 \\
\hline
  & 1 & -2 & -2 & 0
\end{array}
$$

The quotient is $x^2 - 2x - 2$. Use the quadratic formula:

$$
x = \frac{2 \pm \sqrt{4 - 4(1)(-2)}}{2(1)} = \frac{2 \pm \sqrt{4 + 8}}{2} = \frac{2 \pm \sqrt{12}}{2} = \frac{2 \pm 2\sqrt{3}}{2} = 1 \pm \sqrt{3}
$$

Three $x$-intercepts: $x = 1$, $x = 1 + \sqrt{3}$, $x = 1 - \sqrt{3}$.

---

**Example 3** (Sign analysis and inequalities of cubic functions): Given $f(x) = (x+2)(x-1)(x-3)$.

(i) Find the solutions of $f(x) = 0$;
(ii) Solve $f(x) > 0$;
(iii) Sketch the graph of $y = f(x)$.

**Solution**:

(i) Set each linear factor to zero: $x = -2$, $x = 1$, $x = 3$.

(ii) Divide the real number line into four intervals using the three zeros. Pick a test point in each interval, determine the sign of each factor, and multiply the three signs to get the sign of $f(x)$:

| Interval | Test point | $(x+2)$ | $(x-1)$ | $(x-3)$ | Product sign |
|------|--------|---------|---------|---------|---------|
| $x < -2$ | $x = -3$ | $-1$ (negative) | $-4$ (negative) | $-6$ (negative) | neg × neg × neg = **negative** |
| $-2 < x < 1$ | $x = 0$ | $2$ (positive) | $-1$ (negative) | $-3$ (negative) | pos × neg × neg = **positive** |
| $1 < x < 3$ | $x = 2$ | $4$ (positive) | $1$ (positive) | $-1$ (negative) | pos × pos × neg = **negative** |
| $x > 3$ | $x = 4$ | $6$ (positive) | $3$ (positive) | $1$ (positive) | pos × pos × pos = **positive** |

Therefore $f(x) > 0$ for $-2 < x < 1$ or $x > 3$.

(iii) Sketch key points:
- $x$-intercepts: $(-2, 0)$, $(1, 0)$, $(3, 0)$
- $y$-intercept: $f(0) = (2)(-1)(-3) = 6$
- End behaviour: $a = 1 > 0$, so as $x \to -\infty$, $f \to -\infty$; as $x \to \infty$, $f \to \infty$
- The graph crosses the $x$-axis at each of the three zeros

---

**Example 4** (Factor theorem and cubic factorisation): Given that $f(x) = x^3 + kx^2 - 4x - 4$ is exactly divisible by $x+1$, find $k$ and fully factorise $f(x)$.

**Solution**:

**Step 1** (Apply the factor theorem): If $x+1$ is a factor, then $f(-1) = 0$.

$$
f(-1) = (-1)^3 + k(-1)^2 - 4(-1) - 4 = -1 + k + 4 - 4 = k - 1
$$

Set $f(-1) = 0$: $k - 1 = 0 \Rightarrow k = 1$.

**Step 2** (Synthetic division): $f(x) = x^3 + x^2 - 4x - 4$.

Divide by $(x+1)$:

$$
\begin{array}{c|ccc}
-1 & 1 & 1 & -4 & -4 \\
   &   & -1 & 0 & 4 \\
\hline
   & 1 & 0 & -4 & 0
\end{array}
$$

The quotient is $x^2 - 4 = (x-2)(x+2)$.

**Step 3** (Write the complete factorisation):

$$
f(x) = (x+1)(x-2)(x+2)
$$

---

## 4.3 Exponential Functions and Logarithmic Functions

### 4.3.1 Exponential Functions $f(x) = a^x$ ($a > 0$, $a \neq 1$)

The core characteristic of an exponential function is that the rate of growth (or decay) is proportional to the function value itself.

**Graph properties** (taking $a > 1$ as an example):
- Domain: $\mathbb{R}$ (all real numbers)
- Range: $(0, \infty)$ (always positive)
- Always passes through $(0, 1)$, because $a^0 = 1$
- When $a > 1$, the function is strictly increasing; when $0 < a < 1$, strictly decreasing
- **Horizontal asymptote**: $y = 0$ (the $x$-axis). When $a > 1$, approaches $y=0$ as $x \to -\infty$; when $0 < a < 1$, approaches $y=0$ as $x \to \infty$

**More general form**: $y = k e^{nx} + a$
- Horizontal asymptote is $y = a$
- $k$ controls vertical stretch and direction ($k > 0$ means the graph is above the asymptote, $k < 0$ means below)

**Why is $e$ so important?**

$$
\frac{d}{dx}e^x = e^x
$$

$e^x$ is the **only function whose derivative equals itself**. For a general base $a$:

$$
\frac{d}{dx}a^x = a^x \ln a
$$

When $a = e$, $\ln e = 1$, and the derivative simplifies to $e^x$ itself.

### 4.3.2 Detailed Derivation of the Natural Exponential Function $e^x$

**Question**: Does there exist a number $e$ such that the derivative of $e^x$ equals $e^x$?

Start from the general exponential function $f(x) = a^x$. By the definition of the derivative:

$$
f'(x) = \lim_{h \to 0} \frac{a^{x+h} - a^x}{h}
$$

**Step 1**: Factor out $a^x$:

$$
f'(x) = \lim_{h \to 0} \frac{a^x(a^h - 1)}{h} = a^x \cdot \lim_{h \to 0} \frac{a^h - 1}{h}
$$

**Step 2**: Denote $L(a) = \displaystyle\lim_{h \to 0} \frac{a^h - 1}{h}$. This limit depends on $a$. So:

$$
f'(x) = a^x \cdot L(a) = f(x) \cdot L(a)
$$

**Step 3**: We want $L(a) = 1$, so that $f'(x) = f(x)$. Solving $L(a) = 1$ numerically:

| $a$ | $L(a) \approx \dfrac{a^{0.001} - 1}{0.001}$ |
|-----|-------------------------------------------|
| $2$ | $\approx 0.693$ |
| $2.7$ | $\approx 0.993$ |
| $2.71$ | $\approx 0.996$ |
| $2.718$ | $\approx 0.999$ |
| $2.71828$ | $\approx 1.000$ |

This special number is $e \approx 2.71828$, which can also be defined as a limit:

$$
e = \lim_{n \to \infty} \left(1 + \frac{1}{n}\right)^n
$$

**Numerical verification**:
- $n = 1$: $(1+1)^1 = 2$
- $n = 10$: $(1.1)^{10} \approx 2.594$
- $n = 100$: $(1.01)^{100} \approx 2.705$
- $n = 10000$: $(1.0001)^{10000} \approx 2.718$

### 4.3.3 Logarithmic Functions $f(x) = \log_a x$ ($a > 0$, $a \neq 1$)

The logarithmic function is the **inverse** of the exponential function:

$$
y = \log_a x \iff a^y = x \quad (x > 0)
$$

**Graph properties** (taking $a > 1$ as an example):
- Domain: $(0, \infty)$ (the argument must be positive)
- Range: $\mathbb{R}$
- Always passes through $(1, 0)$, because $\log_a 1 = 0$
- When $a > 1$, the function is strictly increasing; when $0 < a < 1$, strictly decreasing
- **Vertical asymptote**: $x = 0$ (the $y$-axis). When $a > 1$, as $x \to 0^+$, $\log_a x \to -\infty$

**More general form**: $y = k \ln(ax + b)$
- Vertical asymptote at $ax + b = 0$, i.e., $x = -\dfrac{b}{a}$
- Domain is $x > -\dfrac{b}{a}$

**Two important special bases**:
- **Common logarithm** (base $10$): $\log_{10} x$, sometimes written as $\lg x$
- **Natural logarithm** (base $e$): $\log_e x$, written as $\ln x$

**Exponential and logarithmic functions are inverses of each other**:

$$
y = a^x \quad \stackrel{\text{inverse}}{\longleftrightarrow} \quad y = \log_a x
$$

**Derivation of symmetry**:
Suppose point $(p, q)$ lies on $y = a^x$, then $q = a^p$.
By the definition of the logarithm, $p = \log_a q$, so point $(q, p)$ lies on $y = \log_a x$.
Point $(p, q)$ reflected across the line $y = x$ is exactly $(q, p)$ (because the coordinates are swapped).
Therefore the graphs of the two functions are symmetrical about $y = x$.

### 4.3.4 Detailed Derivation of Logarithmic Laws

The essence of logarithm laws is **downgrading** the operation — multiplication becomes addition, division becomes subtraction, and exponents become coefficients.

**Law 1 — Logarithm of a product**: $\log_a (MN) = \log_a M + \log_a N$

*Derivation*:
Let $\log_a M = x$, $\log_a N = y$.
By definition of the logarithm: $a^x = M$, $a^y = N$.
Then $MN = a^x \cdot a^y = a^{x+y}$.
By the definition of the logarithm again: $\log_a (MN) = x + y = \log_a M + \log_a N$. $\square$

**Law 2 — Logarithm of a quotient**: $\log_a \left(\dfrac{M}{N}\right) = \log_a M - \log_a N$

*Derivation*:
Let $\log_a M = x$, $\log_a N = y$.
Then $\dfrac{M}{N} = \dfrac{a^x}{a^y} = a^{x-y}$.
Therefore $\log_a \left(\dfrac{M}{N}\right) = x - y = \log_a M - \log_a N$. $\square$

**Law 3 — Logarithm of a power**: $\log_a (M^k) = k \log_a M$

*Derivation*:
Let $\log_a M = x$, then $a^x = M$.
Then $M^k = (a^x)^k = a^{kx}$.
By definition: $\log_a (M^k) = kx = k \log_a M$. $\square$

**Law 4 — Change of base formula**: $\log_a M = \dfrac{\log_b M}{\log_b a}$

*Derivation*:
Let $y = \log_a M$, then $a^y = M$.
Take the logarithm to base $b$ of both sides:
$\log_b (a^y) = \log_b M$
$y \log_b a = \log_b M$
$y = \dfrac{\log_b M}{\log_b a}$
Therefore $\log_a M = \dfrac{\log_b M}{\log_b a}$. $\square$

The two most common applications of the change of base formula:

$$
\log_a M = \frac{\log M}{\log a} \quad \text{(change to common logarithm)},
\qquad
\log_a M = \frac{\ln M}{\ln a} \quad \text{(change to natural logarithm)}
$$

**Inverse identities** (directly from the definition of inverse functions):

$$
a^{\log_a x} = x \quad (x > 0), \qquad \log_a (a^x) = x \quad (x \in \mathbb{R})
$$

### 4.3.5 Solving Exponential Equations $a^x = b$

**Basic method**: Take logarithms of both sides, then use the power law to bring the exponent down as a coefficient.

$$
a^x = b \quad \Rightarrow \quad \ln(a^x) = \ln b \quad \Rightarrow \quad x \ln a = \ln b \quad \Rightarrow \quad x = \frac{\ln b}{\ln a}
$$

Common logarithms can also be used: $x = \dfrac{\log b}{\log a}$.

> ⚠️ **Note**: The equation has a real solution only when $b > 0$. If $b \leq 0$, the equation $a^x = b$ has no real solution (since the range of the exponential function is $(0, \infty)$).

---

### Worked Examples 4.3 (Exponential and Logarithmic Functions)

**Example 1** (Logarithm simplification and evaluation): Simplify $\log_2 24 - \log_2 3 + \log_2 \dfrac{1}{2}$.

**Solution**:

**Step 1** (Use the quotient law to combine the first two terms):

$$
\log_2 24 - \log_2 3 = \log_2 \frac{24}{3} = \log_2 8
$$

**Step 2** (Use the product law to continue):

$$
\log_2 8 + \log_2 \frac{1}{2} = \log_2 \left(8 \times \frac{1}{2}\right) = \log_2 4
$$

**Step 3** (Evaluate): $\log_2 4 = 2$, because $2^2 = 4$.

Therefore the value of the expression is $2$.

---

**Example 2** (Change of base and logarithmic equations):

(i) Express $\log_5 20$ in terms of natural logarithms and simplify;
(ii) Solve $\log_2 (x+1) + \log_2 (x-1) = 3$.

**Solution**:

(i) Using the change of base formula:

$$
\log_5 20 = \frac{\ln 20}{\ln 5}
$$

Factor $20 = 4 \times 5$, so $\ln 20 = \ln(4 \times 5) = \ln 4 + \ln 5 = \ln(2^2) + \ln 5 = 2\ln 2 + \ln 5$.

Therefore:

$$
\log_5 20 = \frac{2\ln 2 + \ln 5}{\ln 5} = \frac{2\ln 2}{\ln 5} + 1
$$

(ii) **Step 1** (Combine the logarithms):

$$
\log_2[(x+1)(x-1)] = 3 \Rightarrow \log_2(x^2 - 1) = 3
$$

**Step 2** (Remove the logarithm — exponentiate both sides base $2$):

$$
x^2 - 1 = 2^3 = 8
$$

**Step 3** (Solve the quadratic):

$$
x^2 = 9 \Rightarrow x = \pm 3
$$

**Step 4** (Check the domain): The arguments of logarithms must be positive.

$x+1 > 0 \Rightarrow x > -1$, $x-1 > 0 \Rightarrow x > 1$. Intersection gives $x > 1$.

$x = 3 > 1$, valid. $x = -3$ does not satisfy $x > 1$, rejected.

Therefore $x = 3$.

---

**Example 3** (Solving exponential equations and exponential–logarithmic composites):

(i) Solve $3^{2x-1} = 7$, giving the result in terms of natural logarithms;
(ii) Given $f(x) = \ln(e^{2x} + 1)$, find $f(0)$.

**Solution**:

(i) Take natural logarithms of both sides:

$$
\ln(3^{2x-1}) = \ln 7
$$

Use the power law to bring the exponent down:

$$
(2x - 1)\ln 3 = \ln 7
$$

Solve for $x$:

$$
2x - 1 = \frac{\ln 7}{\ln 3} \Rightarrow 2x = 1 + \frac{\ln 7}{\ln 3} \Rightarrow x = \frac{1}{2}\left(1 + \frac{\ln 7}{\ln 3}\right)
$$

(ii) Substitute $x = 0$:

$$
f(0) = \ln(e^{0} + 1) = \ln(1 + 1) = \ln 2
$$

---

**Example 4** (Exponential equation — substitution method): Solve $4^x - 5 \cdot 2^x + 4 = 0$.

**Solution**:

**Step 1** (Identify the structure): Note that $4^x = (2^2)^x = 2^{2x} = (2^x)^2$.

**Step 2** (Substitute): Let $u = 2^x$, noting $u > 0$ (since the exponential function is always positive).

The equation becomes:

$$
u^2 - 5u + 4 = 0
$$

**Step 3** (Solve the quadratic):

$$
(u-1)(u-4) = 0 \Rightarrow u = 1 \text{ or } u = 4
$$

**Step 4** (Back-substitute):

- $2^x = 1 \Rightarrow x = \log_2 1 = 0$
- $2^x = 4 \Rightarrow x = \log_2 4 = 2$

Both solutions satisfy the domain, so $x = 0$ or $x = 2$.

---

**Example 5** (Logarithmic equation — change of base leading to a quadratic): Solve $\log_3 x + \log_x 3 = 2$.

**Solution**:

**Step 1** (Change of base): Use the change of base formula to express $\log_x 3$ in base $3$:

$$
\log_x 3 = \frac{\log_3 3}{\log_3 x} = \frac{1}{\log_3 x}
$$

**Step 2** (Substitute): Let $u = \log_3 x$ (note $x > 0$ and $x \neq 1$, otherwise $\log_x 3$ is undefined).

The equation becomes:

$$
u + \frac{1}{u} = 2
$$

**Step 3** (Clear denominators): Multiply both sides by $u$ ($u \neq 0$):

$$
u^2 + 1 = 2u \Rightarrow u^2 - 2u + 1 = 0 \Rightarrow (u-1)^2 = 0
$$

**Step 4** (Back-substitute): $u = 1 \Rightarrow \log_3 x = 1 \Rightarrow x = 3^1 = 3$.

**Verification**: $\log_3 3 = 1$, $\log_3 3 = 1$, $1 + 1 = 2$. $\checkmark$

---

**Example 6** (Exponential inequality — taking logarithms of both sides): Solve $2^x < 5$.

**Solution**:

Take natural logarithms of both sides. Since $\ln$ is an increasing function, the direction of the inequality **does not change**:

$$
\ln(2^x) < \ln 5
$$

Use the power law:

$$
x \ln 2 < \ln 5
$$

Since $\ln 2 > 0$, dividing both sides by $\ln 2$ does not change the inequality direction:

$$
x < \frac{\ln 5}{\ln 2}
$$

So the solution is $x < \dfrac{\ln 5}{\ln 2}$ (approximately $x < 2.322$).

> ⚠️ **Note**: If the base $a$ satisfies $0 < a < 1$, the inequality direction reverses when taking logarithms (because $\ln a < 0$). For example, solving $\left(\dfrac12\right)^x < 3$:
>
> $x\ln\frac12 < \ln 3$, since $\ln\frac12 < 0$, dividing both sides gives $x > \dfrac{\ln 3}{\ln(1/2)}$.

---

**Example 7** (Expressing unknown logarithms in terms of known ones): Given $\log_a 2 = p$, $\log_a 5 = q$. Express in terms of $p$ and $q$:

(i) $\log_a 20$;
(ii) $\log_a 0.4$.

**Solution**:

(i) $20 = 2^2 \times 5$, so:

$$
\log_a 20 = \log_a (2^2 \times 5) = \log_a 2^2 + \log_a 5 = 2\log_a 2 + \log_a 5 = 2p + q
$$

(ii) $0.4 = \dfrac{2}{5}$, so:

$$
\log_a 0.4 = \log_a \frac{2}{5} = \log_a 2 - \log_a 5 = p - q
$$

---

**Example 8** (Asymptotes and transformations of exponential function graphs — Syllabus 6.1): Function $f(x) = 3e^{2x} - 4$.

(i) Find the horizontal asymptote of $f(x)$;
(ii) Find the intercepts of $f(x)$ with the coordinate axes;
(iii) Describe the domain and range of $f$.

**Solution**:

(i) As $x \to -\infty$, $e^{2x} \to 0$, so $3e^{2x} - 4 \to -4$.

Thus the horizontal asymptote is $y = -4$.

(ii) **$y$-intercept**: Set $x = 0$, $f(0) = 3e^{0} - 4 = 3 - 4 = -1$, i.e., $(0, -1)$.

**$x$-intercept**: Set $f(x) = 0$:

$$
3e^{2x} - 4 = 0 \Rightarrow e^{2x} = \frac{4}{3}
$$

Take natural logarithms of both sides: $2x = \ln\frac{4}{3} \Rightarrow x = \dfrac12\ln\frac{4}{3}$.

The $x$-intercept is $\left(\dfrac12\ln\frac{4}{3}, 0\right)$.

(iii) **Domain**: $\mathbb{R}$ (all real numbers).

**Range**: Since $e^{2x} > 0$ for all real $x$, $3e^{2x} > 0$, $3e^{2x} - 4 > -4$. Range is $(-4, \infty)$.

---

**Example 9** (Asymptotes of logarithmic function graphs — Syllabus 6.1): Function $g(x) = 2\ln(x-1) + 3$.

(i) Find the domain and vertical asymptote of $g(x)$;
(ii) Find the intercepts of $g(x)$ with the coordinate axes.

**Solution**:

(i) **Domain**: The argument must be positive: $x-1 > 0 \Rightarrow x > 1$. Domain is $(1, \infty)$.

**Vertical asymptote**: Occurs where the argument is zero: $x-1 = 0 \Rightarrow x = 1$. As $x \to 1^+$, $\ln(x-1) \to -\infty$, $g(x) \to -\infty$.

Therefore the vertical asymptote is $x = 1$.

(ii) **$y$-intercept**: $x = 0$ is not in the domain, so there is no $y$-intercept.

**$x$-intercept**: Set $g(x) = 0$:

$$
2\ln(x-1) + 3 = 0 \Rightarrow \ln(x-1) = -\frac{3}{2}
$$

Exponentiate both sides: $x - 1 = e^{-3/2} \Rightarrow x = 1 + e^{-3/2}$.

The $x$-intercept is $(1 + e^{-3/2}, 0)$ (approximately $(1.223, 0)$).

---

## 4.4 Inverse Functions and Composite Functions

### 4.4.1 Inverse Functions

**Definition**: If a function $f$ is one–one (injective), then it has an inverse $f^{-1}$, satisfying:

$$
f^{-1}(y) = x \iff f(x) = y
$$

**Core properties**:

$$
f^{-1}(f(x)) = x, \qquad f(f^{-1}(x)) = x
$$

**Geometric meaning**: The graphs of $y = f(x)$ and $y = f^{-1}(x)$ are symmetrical about the line $y = x$.

**Detailed derivation of symmetry**:

Let point $(a, b)$ lie on $y = f(x)$, i.e., $b = f(a)$.
By the definition of the inverse, $a = f^{-1}(b)$, so point $(b, a)$ lies on $y = f^{-1}(x)$.
Point $(a, b)$ reflected across the line $y = x$ is exactly $(b, a)$ (because the coordinates are swapped).
Therefore the graphs of $f$ and $f^{-1}$ are mirror images of each other across $y = x$.

**Example**: For $f(x) = 2^x$ and $f^{-1}(x) = \log_2 x$:
- $f$ passes through $(0, 1)$, $(1, 2)$, $(2, 4)$
- $f^{-1}$ passes through $(1, 0)$, $(2, 1)$, $(4, 2)$
- Each pair of points is symmetrical about $y = x$

**Why do only one–one functions have inverses?**

If $f$ is not one–one (i.e., there exist $x_1 \neq x_2$ such that $f(x_1) = f(x_2) = y_0$), then the inverse $f^{-1}$ would need to return two different values — $x_1$ and $x_2$ — at $x = y_0$, which violates the definition of a function. Therefore non–one–one functions have no inverses.

**How to explain in words why a function has no inverse** (Syllabus 1.5 standard wording):

"The function $f$ is not one–one because different $x$ values correspond to the same $y$ value. For example, $f(a) = f(b)$ but $a \neq b$. The horizontal line $y = f(a)$ intersects the graph of $y = f(x)$ at more than one point. Therefore $f$ has no inverse."

**Steps for finding the inverse**:
1. Write $y = f(x)$ as an equation.
2. Solve for $x$ in terms of $y$.
3. Swap the roles of $x$ and $y$ to obtain the expression $y = f^{-1}(x)$.
4. State the domain of the inverse function (which is the range of the original function).

**Relationship between the domain and range of a function and its inverse**:
- Domain of $f$ = Range of $f^{-1}$
- Range of $f$ = Domain of $f^{-1}$

> ⚠️ **Key point**: Sometimes the domain of the original function must be **restricted** to make $f$ one–one, so that an inverse exists. For example, $f(x) = x^2$ is not one–one on all of $\mathbb{R}$, but restricting to $x \geq 0$ makes it one–one, and the inverse becomes $\sqrt{x}$.

### 4.4.2 Composite Functions

**Definition**: $(f \circ g)(x) = f(g(x))$, read as "$f$ composed with $g$", also written as $fg(x)$.

**Order of composition**: Apply $g$ first, then apply $f$ to the result. The order is usually not commutative — generally $f(g(x)) \neq g(f(x))$.

**Domain of a composite function**: Two conditions must be satisfied:
1. $x$ must be in the domain of $g$
2. $g(x)$ must be in the domain of $f$

**Important relationships** (Syllabus 1.2):

$$
\text{Domain}(gf) \subseteq \text{Domain}(f), \qquad \text{Range}(gf) \subseteq \text{Range}(g)
$$

> Explanation: To compute $gf(x) = g(f(x))$, $x$ must first be in the domain of $f$, and $f(x)$ must be in the domain of $g$. Therefore the domain of $gf$ is a subset of the domain of $f$. The output of $gf$ comes from $g$, so its range is a subset of the range of $g$.

**Further explanation of domain restrictions for the existence of composite functions**:

Sometimes the domain of $f$ needs to be restricted for $gf$ to exist. This is because $f(x)$ must lie within the domain of $g$.

*Example*: Given $f(x) = x^2$ (domain $\mathbb{R}$), $g(x) = \sqrt{1 - x^2}$ (domain $|x| \leq 1$).

$gf(x) = g(f(x)) = \sqrt{1 - (x^2)^2} = \sqrt{1 - x^4}$.

The domain of $gf$ requires $1 - x^4 \geq 0 \Rightarrow |x| \leq 1$.

So $\text{Domain}(gf) = [-1, 1] \subset \mathbb{R} = \text{Domain}(f)$.

---

### Worked Examples 4.4 (Inverse Functions and Composite Functions)

**Example 1** (Finding the inverse — linear function): Find the inverse of $f(x) = \dfrac{2x - 3}{5}$.

**Solution**:

**Step 1** (Write the equation): $y = \dfrac{2x - 3}{5}$

**Step 2** (Solve for $x$):

$$
5y = 2x - 3 \Rightarrow 2x = 5y + 3 \Rightarrow x = \frac{5y + 3}{2}
$$

**Step 3** (Swap $x$ and $y$):

$$
f^{-1}(x) = \frac{5x + 3}{2}
$$

**Step 4** (Domain): The domain of the inverse is $\mathbb{R}$ (the range of the original function is $\mathbb{R}$).

**Verification**:

$$
f(f^{-1}(x)) = f\left(\frac{5x+3}{2}\right) = \frac{2\cdot\frac{5x+3}{2} - 3}{5} = \frac{5x+3-3}{5} = x
$$

---

**Example 2** (Finding the inverse — with domain restriction): Given $f(x) = x^2 - 4x + 3$, $x \geq 2$. Find $f^{-1}(x)$ and its domain.

**Solution**:

**Step 1** (Complete the square to find the vertex and range):

$$
f(x) = x^2 - 4x + 3 = (x^2 - 4x + 4) - 4 + 3 = (x-2)^2 - 1
$$

The vertex is at $(2, -1)$. Since $a = 1 > 0$ and the domain is $x \geq 2$ (to the right of the vertex), the function is strictly increasing. The range is $[-1, \infty)$.

**Step 2** (Solve for $x$): Let $y = (x-2)^2 - 1$.

$$
y + 1 = (x-2)^2 \Rightarrow x - 2 = \pm \sqrt{y+1}
$$

Since $x \geq 2$, take the positive root: $x = 2 + \sqrt{y+1}$.

**Step 3** (Swap $x$ and $y$):

$$
f^{-1}(x) = 2 + \sqrt{x+1}
$$

**Step 4** (Domain): The domain of the inverse is the range of the original function, i.e., $[-1, \infty)$.

**Verification**:

$$
f(f^{-1}(x)) = f(2 + \sqrt{x+1}) = (2+\sqrt{x+1} - 2)^2 - 1 = (x+1) - 1 = x
$$

---

**Example 3** (Composite function and its domain — detailed derivation): Given $f(x) = \sqrt{x-1}$, $g(x) = \dfrac{1}{x-2}$.

(i) Find $fg(x)$ and its domain;
(ii) Find $gf(x)$ and its domain.

**Solution**:

(i) $fg(x) = f(g(x)) = \sqrt{\dfrac{1}{x-2} - 1}$

**Domain analysis**:

**Condition 1**: $g(x)$ must be defined. Denominator non-zero: $x \neq 2$.

**Condition 2**: $g(x)$ must lie in the domain of $f$. $f$'s domain requires the radicand $\geq 0$, i.e.:

$$
\frac{1}{x-2} - 1 \geq 0
$$

Solve this inequality. This is the key step — consider cases:

*Case A*: $x > 2$. Multiply both sides by the positive number $(x-2)$, the inequality sign stays the same:

$$
1 \geq x - 2 \Rightarrow x \leq 3
$$

Combining with $x > 2$, we get $2 < x \leq 3$.

*Case B*: $x < 2$. Multiply both sides by the negative number $(x-2)$, the inequality sign reverses:

$$
1 \leq x - 2 \Rightarrow x \geq 3
$$

Combining with $x < 2$, there is no solution.

Therefore condition 2 gives $2 < x \leq 3$.

**Intersection**: $x \neq 2$ and $2 < x \leq 3$, the domain is $(2, 3]$.

**Simplify the expression**:

$$
\frac{1}{x-2} - 1 = \frac{1 - (x-2)}{x-2} = \frac{3 - x}{x-2}
$$

Therefore:

$$
fg(x) = \sqrt{\frac{3 - x}{x - 2}}, \quad x \in (2, 3]
$$

(ii) $gf(x) = g(f(x)) = \dfrac{1}{\sqrt{x-1} - 2}$

**Domain analysis**:

**Condition 1**: $f(x)$ must be defined. Radicand non-negative: $x - 1 \geq 0 \Rightarrow x \geq 1$.

**Condition 2**: $f(x)$ must lie in $g$'s domain. $g$'s denominator cannot be zero: $\sqrt{x-1} - 2 \neq 0$.

$$
\sqrt{x-1} \neq 2 \Rightarrow x-1 \neq 4 \Rightarrow x \neq 5
$$

**Intersection**: $x \geq 1$ and $x \neq 5$, the domain is $[1, 5) \cup (5, \infty)$.

---

**Example 4** (Range of composite functions and $fg \neq gf$): $f(x) = 2^x$, $g(x) = x^2$. Find expressions for $fg(x)$ and $gf(x)$, and find the range of $fg(x)$.

**Solution**:

**$fg(x)$**: $fg(x) = f(g(x)) = 2^{x^2}$

**$gf(x)$**: $gf(x) = g(f(x)) = (2^x)^2 = 2^{2x} = 4^x$

Note that $fg(x) = 2^{x^2} \neq 4^x = gf(x)$, showing that the order of composition matters.

**Find the range of $fg(x)$**:
- $g(x) = x^2$ has range $[0, \infty)$
- $f(u) = 2^u$ is strictly increasing on $[0, \infty)$
- Minimum: when $u = 0$, $2^0 = 1$
- Upper bound: as $u \to \infty$, $2^u \to \infty$

Therefore the range of $fg(x)$ is $[1, \infty)$.

---

**Example 5** (Explaining in words why a function has no inverse — Syllabus 1.5):

(i) $f(x) = x^2$, domain $\mathbb{R}$.
(ii) $f(x) = \cos x$, domain $[0, 2\pi]$.

**Solution**:

(i) $f(x) = x^2$ **is not one–one** because different $x$ values correspond to the same $y$ value. For example, $f(2) = 4$ and $f(-2) = 4$, i.e., $2 \neq -2$ but $f(2) = f(-2)$. The horizontal line $y = 4$ intersects the graph of $y = x^2$ at $(2, 4)$ and $(-2, 4)$, two points. Therefore $f$ has no inverse.

> However, if we restrict the domain to $x \geq 0$, then $f$ becomes one–one, and the inverse is $f^{-1}(x) = \sqrt{x}$.

(ii) $f(x) = \cos x$ **is not one–one** on $[0, 2\pi]$. For example, $\cos(\frac{\pi}{3}) = \frac12$ and $\cos(\frac{5\pi}{3}) = \frac12$, but $\frac{\pi}{3} \neq \frac{5\pi}{3}$. The horizontal line $y = \frac12$ intersects the graph at two points. Therefore $f$ has no inverse.

> However, if we restrict the domain to $[0, \pi]$, $\cos x$ is strictly decreasing, and the inverse is $\arccos x$.

---

**Example 6** (Sketching the symmetrical relationship between a function and its inverse about $y=x$ — Syllabus 1.8): Given $f(x) = e^x$.

(i) Find $f^{-1}(x)$;
(ii) Describe the relationship between $y = f(x)$, $y = f^{-1}(x)$ and $y = x$ on the same coordinate axes.

**Solution**:

(i) $y = e^x \Rightarrow x = \ln y \Rightarrow f^{-1}(x) = \ln x$ (domain $x > 0$).

(ii) **Symmetry**: The graphs of $y = e^x$ and $y = \ln x$ are symmetrical about the line $y = x$.

Corresponding points:
- $e^x$ passes through $(0, 1)$ → $\ln x$ passes through $(1, 0)$
- $e^x$ passes through $(1, e)$ → $\ln x$ passes through $(e, 1)$
- $e^x$ passes through $(-1, e^{-1})$ → $\ln x$ passes through $(e^{-1}, -1)$

Each curve is the mirror image of the other in $y = x$.

**Asymptote relationship**:
- $y = e^x$ has a horizontal asymptote $y = 0$ (the $x$-axis)
- $y = \ln x$ has a vertical asymptote $x = 0$ (the $y$-axis)
- This pair of asymptotes is also symmetrical about $y = x$

---

**Example 7** (The importance of order in composite functions $fg \neq gf$ — Syllabus 1.7): $f(x) = 3x + 1$, $g(x) = x^2$. Find $fg(x)$ and $gf(x)$ and compare.

**Solution**:

$fg(x) = f(g(x)) = f(x^2) = 3x^2 + 1$

$gf(x) = g(f(x)) = g(3x+1) = (3x+1)^2 = 9x^2 + 6x + 1$

Clearly $fg(x) \neq gf(x)$, so the order of composition is crucial.

---

**Example 8** (Integrated application of inverse and composite functions): Given $f(x) = 2x + 3$, $g(x) = \dfrac{1}{x-1}$, $x \neq 1$.

(i) Find $f^{-1}(x)$;
(ii) Find $gf^{-1}(x)$ and its domain.

**Solution**:

(i) $y = 2x + 3 \Rightarrow 2x = y - 3 \Rightarrow x = \dfrac{y-3}{2}$
Swap: $f^{-1}(x) = \dfrac{x-3}{2}$, domain $\mathbb{R}$.

(ii) $gf^{-1}(x) = g\left(\dfrac{x-3}{2}\right) = \dfrac{1}{\dfrac{x-3}{2} - 1}$

Simplify the denominator: $\dfrac{x-3}{2} - 1 = \dfrac{x-3 - 2}{2} = \dfrac{x-5}{2}$

Therefore:

$$
gf^{-1}(x) = \frac{1}{\frac{x-5}{2}} = \frac{2}{x-5}
$$

**Domain**:
- $f^{-1}(x)$ has domain $\mathbb{R}$ (no restriction)
- $g$'s domain requires the denominator non-zero: $\dfrac{x-3}{2} - 1 \neq 0 \Rightarrow \dfrac{x-5}{2} \neq 0 \Rightarrow x \neq 5$

Therefore the domain is $\mathbb{R} \setminus \{5\}$.

---

**Example 9** (Syllabus 1.6 specified example — inverse of an exponential function): Given $f(x) = e^{2x}$, find $f^{-1}(x)$.

**Solution**:

Let $y = e^{2x}$. Take natural logarithms of both sides:

$$
\ln y = \ln(e^{2x}) = 2x \cdot \ln e = 2x
$$

Since $\ln e = 1$, we have $2x = \ln y \Rightarrow x = \frac12\ln y$.

Swap $x$ and $y$:

$$
f^{-1}(x) = \frac12\ln x
$$

**Domain**: The range of the original function $f(x) = e^{2x}$ is $(0, \infty)$, so the domain of $f^{-1}$ is $(0, \infty)$.

**Verification**:

$$
f(f^{-1}(x)) = e^{2 \cdot \frac12\ln x} = e^{\ln x} = x \quad (x > 0)
$$

---

**Example 10** (Verifying $\text{Domain}(gf) \subseteq \text{Domain}(f)$ — Syllabus 1.2): $f(x) = \sqrt{x}$, $g(x) = \dfrac{1}{x-3}$. Find the domain of $gf(x)$ and verify $\text{Domain}(gf) \subseteq \text{Domain}(f)$.

**Solution**:

$gf(x) = g(f(x)) = \dfrac{1}{\sqrt{x} - 3}$

**Condition 1**: $f$'s domain: $x \geq 0$.
**Condition 2**: $f(x)$ must be in $g$'s domain: $\sqrt{x} - 3 \neq 0 \Rightarrow \sqrt{x} \neq 3 \Rightarrow x \neq 9$.

Intersection: $x \geq 0$ and $x \neq 9$, i.e., $[0, 9) \cup (9, \infty)$.

Verifying $\text{Domain}(gf) \subseteq \text{Domain}(f)$:
$\text{Domain}(f) = [0, \infty)$, $\text{Domain}(gf) = [0, 9) \cup (9, \infty) \subset [0, \infty)$. $\checkmark$

---

## 4.5 Graphs of Absolute Value Functions $y = |f(x)|$

### 4.5.1 Basic Principles

$y = |f(x)|$ is defined as:

$$
|f(x)| = \begin{cases}
f(x), & f(x) \geq 0 \\
-f(x), & f(x) < 0
\end{cases}
$$

**Graph transformation rule**: Take the graph of $y = f(x)$, **reflect** the parts below the $x$-axis **upwards** across the $x$-axis (i.e., take the absolute value of the $y$-coordinate), while the parts above and on the $x$-axis remain unchanged.

**Key observations**:
- After reflection, all $y$ values are non-negative ($|f(x)| \geq 0$).
- At points where $f(x) = 0$ (i.e., $x$-intercepts), the absolute value graph forms **cusps** — because the slope suddenly changes sign on either side.
- The range of $|f(x)|$ is $[0, \infty)$ (if the original function can take arbitrarily large positive values) or $[0, \text{finite maximum}]$.

### 4.5.2 Characteristics of Absolute Value Graphs for Different Function Types

| Original function type | Features of $|f(x)|$ |
|-----------|----------------|
| **Linear** $|mx + c|$ | V-shape, cusp at $x = -c/m$ |
| **Quadratic** $|ax^2+bx+c|$ | Cusps at $x$-intercepts, portions of parabola below $x$-axis reflected upward |
| **Cubic** $|(x-p)(x-q)(x-r)|$ | Cusps at all three $x$-intercepts |
| **Trigonometric** $|a\sin bx + c|$ | Period halved (for $\sin$, from $2\pi$ to $\pi$), troughs become peaks |
| **Trigonometric** $|a\cos bx + c|$ | Period halved (for $\cos$, from $2\pi$ to $\pi$), troughs become peaks |
| **Trigonometric** $|a\tan bx + c|$ | Vertical asymptotes unchanged, graph reflected to make $y \geq 0$ |

### 4.5.3 Solving Absolute Value Equations and Inequalities

**Equation $|f(x)| = k$ ($k > 0$)**: Equivalent to $f(x) = k$ or $f(x) = -k$.

**Inequality $|f(x)| < k$ ($k > 0$)**: Equivalent to $-k < f(x) < k$.

**Inequality $|f(x)| > k$ ($k > 0$)**: Equivalent to $f(x) > k$ or $f(x) < -k$.

---

### Worked Examples 4.5 (Absolute Value Functions)

**Example 1** (Absolute value of a linear function — V-shape): Sketch the graph of $y = |2x - 3|$ and find the values of $x$ for which $y = 5$.

**Solution**:

**Sketch**:

$f(x) = 2x - 3$, $f(x) = 0$ when $x = 1.5$.

When $x \geq 1.5$, $2x - 3 \geq 0$, so $|2x-3| = 2x-3$ (straight line, slope $2$).
When $x < 1.5$, $2x - 3 < 0$, so $|2x-3| = -(2x-3) = -2x+3$ (straight line, slope $-2$).

The graph is V-shaped, with the cusp at $(1.5, 0)$.

**Solve $|2x-3| = 5$**:

Case 1: $2x-3 = 5 \Rightarrow 2x = 8 \Rightarrow x = 4$
Case 2: $2x-3 = -5 \Rightarrow 2x = -2 \Rightarrow x = -1$

Solutions are $x = 4$ or $x = -1$.

---

**Example 2** (Absolute value of a quadratic function): Sketch the graph of $y = |x^2 - 4x + 3|$.

**Solution**:

**Step 1** (Sketch the original function): $y = x^2 - 4x + 3 = (x-1)(x-3)$.

- $x$-intercepts: $x = 1$ and $x = 3$
- Vertex: $x = 2$, $y = 4 - 8 + 3 = -1$, i.e., $(2, -1)$
- Opens upward ($a = 1 > 0$)

**Step 2** (Take absolute value): On the interval $[1, 3]$, the original function $f(x) \leq 0$; this part is reflected upward. For $x < 1$ and $x > 3$, $f(x) > 0$, so these parts remain unchanged.

**Step 3** (Mark key points): Cusps at $x = 1$ and $x = 3$. After reflection, the original vertex $(2, -1)$ becomes $(2, 1)$.

Range is $[0, \infty)$.

---

**Example 3** (Absolute value graph and sign analysis of a cubic function): Given $f(x) = (x+1)(x-1)(x-2)$.

(i) Sketch the graph of $y = |f(x)|$;
(ii) Discuss the number of intersection points between $|f(x)|$ and $y = 2$.

**Solution**:

(i) **Sign analysis**:

| Interval | Test point | $(x+1)$ | $(x-1)$ | $(x-2)$ | Sign of $f(x)$ | $|f(x)|$ |
|------|--------|---------|---------|---------|------------|----------|
| $x < -1$ | $x=-2$ | neg | neg | neg | **neg** | reflected to positive |
| $-1 < x < 1$ | $x=0$ | pos | neg | neg | **pos** | unchanged |
| $1 < x < 2$ | $x=1.5$ | pos | pos | neg | **neg** | reflected to positive |
| $x > 2$ | $x=3$ | pos | pos | pos | **pos** | unchanged |

$x$-intercepts: $x = -1, 1, 2$ (all cusps).
$y$-intercept: $f(0) = (1)(-1)(-2) = 2$.

(ii) Intersections of $y = 2$ with $|f(x)|$:
- On $(-1, 1)$: $f(0) = 2$, one intersection.
- In the reflected region $x < -1$: $|f(x)| = -f(x)$. $f(-2) = (-1)(-3)(-4) = -12$, $|f(-2)| = 12$, $f(-1) = 0$. By continuity, $y = 2$ intersects once in this region.
- In the reflected region $(1, 2)$: similarly intersects once.

Therefore there are **3 intersection points** in total.

---

**Example 4** (Form $|a\sin bx + c|$ — Syllabus 1.4 specified): Sketch the graph of $y = |\sin x|$ on $[0, 2\pi]$.

**Solution**:

First sketch $y = \sin x$:
- On $[0, \pi]$, $\sin x \geq 0$ (on or above the $x$-axis)
- On $[\pi, 2\pi]$, $\sin x \leq 0$ (below the $x$-axis)

Take absolute value:
- $[0, \pi]$: unchanged
- $[\pi, 2\pi]$: reflected upward ($|\sin x| = -\sin x$)

Graph features:
- Two identical "arches": $(0,0)\to(\frac{\pi}{2},1)\to(\pi,0)$ and $(\pi,0)\to(\frac{3\pi}{2},1)\to(2\pi,0)$
- **Period**: $\pi$ (the original $\sin x$ has period $2\pi$; after reflection, it repeats every $\pi$)
- **Range**: $[0, 1]$
- **Cusps**: at $x = 0, \pi, 2\pi$, etc.

---

**Example 5** (Form $|a\cos bx + c|$ — Syllabus 1.4 specified): Sketch the graph of $y = |3\cos 2x - 1|$ on $[0, \pi]$.

**Solution**:

**Step 1** (Sketch the original function $y = 3\cos 2x - 1$):
- Amplitude $3$, period $\dfrac{2\pi}{2} = \pi$, shifted down by $1$ unit
- Maximum: $3(1) - 1 = 2$, minimum: $3(-1) - 1 = -4$
- Zeros: $3\cos 2x - 1 = 0 \Rightarrow \cos 2x = \dfrac13$
  $2x = \arccos\dfrac13$ or $2x = 2\pi - \arccos\dfrac13$
  i.e., $x = \dfrac12\arccos\dfrac13$ or $x = \pi - \dfrac12\arccos\dfrac13$
  Let $\alpha = \dfrac12\arccos\dfrac13 \approx 0.615$ radians

**Step 2** (Take absolute value):
- On the interval between the two zeros ($\alpha < x < \pi - \alpha$), $3\cos 2x - 1 \leq 0$, this part is reflected upward
- The remaining parts are unchanged

**Step 3** (Mark key points):
- Cusps: at $x = \alpha$ and $x = \pi - \alpha$
- Reflected "peak": the original minimum at $x = \dfrac{\pi}{2}$, where $3\cos\pi - 1 = -4$, becomes $4$
- Original maxima at $x = 0$ (value $2$) and $x = \pi$ (value $2$) remain unchanged

**Final graph features**:
- Range: $[0, 4]$
- Number of cusps (in one period): 2
- Asymptotes: none

---

**Example 6** (Form $|a\tan bx + c|$ — Syllabus 1.4 specified): Sketch the graph of $y = |\tan x - 1|$ on $\left(-\dfrac{\pi}{2}, \dfrac{\pi}{2}\right)$.

**Solution**:

**Step 1** (Sketch the original function $y = \tan x - 1$):
- $\tan x$ has period $\pi$, shifted down by $1$ unit
- Vertical asymptotes: $x = -\dfrac{\pi}{2}$ and $x = \dfrac{\pi}{2}$
- Zero: $\tan x - 1 = 0 \Rightarrow \tan x = 1 \Rightarrow x = \dfrac{\pi}{4}$ (within $(-\frac{\pi}{2}, \frac{\pi}{2})$)
- As $x \to \dfrac{\pi}{2}^-$, $\tan x \to \infty$, $\tan x - 1 \to \infty$
- As $x \to -\dfrac{\pi}{2}^+$, $\tan x \to -\infty$, $\tan x - 1 \to -\infty$

**Step 2** (Take absolute value):
- When $x < \dfrac{\pi}{4}$, $\tan x - 1 < 0$, reflect upward
- When $x > \dfrac{\pi}{4}$, $\tan x - 1 > 0$, unchanged
- When $x = \dfrac{\pi}{4}$, $\tan\dfrac{\pi}{4} - 1 = 0$, cusp

**Step 3** (Analyse behaviour after reflection):
- In the region $x < \dfrac{\pi}{4}$, $|\tan x - 1| = -(\tan x - 1) = 1 - \tan x$
  As $x \to -\dfrac{\pi}{2}^+$, $\tan x \to -\infty$, $1 - \tan x \to \infty$
- In the region $x > \dfrac{\pi}{4}$, $|\tan x - 1| = \tan x - 1$
  As $x \to \dfrac{\pi}{2}^-$, $\tan x \to \infty$, $\tan x - 1 \to \infty$

**Final graph features**:
- Vertical asymptotes still at $x = -\dfrac{\pi}{2}$ and $x = \dfrac{\pi}{2}$ (absolute value does not change the position of asymptotes)
- Cusp at $x = \dfrac{\pi}{4}$
- The graph tends to infinity on both sides of the cusp
- Range: $[0, \infty)$ (minimum value $0$ at $x = \dfrac{\pi}{4}$)

---

**Example 7** (Absolute value equation — quadratic type): Solve $|x^2 - 3x + 2| = 2$.

**Solution**:

Original quadratic: $x^2 - 3x + 2 = (x-1)(x-2)$, roots at $x = 1, 2$.

**Case 1**: $x^2 - 3x + 2 = 2$

$$
x^2 - 3x = 0 \Rightarrow x(x-3) = 0 \Rightarrow x = 0 \text{ or } x = 3
$$

Check: $x = 0$ gives $0 - 0 + 2 = 2 > 0$ (in the non-negative region), valid. $x = 3$ gives $9 - 9 + 2 = 2 > 0$, valid.

**Case 2**: $x^2 - 3x + 2 = -2$

$$
x^2 - 3x + 4 = 0
$$

Discriminant $\Delta = 9 - 16 = -7 < 0$, no real solutions.

Therefore the solutions are $x = 0$ or $x = 3$.

---

**Example 8** (Absolute value inequality — squaring technique): Solve $|x-1| > |2x+3|$.

**Solution**:

Both sides are non-negative, so we can square both sides without changing the inequality direction:

$$
(x-1)^2 > (2x+3)^2
$$

Expand:

$$
x^2 - 2x + 1 > 4x^2 + 12x + 9
$$

Rearrange:

$$
0 > 3x^2 + 14x + 8 \Rightarrow 3x^2 + 14x + 8 < 0
$$

Find roots:

$$
x = \frac{-14 \pm \sqrt{196 - 96}}{6} = \frac{-14 \pm 10}{6}
$$

$x = \dfrac{-14 + 10}{6} = -\dfrac{4}{6} = -\dfrac{2}{3}$, $x = \dfrac{-14 - 10}{6} = -\dfrac{24}{6} = -4$.

Since the coefficient of $x^2$ is $3 > 0$, the parabola opens upward, and the inequality holds between the roots:

$$
-4 < x < -\frac{2}{3}
$$

---

**Example 9** (Extreme values of absolute value functions — geometric interpretation): Function $f(x) = |x-1| + |x-3|$, find the minimum value of $f(x)$.

**Solution**:

**Geometric interpretation**: $|x-1|$ is the distance from $x$ to $1$ on the number line, $|x-3|$ is the distance from $x$ to $3$. $f(x)$ is the sum of these two distances.

When $x$ lies between $[1, 3]$, the sum of the two distances is always equal to the segment length $2$.
When $x < 1$ or $x > 3$, the sum is greater than $2$.

Therefore the minimum value of $f(x)$ is $2$, attained for $x \in [1, 3]$.

**Algebraic verification** — piecewise analysis:

$$
f(x) = \begin{cases}
-(x-1) - (x-3) = -2x + 4, & x < 1 \\
(x-1) - (x-3) = 2, & 1 \leq x \leq 3 \\
(x-1) + (x-3) = 2x - 4, & x > 3
\end{cases}
$$

When $x < 1$, $f(x) = -2x + 4 > 2$ (since $-2x > -2$).
When $1 \leq x \leq 3$, $f(x) = 2$.
When $x > 3$, $f(x) = 2x - 4 > 2$.

The minimum value is $2$.

---

## Chapter Practice Problems

### I. Domain and Range (6 questions)

1. Find the domain of $f(x) = \dfrac{\sqrt{x+3}}{x-5}$.

2. Given $f(x) = x^2 - 6x + 10$, $x \in \mathbb{R}$. Find the minimum value of $f(x)$ and its range.

3. Find the domain and range of $f(x) = \ln(4 - x^2)$.

4. Find the domain of $f(x) = \dfrac{1}{\sqrt{2x-1}} + \ln(5-x)$.

5. Determine whether $y = \pm \sqrt{9 - x^2}$ ($|x| \leq 3$) is a function, and explain why.

6. Given $f(x) = \dfrac{3x-1}{x+2}$, find the range of $f$ and determine whether $f$ is one–one.

### II. Linear and Cubic Functions (5 questions)

7. Line $L$ passes through $(2, -1)$ and is parallel to $y = 3x + 2$. Find the equation of $L$.

8. Given $f(x) = x^3 - 2x^2 - 5x + 6$.
   (i) Verify that $x = 1$ is a root of $f(x)$ and fully factorise $f(x)$;
   (ii) Find all solutions of $f(x) = 0$.

9. Given the cubic function $f(x) = x^3 - 3x^2 - 9x + 11$, find $f'(x)$ and solve $f'(x) = 0$, determining the type of stationary points.

10. Solve the cubic inequality $(x+1)(x-2)(x-4) > 0$.

11. Given that $f(x) = x^3 + kx^2 - 5x - 6$ is exactly divisible by $x+2$, find $k$ and fully factorise $f(x)$.

### III. Exponentials and Logarithms (9 questions)

12. Simplify: $\log_3 54 - \log_3 2 + \log_3 \dfrac13$.

13. Solve $2^{x+1} = 5$, giving the result in terms of natural logarithms.

14. Solve $\log_3 (x+2) + \log_3 (x-4) = 2$.

15. Solve $3^{2x} - 10 \cdot 3^x + 9 = 0$.

16. Compute: $\log_2 3 \cdot \log_3 4 \cdot \log_4 5 \cdot \log_5 2$.

17. Function $f(x) = 2e^{x} - 3$. Find the horizontal asymptote, $y$-intercept and $x$-intercept of $f(x)$.

18. Solve $3^x < 7$.

19. Given $\log_a 3 = p$, $\log_a 7 = q$. Express $\log_a 21$ and $\log_a \dfrac73$ in terms of $p$ and $q$.

20. Solve $\log_2 x + \log_4 x = 3$. (Hint: Use the change of base formula to convert $\log_4 x$ to base $2$.)

### IV. Inverse Functions and Composite Functions (8 questions)

21. Find the inverse $f^{-1}(x)$ of $f(x) = \dfrac{3x - 2}{4}$.

22. Given $f(x) = x^2 + 2x$, $x \geq -1$. Find $f^{-1}(x)$ and its domain.

23. Given $f(x) = 2x + 1$, $g(x) = \dfrac1x$. Find $fg(x)$ and $gf(x)$, and find the domain of $gf(x)$.

24. Given $f(x) = e^{3x}$, find $f^{-1}(x)$.

25. Given $f(x) = \ln(x+2)$, $x > -2$. Find $f^{-1}(x)$.

26. Explain in words why $f(x) = x^4$ (domain $\mathbb{R}$) has no inverse.

27. $f(x) = \sqrt{x+1}$, $g(x) = x^2 - 4$. Find $fg(x)$ and its domain.

28. Given $f(x) = x^2$, $x \geq 0$, $g(x) = 2x + 1$. Verify $\text{Domain}(gf) \subseteq \text{Domain}(f)$.

### V. Absolute Value Functions (6 questions)

29. Sketch the graph of $y = |x-2|$ and solve $|x-2| = 3$.

30. Solve $|2x+1| < 5$.

31. Sketch the graph of $y = |\cos x|$ on $[0, 2\pi]$ and state its period.

32. Solve $|x^2 - 5x + 6| = 2$.

33. Solve $|x+2| \geq 3$.

34. Function $f(x) = |x-2| + |x+1|$, find the minimum value of $f(x)$.

### VI. Trigonometric Absolute Values (3 new questions — Syllabus 1.4 specified)

35. Sketch the key features of $y = |2\cos x + 1|$ on $[0, 2\pi]$, labelling key points and the positions of cusps.

36. Sketch the graph of $y = |\tan x|$ on $\left(-\dfrac{\pi}{2}, \dfrac{\pi}{2}\right)$, indicating the positions of asymptotes.

37. Given $f(x) = |3\sin 2x - 2|$, find the maximum and minimum values of $f(x)$ on $[0, \pi]$.

### VII. Domain Restrictions and Existence of Composite Functions (1 new question — Syllabus 1.2)

38. Given $f(x) = \sqrt{x-2}$, $g(x) = \dfrac{1}{\sqrt{5-x}}$. Find $gf(x)$ and its domain, and verify $\text{Domain}(gf) \subseteq \text{Domain}(f)$.

---

## Answers to Practice Problems

### I. Domain and Range

**1.**
Condition 1 (root): $x+3 \geq 0 \Rightarrow x \geq -3$.
Condition 2 (denominator non-zero): $x-5 \neq 0 \Rightarrow x \neq 5$.
Intersection: $[-3, 5) \cup (5, \infty)$.

---

**2.**
Complete the square:

$$
f(x) = (x^2 - 6x + 9) + 1 = (x-3)^2 + 1
$$

Since $(x-3)^2 \geq 0$, $f(x) \geq 1$.
Minimum at $x = 3$, $f(3) = 1$.
Range is $[1, \infty)$.

---

**3.**
Domain: $4 - x^2 > 0 \Rightarrow x^2 < 4 \Rightarrow -2 < x < 2$, i.e., $(-2, 2)$.

Range: Let $u = 4 - x^2$, $x \in (-2, 2)$, then $u \in (0, 4]$.
$f(x) = \ln u$, $u \in (0, 4]$.
$\ln u$ is increasing on $(0, 4]$, minimum approaches $-\infty$ (as $u \to 0^+$), maximum is $\ln 4$ (at $u = 4$).
Range is $(-\infty, \ln 4]$.

---

**4.**
Condition 1 (denominator radicand): $2x-1 > 0$ (strictly greater, as it is in the denominator) $\Rightarrow x > \dfrac12$.
Condition 2 (logarithm argument): $5 - x > 0 \Rightarrow x < 5$.
Intersection: $\left(\dfrac12, 5\right)$.

---

**5.**
**Not a function**. For example, when $x = 0$, $y = \pm \sqrt{9 - 0} = \pm 3$, one $x$ corresponds to two $y$ values. The vertical line $x = 0$ intersects the graph at $(0, 3)$ and $(0, -3)$, two points.

---

**6.**
Separate the constant:

$$
f(x) = \frac{3x-1}{x+2} = \frac{3(x+2) - 7}{x+2} = 3 - \frac{7}{x+2}
$$

Since $\dfrac{7}{x+2} \neq 0$, $f(x) \neq 3$. Range is $\mathbb{R} \setminus \{3\}$.

One–one test: Suppose $f(a) = f(b)$:

$$
3 - \frac{7}{a+2} = 3 - \frac{7}{b+2} \Rightarrow \frac{7}{a+2} = \frac{7}{b+2} \Rightarrow a+2 = b+2 \Rightarrow a = b
$$

Therefore $f$ is one–one.

---

### II. Linear and Cubic Functions

**7.**
Parallel lines have the same slope, $m = 3$.
Point-slope form: $y - (-1) = 3(x - 2) \Rightarrow y + 1 = 3x - 6 \Rightarrow y = 3x - 7$.

---

**8.**
(i) $f(1) = 1 - 2 - 5 + 6 = 0$, so $x-1$ is a factor.

Synthetic division:

$$
\begin{array}{c|ccc}
1 & 1 & -2 & -5 & 6 \\
  &   & 1  & -1 & -6 \\
\hline
  & 1 & -1 & -6 & 0
\end{array}
$$

Quotient: $x^2 - x - 6 = (x-3)(x+2)$.

Therefore $f(x) = (x-1)(x-3)(x+2)$.

(ii) Solutions of $f(x) = 0$: $x = 1, 3, -2$.

---

**9.**
$f'(x) = 3x^2 - 6x - 9 = 3(x^2 - 2x - 3) = 3(x-3)(x+1)$.

Set $f'(x) = 0$: $x = -1$ or $x = 3$.

Sign test:
- $x < -1$ (take $x = -2$): $f'(-2) = 3(-5)(-1) = 15 > 0$, increasing
- $-1 < x < 3$ (take $x = 0$): $f'(0) = 3(-3)(1) = -9 < 0$, decreasing
- $x > 3$ (take $x = 4$): $f'(4) = 3(1)(5) = 15 > 0$, increasing

$x = -1$: increasing → decreasing → **local maximum**, $f(-1) = -1 - 3 + 9 + 11 = 16$.
$x = 3$: decreasing → increasing → **local minimum**, $f(3) = 27 - 27 - 27 + 11 = -16$.

---

**10.**
Three roots: $x = -1, 2, 4$. Leading coefficient $a = 1 > 0$.

Sign analysis:

| Interval | $x+1$ | $x-2$ | $x-4$ | Product |
|------|-------|-------|-------|------|
| $x < -1$ | neg | neg | neg | **neg** |
| $-1 < x < 2$ | pos | neg | neg | **pos** |
| $2 < x < 4$ | pos | pos | neg | **neg** |
| $x > 4$ | pos | pos | pos | **pos** |

$f(x) > 0$ for $-1 < x < 2$ or $x > 4$.

---

**11.**
By the factor theorem, $f(-2) = 0$:

$$
f(-2) = (-2)^3 + k(4) - 5(-2) - 6 = -8 + 4k + 10 - 6 = 4k - 4 = 0
$$

$k = 1$.

Synthetic division by $(x+2)$:

$$
\begin{array}{c|ccc}
-2 & 1 & 1 & -5 & -6 \\
   &   & -2 & 2 & 6 \\
\hline
   & 1 & -1 & -3 & 0
\end{array}
$$

Quotient: $x^2 - x - 3$.

Therefore $f(x) = (x+2)(x^2 - x - 3)$. The quadratic cannot be further factorised over the rationals.

---

### III. Exponentials and Logarithms

**12.**

$$
\log_3 54 - \log_3 2 = \log_3 \frac{54}{2} = \log_3 27 = 3
$$

$$
3 + \log_3 \frac13 = \log_3 \left(27 \times \frac13\right) = \log_3 9 = 2
$$

The value is $2$.

---

**13.**

$$
2^{x+1} = 5 \Rightarrow \ln(2^{x+1}) = \ln 5 \Rightarrow (x+1)\ln 2 = \ln 5
$$

$$
x+1 = \frac{\ln 5}{\ln 2} \Rightarrow x = \frac{\ln 5}{\ln 2} - 1
$$

---

**14.**

$$
\log_3[(x+2)(x-4)] = 2 \Rightarrow (x+2)(x-4) = 3^2 = 9
$$

$$
x^2 - 2x - 8 = 9 \Rightarrow x^2 - 2x - 17 = 0
$$

$$
x = \frac{2 \pm \sqrt{4 + 68}}{2} = \frac{2 \pm \sqrt{72}}{2} = \frac{2 \pm 6\sqrt{2}}{2} = 1 \pm 3\sqrt{2}
$$

Check domain: $x+2 > 0$ and $x-4 > 0 \Rightarrow x > 4$.

$1 + 3\sqrt{2} \approx 5.24 > 4$, valid.
$1 - 3\sqrt{2} \approx -3.24 < 4$, rejected.

Therefore $x = 1 + 3\sqrt{2}$.

---

**15.**
Let $u = 3^x > 0$, then $3^{2x} = (3^x)^2 = u^2$.

$$
u^2 - 10u + 9 = 0 \Rightarrow (u-1)(u-9) = 0 \Rightarrow u = 1 \text{ or } u = 9
$$

$3^x = 1 \Rightarrow x = 0$.
$3^x = 9 \Rightarrow x = 2$.

Solutions are $x = 0$ or $x = 2$.

---

**16.**
Use the change of base formula, converting everything to natural logarithms:

$$
\log_2 3 = \frac{\ln 3}{\ln 2}, \quad \log_3 4 = \frac{\ln 4}{\ln 3}, \quad \log_4 5 = \frac{\ln 5}{\ln 4}, \quad \log_5 2 = \frac{\ln 2}{\ln 5}
$$

The product is:

$$
\frac{\ln 3}{\ln 2} \cdot \frac{\ln 4}{\ln 3} \cdot \frac{\ln 5}{\ln 4} \cdot \frac{\ln 2}{\ln 5} = 1
$$

The value is $1$ (all terms cancel out).

---

**17.**
Horizontal asymptote: as $x \to -\infty$, $e^x \to 0$, $2e^x - 3 \to -3$, asymptote is $y = -3$.

$y$-intercept: $f(0) = 2e^0 - 3 = 2 - 3 = -1$, i.e., $(0, -1)$.

$x$-intercept: $2e^x - 3 = 0 \Rightarrow e^x = \dfrac32 \Rightarrow x = \ln\dfrac32$, i.e., $\left(\ln\dfrac32, 0\right)$.

---

**18.**
$3^x < 7 \Rightarrow \ln(3^x) < \ln 7 \Rightarrow x\ln 3 < \ln 7 \Rightarrow x < \dfrac{\ln 7}{\ln 3}$.

---

**19.**
$\log_a 21 = \log_a (3 \times 7) = \log_a 3 + \log_a 7 = p + q$.

$\log_a \dfrac73 = \log_a 7 - \log_a 3 = q - p$.

---

**20.**
Use the change of base formula to convert $\log_4 x$ to base $2$:

$$
\log_4 x = \frac{\log_2 x}{\log_2 4} = \frac{\log_2 x}{2}
$$

Let $u = \log_2 x$, then the equation becomes:

$$
u + \frac{u}{2} = 3 \Rightarrow \frac{3u}{2} = 3 \Rightarrow u = 2
$$

$\log_2 x = 2 \Rightarrow x = 2^2 = 4$.

---

### IV. Inverse Functions and Composite Functions

**21.**
$y = \dfrac{3x-2}{4} \Rightarrow 4y = 3x - 2 \Rightarrow 3x = 4y + 2 \Rightarrow x = \dfrac{4y+2}{3}$.

Swap: $f^{-1}(x) = \dfrac{4x+2}{3}$.

---

**22.**
Complete the square: $f(x) = (x+1)^2 - 1$, $x \geq -1$. Range is $[-1, \infty)$.

Let $y = (x+1)^2 - 1 \Rightarrow y+1 = (x+1)^2 \Rightarrow x+1 = \sqrt{y+1}$ (since $x \geq -1$, take the positive root).

$x = \sqrt{y+1} - 1$.

Swap: $f^{-1}(x) = \sqrt{x+1} - 1$, domain $[-1, \infty)$.

---

**23.**
$fg(x) = f(g(x)) = f\left(\dfrac1x\right) = 2\left(\dfrac1x\right) + 1 = \dfrac{2}{x} + 1$, $x \neq 0$.

$gf(x) = g(f(x)) = g(2x+1) = \dfrac{1}{2x+1}$.

Domain of $gf(x)$: $2x+1 \neq 0 \Rightarrow x \neq -\dfrac12$, i.e., $\mathbb{R} \setminus \left\{-\dfrac12\right\}$.

---

**24.**
$y = e^{3x} \Rightarrow \ln y = 3x \Rightarrow x = \dfrac13\ln y$.

Swap: $f^{-1}(x) = \dfrac13\ln x$, domain $x > 0$.

---

**25.**
$y = \ln(x+2) \Rightarrow e^y = x+2 \Rightarrow x = e^y - 2$.

Swap: $f^{-1}(x) = e^x - 2$.

The range of the original function is $\mathbb{R}$, so the domain of $f^{-1}$ is $\mathbb{R}$.

Verification: $f(f^{-1}(x)) = \ln(e^x - 2 + 2) = \ln(e^x) = x$. $\checkmark$

---

**26.**
$f(x) = x^4$ **is not one–one** because different $x$ values correspond to the same $y$ value. For example, $f(2) = 16$ and $f(-2) = 16$, i.e., $2 \neq -2$ but $f(2) = f(-2)$. The horizontal line $y = 16$ intersects the graph of $y = x^4$ at $(2, 16)$ and $(-2, 16)$, two points. Therefore $f$ has no inverse.

> If we restrict the domain to $x \geq 0$, then the inverse is $f^{-1}(x) = \sqrt[4]{x}$.

---

**27.**
$fg(x) = f(g(x)) = \sqrt{(x^2 - 4) + 1} = \sqrt{x^2 - 3}$.

Domain: $f(x) = \sqrt{x+1}$ has domain $x+1 \geq 0 \Rightarrow x \geq -1$.

So $g(x) \geq -1 \Rightarrow x^2 - 4 \geq -1 \Rightarrow x^2 \geq 3 \Rightarrow |x| \geq \sqrt{3}$.

Domain is $(-\infty, -\sqrt{3}] \cup [\sqrt{3}, \infty)$.

---

**28.**
$f(x) = x^2$, $x \geq 0$, domain $[0, \infty)$.
$g(x) = 2x + 1$, domain $\mathbb{R}$.

$gf(x) = g(f(x)) = 2x^2 + 1$.

Domain of $gf$: $x$ must be in $f$'s domain ($x \geq 0$), and $f(x)$ must be in $g$'s domain ($\mathbb{R}$, no restriction).

Therefore $\text{Domain}(gf) = [0, \infty)$.

$\text{Domain}(f) = [0, \infty)$, so $\text{Domain}(gf) \subseteq \text{Domain}(f)$ holds (in fact they are equal). $\checkmark$

---

### V. Absolute Value Functions

**29.**
V-shape, cusp at $(2, 0)$.
$x \geq 2$: $y = x-2$; $x < 2$: $y = 2-x$.

Solve $|x-2| = 3$:
Case 1: $x-2 = 3 \Rightarrow x = 5$
Case 2: $x-2 = -3 \Rightarrow x = -1$

Solutions: $x = 5$ or $x = -1$.

---

**30.**
$|2x+1| < 5 \Rightarrow -5 < 2x+1 < 5$.

Left: $-5 < 2x+1 \Rightarrow -6 < 2x \Rightarrow -3 < x$.
Right: $2x+1 < 5 \Rightarrow 2x < 4 \Rightarrow x < 2$.

Intersection: $-3 < x < 2$.

---

**31.**
$y = |\cos x|$ on $[0, 2\pi]$:
- $[0, \frac{\pi}{2}]$: $\cos x \geq 0$, decreasing from $(0,1)$ to $(\frac{\pi}{2}, 0)$
- $[\frac{\pi}{2}, \frac{3\pi}{2}]$: $\cos x \leq 0$, reflected upward: from $(\frac{\pi}{2}, 0)$ up to $(\pi, 1)$ then down to $(\frac{3\pi}{2}, 0)$
- $[\frac{3\pi}{2}, 2\pi]$: $\cos x \geq 0$, increasing from $(\frac{3\pi}{2}, 0)$ to $(2\pi, 1)$

Period is $\pi$. Cusps at $x = \dfrac{\pi}{2}, \dfrac{3\pi}{2}$, etc.

---

**32.**
$x^2 - 5x + 6 = (x-2)(x-3)$.

Case 1: $x^2 - 5x + 6 = 2 \Rightarrow x^2 - 5x + 4 = 0 \Rightarrow (x-1)(x-4) = 0 \Rightarrow x = 1$ or $x = 4$.
Check: $x=1$ gives $1-5+6=2>0$, valid. $x=4$ gives $16-20+6=2>0$, valid.

Case 2: $x^2 - 5x + 6 = -2 \Rightarrow x^2 - 5x + 8 = 0$.
$\Delta = 25 - 32 = -7 < 0$, no real solutions.

Solutions: $x = 1$ or $x = 4$.

---

**33.**
$|x+2| \geq 3 \Rightarrow x+2 \leq -3$ or $x+2 \geq 3$.

$x+2 \leq -3 \Rightarrow x \leq -5$.
$x+2 \geq 3 \Rightarrow x \geq 1$.

Solution: $x \leq -5$ or $x \geq 1$.

---

**34.**
Geometric interpretation: $|x-2|$ is the distance from $x$ to $2$, $|x+1| = |x-(-1)|$ is the distance from $x$ to $-1$. $f(x)$ is the sum of these two distances.

The distance on the number line from $-1$ to $2$ is $3$. When $x$ lies between $[-1, 2]$, the sum of the two distances is always $3$. When $x < -1$ or $x > 2$, the sum is greater than $3$.

Therefore the minimum value is $3$, attained for $x \in [-1, 2]$.

Algebraic verification:

$$
f(x) = \begin{cases}
-(x-2) - (x+1) = -2x + 1, & x < -1 \\
-(x-2) + (x+1) = 3, & -1 \leq x \leq 2 \\
(x-2) + (x+1) = 2x - 1, & x > 2
\end{cases}
$$

When $x < -1$, $f(x) = -2x + 1 > 3$.
When $-1 \leq x \leq 2$, $f(x) = 3$.
When $x > 2$, $f(x) = 2x - 1 > 3$.

The minimum value is $3$.

---

### VI. Trigonometric Absolute Values

**35.**
$y = 2\cos x + 1$ on $[0, 2\pi]$:
- Maximum: $2(1) + 1 = 3$ ($x = 0, 2\pi$)
- Minimum: $2(-1) + 1 = -1$ ($x = \pi$)
- Zeros: $2\cos x + 1 = 0 \Rightarrow \cos x = -\dfrac12 \Rightarrow x = \dfrac{2\pi}{3}, \dfrac{4\pi}{3}$

After taking absolute value:
- On $[\frac{2\pi}{3}, \frac{4\pi}{3}]$, $2\cos x + 1 \leq 0$, reflected upward
- Remaining parts unchanged
- Cusps: $x = \dfrac{2\pi}{3}$ and $x = \dfrac{4\pi}{3}$
- After reflection, the maximum occurs at $x = \pi$: $|2\cos\pi + 1| = |-2+1| = 1$
- Original maxima at $x = 0$ (value $3$) and $x = 2\pi$ (value $3$) remain unchanged

Range: $[0, 3]$.

---

**36.**
$y = |\tan x|$ on $(-\frac{\pi}{2}, \frac{\pi}{2})$:

- $(-\frac{\pi}{2}, 0)$: $\tan x < 0$, reflected upward, $|\tan x| = -\tan x$
- $(0, \frac{\pi}{2})$: $\tan x > 0$, unchanged, $|\tan x| = \tan x$
- $x = 0$: $\tan 0 = 0$, cusp

**Asymptotes**: $x = -\dfrac{\pi}{2}$ and $x = \dfrac{\pi}{2}$ are still vertical asymptotes (absolute value does not change the position of asymptotes).

Graph features:
- Cusp at $x = 0$
- As $x \to \pm\frac{\pi}{2}$, $|\tan x| \to \infty$
- Range: $[0, \infty)$
- Graph is symmetric about $x = 0$ (even function), because $|\tan(-x)| = |-\tan x| = |\tan x|$

---

**37.**
$f(x) = |3\sin 2x - 2|$, $x \in [0, \pi]$.

First analyse $y = 3\sin 2x - 2$:
- Amplitude $3$, period $\pi$, shifted down by $2$
- Maximum: $3(1) - 2 = 1$, minimum: $3(-1) - 2 = -5$
- Zeros: $3\sin 2x - 2 = 0 \Rightarrow \sin 2x = \dfrac23$
  $2x = \arcsin\dfrac23$ or $2x = \pi - \arcsin\dfrac23$
  Let $\alpha = \dfrac12\arcsin\dfrac23 \approx 0.364$ radians
  Then $x = \alpha$ or $x = \dfrac{\pi}{2} - \alpha$

On $[0, \pi]$, $3\sin 2x - 2$ is negative on $[\alpha, \frac{\pi}{2} - \alpha]$, so this part is reflected upward.

Maximum: after reflection, the original minimum $-5$ (at $x = \dfrac{3\pi}{4}$) becomes $5$. So the maximum of $f(x)$ is $5$.
Minimum: $0$ (at the zeros $x = \alpha$ and $x = \dfrac{\pi}{2} - \alpha$).

Therefore $f(x)$ on $[0, \pi]$ has maximum $5$ and minimum $0$.

---

### VII. Domain Restrictions and Existence of Composite Functions

**38.**
$f(x) = \sqrt{x-2}$, domain $[2, \infty)$.
$g(x) = \dfrac{1}{\sqrt{5-x}}$, domain $x < 5$.

$gf(x) = g(f(x)) = \dfrac{1}{\sqrt{5 - \sqrt{x-2}}}$.

Domain conditions:
1. $f$'s domain: $x \geq 2$
2. $f(x)$ must be in $g$'s domain:
   - $5 - \sqrt{x-2} > 0$ (denominator radicand must be positive)
   - $\sqrt{x-2} < 5 \Rightarrow x-2 < 25 \Rightarrow x < 27$
   - $5 - \sqrt{x-2} \neq 0$ is already guaranteed by $>0$

Intersection: $2 \leq x < 27$.

Verification $\text{Domain}(gf) \subseteq \text{Domain}(f)$:
$\text{Domain}(f) = [2, \infty)$, $\text{Domain}(gf) = [2, 27) \subset [2, \infty)$. $\checkmark$

---

> **Study tips**: Functions are the cornerstone of IGCSE 0606 Additional Mathematics — differentiation, integration, curve sketching, and kinematics are all built upon the concept of functions. The key points of this chapter are:
>
> 1. Master the calculation of domain and range (especially when roots, denominators, and logarithms appear together)
> 2. Deeply understand the inverse relationship between exponentials and logarithms ($a^{\log_a x} = x$, $\log_a(a^x) = x$)
> 3. Master the flexible use of logarithm laws (especially the change of base formula $\log_a M = \dfrac{\log_b M}{\log_b a}$)
> 4. Be proficient in finding inverse functions and composite functions, paying attention to changes in domain
> 5. Be able to sketch transformed graphs of $|f(x)|$ (linear, quadratic, cubic, trigonometric of the forms $a\sin bx + c$, $a\cos bx + c$, $a\tan bx + c$)
> 6. Be able to explain in words why a function has no inverse (Syllabus 1.5)
> 7. Understand $\text{Domain}(gf) \subseteq \text{Domain}(f)$ and $\text{Range}(gf) \subseteq \text{Range}(g)$ (Syllabus 1.2)

---
---

# Chapter 5: Differentiation (Derivatives)

## Syllabus Mapping

This chapter covers the following entries from **Unit 14: Calculus** of the **Cambridge IGCSE Additional Mathematics (0606) 2028–2030 syllabus**:

| Syllabus Ref | Content | Section |
|---------|------|---------|
| 14.1 | Understand the concept of a derivative (informal understanding of limits; differentiation from first principles is not required) | 5.1 |
| 14.2 | Use notation $f'(x), f''(x), \frac{dy}{dx}, \frac{d^2y}{dx^2}, \delta x, \delta x \to 0$ | 5.1 |
| 14.3 | Know and use derivatives of standard functions: $x^n$ (any rational $n$), $\sin x$, $\cos x$, $\tan x$, $e^x$, $\ln x$ (including constant multiples, sums/differences, composite functions) | 5.2, 5.3 |
| 14.4 | Product rule and quotient rule | 5.4 |
| 14.5 | Find tangents and normals | 5.5 |
| 14.6 | Find stationary points (points of inflexion not required) | 5.6 |
| 14.7 | Connected rates of change, small increments and approximations | 5.7 |
| 14.8 | Practical maxima and minima problems | 5.8 |
| 14.9 | Use first and second derivative tests to distinguish between maxima and minima | 5.6 |

**Core requirements**:
- Angles in trigonometric functions **must always be in radians**.
- Differentiation from first principles is **not required**.
- Points of inflexion are **not required**.
- The second derivative test requires a complete justification of the conclusion.

---

## Introduction

Differentiation is one of the two core operations of calculus. Its task is to quantify **change** — specifically, to quantify the **instantaneous rate of change** of a function at any given point.

Imagine you are driving along a winding road. The reading on your speedometer is the **instantaneous velocity** — it tells you how fast the car is changing at that exact moment. What differentiation does is calculate this kind of "instantaneous speed" for any function. Geometrically, the derivative gives the **slope of the tangent line** to the curve at a given point — that is, how "steep" the curve is at that point.

Why study differentiation? Because almost everything in nature is changing: the motion of objects, the growth of populations, the rise and fall of temperatures, the fluctuations of profit. Differentiation gives us a precise mathematical tool to describe these changes. Once you master differentiation, subsequent topics like integration (finding accumulated quantities), optimisation (finding the best solution), and kinematics analysis will all fall into place.

This chapter starts from the basic concept of the derivative, then covers basic differentiation formulas, the chain rule, the product rule and the quotient rule, and then applies these tools to tangents and normals, determining extreme values, connected rates of change, and practical maxima and minima problems. Each topic is accompanied by numerous worked examples and practice problems to ensure thorough understanding.

---

## 5.1 The Concept of the Derivative and Notation

### 5.1.1 From Average Rate of Change to Instantaneous Rate of Change

Rate of change is a concept we are very familiar with. For example, if a car travels 120 kilometres in 2 hours, its **average speed** is:

$$
\text{Average speed} = \frac{120}{2} = 60 \text{ km/h}
$$

But this average speed hides the details — the car may be fast at some moments and slow at others. If we want to know the speed **at a precise moment**, we need the instantaneous rate of change.

Let $y = f(x)$. Consider a small interval from $x$ to $x + \delta x$ (where $\delta x$ is read as "delta x", representing a small change in $x$). Over this interval, the average rate of change of the function is:

$$
\frac{\text{Change in function value}}{\text{Change in independent variable}} = \frac{f(x + \delta x) - f(x)}{\delta x}
$$

As $\delta x$ approaches $0$, this average rate of change approaches a limiting value — this is the **derivative** of the function at point $x$:

$$
\boxed{f'(x) = \lim_{\delta x \to 0} \frac{f(x + \delta x) - f(x)}{\delta x}}
$$

Here $\lim_{\delta x \to 0}$ means "as $\delta x$ tends to $0$". Whether this limit exists (i.e., whether the derivative exists) depends on whether the function is "smooth" at that point.

### 5.1.2 Geometric Meaning of the Derivative

Geometrically, the derivative $f'(a)$ is the **slope of the tangent line** to the curve $y = f(x)$ at the point $(a, f(a))$.

- If $f'(a) > 0$, the curve is **increasing** at that point (the tangent slopes upward to the right).
- If $f'(a) < 0$, the curve is **decreasing** at that point (the tangent slopes downward to the right).
- If $f'(a) = 0$, the curve is **horizontal** at that point (could be a maximum, a minimum, or a saddle point).

### 5.1.3 Notation

There are several notations for derivatives commonly seen in exams:

| Notation | Name | Example |
|-----|------|------|
| $f'(x)$ | Lagrange notation | $f'(x) = 2x$ |
| $\frac{dy}{dx}$ | Leibniz notation | $\frac{dy}{dx} = 2x$ |
| $\frac{d}{dx}f(x)$ | Operator notation | $\frac{d}{dx}(x^2) = 2x$ |
| $f''(x)$, $\frac{d^2y}{dx^2}$ | Second derivative | Derivative of the derivative |

> ⚠️ **Important understanding**: The notation $\frac{dy}{dx}$ is not a fraction, but a single symbol representing the result of the operation "differentiate with respect to $x$". However, in small increment approximations, we can treat it as a "ratio" ($\delta y \approx \frac{dy}{dx} \cdot \delta x$), which is very effective for linear approximations.

### 5.1.4 Intuitive Understanding of Limits

In the process of differentiation, we often encounter the indeterminate form $\frac{0}{0}$. The usual method is to **factorise and cancel** before substituting.

**Example**: Evaluate $\lim_{x \to 2} \frac{x^2 - 4}{x - 2}$.

When $x = 2$, both numerator and denominator are $0$, but we can do this:

$$
\lim_{x \to 2} \frac{x^2 - 4}{x - 2} = \lim_{x \to 2} \frac{(x-2)(x+2)}{x-2} = \lim_{x \to 2} (x+2) = 4
$$

Note: $x$ approaches $2$ but never equals $2$, so cancelling $x-2$ is valid.

---

### Worked Example 5.1A (Intuitive Understanding of the Derivative Concept)

> Given $f(x) = x^2$, use the limit definition to find $f'(2)$.

**Solution**:

$$
f'(2) = \lim_{\delta x \to 0} \frac{f(2 + \delta x) - f(2)}{\delta x}
= \lim_{\delta x \to 0} \frac{(2 + \delta x)^2 - 4}{\delta x}
$$

Expanding $(2 + \delta x)^2 = 4 + 4\delta x + (\delta x)^2$ and substituting:

$$
f'(2) = \lim_{\delta x \to 0} \frac{4 + 4\delta x + (\delta x)^2 - 4}{\delta x}
= \lim_{\delta x \to 0} \frac{4\delta x + (\delta x)^2}{\delta x}
= \lim_{\delta x \to 0} (4 + \delta x)
$$

As $\delta x \to 0$, $4 + \delta x \to 4$, so $f'(2) = 4$.

**Geometric meaning**: The slope of the tangent line to the parabola $y = x^2$ at the point $(2, 4)$ is $4$.

---

### Worked Example 5.1B (Comparing Average and Instantaneous Rates of Change)

> An object in free fall has displacement $s(t) = 5t^2$ ($s$ in metres, $t$ in seconds).
> (a) Find the average velocity from $t = 2$ to $t = 2.1$.
> (b) Find the instantaneous velocity at $t = 2$.

**Solution**:

(a) Average velocity:

$$
\text{Average velocity} = \frac{s(2.1) - s(2)}{0.1} = \frac{5(4.41) - 5(4)}{0.1}
= \frac{22.05 - 20}{0.1} = \frac{2.05}{0.1} = 20.5 \text{ m/s}
$$

(b) Instantaneous velocity. First find the derivative in general:

$$
s'(t) = \lim_{\delta t \to 0} \frac{5(t + \delta t)^2 - 5t^2}{\delta t}
= \lim_{\delta t \to 0} \frac{5(t^2 + 2t\delta t + (\delta t)^2) - 5t^2}{\delta t}
$$

$$
= \lim_{\delta t \to 0} \frac{10t\delta t + 5(\delta t)^2}{\delta t}
= \lim_{\delta t \to 0} (10t + 5\delta t) = 10t
$$

Substituting $t = 2$: $s'(2) = 10 \times 2 = 20$ m/s.

Note: The average velocity $20.5$ m/s is very close to the instantaneous velocity $20$ m/s — the smaller the interval, the closer they become.

---

### Worked Example 5.1C (Relationship Between Derivative Value and Tangent Slope)

> What is the slope of the tangent to the curve $y = \frac{1}{x}$ at the point $(2, \frac{1}{2})$? Is the curve rising or falling at that point?

**Solution**:

$$
f'(x) = \lim_{\delta x \to 0} \frac{\frac{1}{x + \delta x} - \frac{1}{x}}{\delta x}
= \lim_{\delta x \to 0} \frac{\frac{x - (x + \delta x)}{x(x + \delta x)}}{\delta x}
= \lim_{\delta x \to 0} \frac{-\delta x}{x(x + \delta x)\delta x}
$$

$$
= \lim_{\delta x \to 0} \frac{-1}{x(x + \delta x)} = -\frac{1}{x^2}
$$

Substituting $x = 2$: $f'(2) = -\frac{1}{4}$.

The slope is negative, so the curve is **falling** at $x = 2$ (as $x$ increases, $y$ decreases).

---

### Worked Example 5.1D (Limit Calculation — Cancellation Method)

> Evaluate $\lim_{x \to 3} \frac{x^2 - 2x - 3}{x - 3}$.

**Solution**:

When $x = 3$, the numerator $3^2 - 2(3) - 3 = 9 - 6 - 3 = 0$, and the denominator is also $0$. Factorise the numerator:

$$
x^2 - 2x - 3 = (x - 3)(x + 1)
$$

Therefore:

$$
\lim_{x \to 3} \frac{x^2 - 2x - 3}{x - 3} = \lim_{x \to 3} \frac{(x - 3)(x + 1)}{x - 3} = \lim_{x \to 3} (x + 1) = 4
$$

---

### Practice Problems 5.1

1. Use the limit definition to find the derivative of $f(x) = x^2 + 2x$ at $x = 1$.
2. An object's displacement is $s(t) = 2t^2 + 3t$ ($t \ge 0$). Find the instantaneous velocity at $t = 3$.
3. Evaluate $\lim_{x \to 4} \frac{x^2 - 16}{x - 4}$.

---

## 5.2 Basic Differentiation Formulas

Now that we have the concept of the derivative, we need an efficient set of tools for differentiation, rather than using the limit definition every time. Below are the most basic differentiation formulas, which must be mastered thoroughly.

### 5.2.1 Derivation of the Power Rule

For $f(x) = x^n$, where $n$ is a positive integer, we first derive using the Binomial Theorem.

From the definition of the derivative:

$$
f'(x) = \lim_{\delta x \to 0} \frac{(x + \delta x)^n - x^n}{\delta x}
$$

By the Binomial Theorem:

$$
(x + \delta x)^n = x^n + nx^{n-1}\delta x + \frac{n(n-1)}{2}x^{n-2}(\delta x)^2 + \cdots + (\delta x)^n
$$

Substituting:

$$
f'(x) = \lim_{\delta x \to 0} \frac{nx^{n-1}\delta x + \frac{n(n-1)}{2}x^{n-2}(\delta x)^2 + \cdots + (\delta x)^n}{\delta x}
$$

$$
= \lim_{\delta x \to 0} \left[ nx^{n-1} + \frac{n(n-1)}{2}x^{n-2}\delta x + \cdots + (\delta x)^{n-1} \right]
$$

As $\delta x \to 0$, all terms except the first tend to $0$, so:

$$
\boxed{\frac{d}{dx}(x^n) = n x^{n-1}}
$$

This formula holds not only for positive integers but for **any rational number** $n$, as explicitly required by the syllabus.

The following table shows common cases:

| $f(x)$ | Rewritten as $x^n$ | $f'(x)$ | Explanation |
|--------|-----------------|---------|------|
| $x^2$ | $x^2$ | $2x$ | $n=2$ |
| $x^3$ | $x^3$ | $3x^2$ | $n=3$ |
| $x$ | $x^1$ | $1$ | $n=1$ |
| $1$ | $x^0$ | $0$ | $n=0$ |
| $\sqrt{x}$ | $x^{1/2}$ | $\frac{1}{2}x^{-1/2} = \frac{1}{2\sqrt{x}}$ | $n = \frac{1}{2}$ |
| $\frac{1}{x}$ | $x^{-1}$ | $-x^{-2} = -\frac{1}{x^2}$ | $n = -1$ |
| $\frac{1}{x^2}$ | $x^{-2}$ | $-2x^{-3} = -\frac{2}{x^3}$ | $n = -2$ |
| $\sqrt[3]{x}$ | $x^{1/3}$ | $\frac{1}{3}x^{-2/3} = \frac{1}{3\sqrt[3]{x^2}}$ | $n = \frac{1}{3}$ |

### 5.2.2 Constant Multiple and Sum/Difference Rules

Differentiating linear combinations of functions is very straightforward:

- **Constant multiple rule**: $\frac{d}{dx}[c \cdot f(x)] = c \cdot f'(x)$
  - Derivation: $\lim_{\delta x \to 0} \frac{c f(x+\delta x) - c f(x)}{\delta x} = c \cdot \lim_{\delta x \to 0} \frac{f(x+\delta x) - f(x)}{\delta x} = c f'(x)$

- **Sum rule**: $\frac{d}{dx}[f(x) + g(x)] = f'(x) + g'(x)$
  - Derivation: $\lim_{\delta x \to 0} \frac{[f(x+\delta x)+g(x+\delta x)] - [f(x)+g(x)]}{\delta x} = \lim_{\delta x \to 0} \frac{f(x+\delta x)-f(x)}{\delta x} + \lim_{\delta x \to 0} \frac{g(x+\delta x)-g(x)}{\delta x} = f'(x) + g'(x)$

- **Difference rule**: $\frac{d}{dx}[f(x) - g(x)] = f'(x) - g'(x)$

**Example**: $f(x) = 3x^2 - 4x + 5$

$$
f'(x) = 3 \cdot (2x) - 4 \cdot (1) + 0 = 6x - 4
$$

### 5.2.3 Derivatives of Trigonometric Functions

**Core condition**: All angles in trigonometric functions **must be in radians**.

Why must we use radians? Because in radians, $\lim_{\theta \to 0} \frac{\sin\theta}{\theta} = 1$. This limit is the foundation for differentiating trigonometric functions. If degrees were used, this limit would include an extra factor of $\frac{\pi}{180}$, and the derivative formulas would no longer be simple.

**Derivation of the derivative of $\sin x$**:

$$
\frac{d}{dx}(\sin x) = \lim_{\delta x \to 0} \frac{\sin(x+\delta x) - \sin x}{\delta x}
$$

Using the trigonometric identity $\sin(A+B) = \sin A\cos B + \cos A\sin B$:

$$
= \lim_{\delta x \to 0} \frac{\sin x\cos(\delta x) + \cos x\sin(\delta x) - \sin x}{\delta x}
$$

$$
= \lim_{\delta x \to 0} \left[ \sin x \cdot \frac{\cos(\delta x) - 1}{\delta x} + \cos x \cdot \frac{\sin(\delta x)}{\delta x} \right]
$$

Using the two important limits: $\lim_{\theta \to 0} \frac{\sin\theta}{\theta} = 1$ and $\lim_{\theta \to 0} \frac{\cos\theta - 1}{\theta} = 0$, we get:

$$
\frac{d}{dx}(\sin x) = \sin x \cdot 0 + \cos x \cdot 1 = \cos x
$$

Similarly, $\frac{d}{dx}(\cos x) = -\sin x$ can be derived.

For $\tan x$, we use $\tan x = \frac{\sin x}{\cos x}$ and the quotient rule (see Section 5.4).

Summary of standard formulas:

$$
\boxed{\frac{d}{dx}(\sin x) = \cos x}
$$

$$
\boxed{\frac{d}{dx}(\cos x) = -\sin x}
$$

$$
\boxed{\frac{d}{dx}(\tan x) = \sec^2 x}
$$

### 5.2.4 Derivatives of Exponential and Logarithmic Functions

$$
\boxed{\frac{d}{dx}(e^x) = e^x}
$$

This is one of the most beautiful formulas in calculus — the derivative of $e^x$ is itself. Geometrically, this means that at any point on the curve $y = e^x$, the slope of the tangent is equal to the function value at that point.

For a general exponential function $a^x$ ($a > 0, a \neq 1$):

$$
\frac{d}{dx}(a^x) = a^x \ln a
$$

**Derivation process**: Write $a^x$ as $e^{\ln(a^x)} = e^{x\ln a}$, then use the chain rule:

$$
\frac{d}{dx}(a^x) = \frac{d}{dx}(e^{x\ln a}) = e^{x\ln a} \cdot \ln a = a^x \ln a
$$

For the natural logarithm:

$$
\boxed{\frac{d}{dx}(\ln x) = \frac{1}{x}}
$$

For a logarithm with a general base:

$$
\frac{d}{dx}(\log_a x) = \frac{1}{x \ln a}
$$

**Derivation of the derivative of $\ln x$**:

Let $y = \ln x$, then $e^y = x$. Differentiate both sides with respect to $x$ (implicit differentiation):

$$
e^y \cdot \frac{dy}{dx} = 1 \quad \Rightarrow \quad \frac{dy}{dx} = \frac{1}{e^y} = \frac{1}{x}
$$

---

### Worked Example 5.2A (Differentiating Polynomials)

> Find the derivatives of the following functions:
> (a) $f(x) = 2x^5 - 3x^3 + 7x - 10$
> (b) $g(x) = \frac{1}{3}x^6 + \frac{4}{x^2} - \sqrt{x}$
> (c) $h(x) = (x+1)(x-2)$ (expand first, then differentiate)
> (d) $p(x) = 5x^4 + 2x^{-3} - 3x^{1/2} + 8$

**Solution**:

(a) Differentiate term by term:

$$
f'(x) = 2 \cdot 5x^4 - 3 \cdot 3x^2 + 7 - 0 = 10x^4 - 9x^2 + 7
$$

(b) First rewrite in power form: $\frac{4}{x^2} = 4x^{-2}$, $\sqrt{x} = x^{1/2}$.

$$
g(x) = \frac{1}{3}x^6 + 4x^{-2} - x^{1/2}
$$

$$
g'(x) = \frac{1}{3} \cdot 6x^5 + 4 \cdot (-2)x^{-3} - \frac{1}{2}x^{-1/2}
= 2x^5 - 8x^{-3} - \frac{1}{2}x^{-1/2}
$$

Writing in fraction form:

$$
g'(x) = 2x^5 - \frac{8}{x^3} - \frac{1}{2\sqrt{x}}
$$

(c) First expand: $(x+1)(x-2) = x^2 - x - 2$, then differentiate:

$$
h'(x) = 2x - 1
$$

(d)

$$
p'(x) = 5 \cdot 4x^3 + 2 \cdot (-3)x^{-4} - 3 \cdot \frac{1}{2}x^{-1/2} + 0
= 20x^3 - 6x^{-4} - \frac{3}{2}x^{-1/2}
$$

---

### Worked Example 5.2B (Differentiating Trigonometric Functions)

> Find the derivatives of the following functions:
> (a) $f(x) = 3\sin x - 2\cos x$
> (b) $g(x) = \tan x + 5$
> (c) Find $f'(0)$, where $f(x) = \sin x - \cos x$
> (d) $h(x) = 4\sin x + \frac{1}{2}\cos x$

**Solution**:

(a)

$$
f'(x) = 3\cos x - 2(-\sin x) = 3\cos x + 2\sin x
$$

(b)

$$
g'(x) = \sec^2 x + 0 = \sec^2 x
$$

(c) First differentiate: $f'(x) = \cos x + \sin x$

Substituting $x = 0$: $f'(0) = \cos 0 + \sin 0 = 1 + 0 = 1$

(d)

$$
h'(x) = 4\cos x + \frac{1}{2}(-\sin x) = 4\cos x - \frac{1}{2}\sin x
$$

---

### Worked Example 5.2C (Differentiating Exponential and Logarithmic Functions)

> Find the derivatives of the following functions:
> (a) $f(x) = 4e^x - \frac{1}{2}\ln x$
> (b) $g(x) = 3^x + \log_2 x$
> (c) Given $h(x) = e^x + \ln x$, find $h'(1)$
> (d) $p(x) = 5^x - 2e^x + 3\ln x$

**Solution**:

(a)

$$
f'(x) = 4e^x - \frac{1}{2} \cdot \frac{1}{x} = 4e^x - \frac{1}{2x}
$$

(b) Use formulas: $\frac{d}{dx}(3^x) = 3^x \ln 3$, $\frac{d}{dx}(\log_2 x) = \frac{1}{x\ln 2}$

$$
g'(x) = 3^x \ln 3 + \frac{1}{x\ln 2}
$$

(c) First differentiate: $h'(x) = e^x + \frac{1}{x}$

Substituting $x = 1$: $h'(1) = e^1 + \frac{1}{1} = e + 1$

(d)

$$
p'(x) = 5^x \ln 5 - 2e^x + 3 \cdot \frac{1}{x} = 5^x \ln 5 - 2e^x + \frac{3}{x}
$$

---

### Worked Example 5.2D (Comprehensive Differentiation — Rewriting First)

> Find the derivatives of the following functions:
> (a) $f(x) = \frac{2}{\sqrt[3]{x}}$
> (b) $g(x) = (2x)^3$ (note the difference from $2x^3$)

**Solution**:

(a) First rewrite: $\frac{2}{\sqrt[3]{x}} = 2x^{-1/3}$

$$
f'(x) = 2 \cdot \left(-\frac{1}{3}\right)x^{-4/3} = -\frac{2}{3}x^{-4/3} = -\frac{2}{3\sqrt[3]{x^4}}
$$

(b) $(2x)^3 = 8x^3$, so $g'(x) = 8 \cdot 3x^2 = 24x^2$

Note: If it were $2x^3$, the derivative would be $6x^2$ — they are different.

---

### Practice Problems 5.2

1. Find the derivative of $f(x) = 4x^3 - 2x^2 + 5x - 7$.
2. Find the derivative of $g(x) = \frac{3}{x^2} - \frac{1}{2\sqrt{x}} + 6x^{1/3}$.
3. Find the derivative of $h(x) = 5\sin x - 3\cos x + 2\tan x$.
4. Find the derivative of $p(x) = 2e^x + 4^x - \frac{1}{3}\ln x$.

---

## 5.3 Chain Rule

### 5.3.1 Principle of the Chain Rule

When we want to differentiate a composite function — for example, $y = (2x+1)^3$ or $y = \sin(3x)$ — we need the **chain rule**.

The core idea of the chain rule is "differentiate layer by layer, multiply as you go." Let $y$ be a function of $u$, and $u$ be a function of $x$, i.e., $y = f(u)$ and $u = g(x)$. Then:

$$
\boxed{\frac{dy}{dx} = \frac{dy}{du} \cdot \frac{du}{dx}}
$$

Written another way: if $y = f(g(x))$, then:

$$
\frac{dy}{dx} = f'(g(x)) \cdot g'(x)
$$

That is: **the derivative of the outer function with respect to the intermediate variable, multiplied by the derivative of the intermediate variable with respect to the independent variable**.

### 5.3.2 Intuitive Understanding of the Chain Rule

Why does the chain rule work? Consider small changes:

- When $x$ changes by $\delta x$, $u = g(x)$ changes by $\delta u \approx g'(x)\delta x$
- When $u$ changes by $\delta u$, $y = f(u)$ changes by $\delta y \approx f'(u)\delta u$

Therefore:

$$
\frac{\delta y}{\delta x} \approx \frac{f'(u)\delta u}{\delta x} \approx f'(u) \cdot \frac{\delta u}{\delta x} \approx f'(u) \cdot g'(x)
$$

As $\delta x \to 0$, the approximation becomes an exact equality.

### 5.3.3 Common Application Patterns of the Chain Rule

**Pattern 1**: $y = (ax+b)^n$

Let $u = ax + b$, then $y = u^n$, $\frac{dy}{du} = nu^{n-1}$, $\frac{du}{dx} = a$, so:

$$
\frac{dy}{dx} = n(ax+b)^{n-1} \cdot a = \boxed{a n (ax+b)^{n-1}}
$$

**Pattern 2**: $y = \sin(ax+b)$

Let $u = ax+b$, then $y = \sin u$, $\frac{dy}{du} = \cos u$, $\frac{du}{dx} = a$, so:

$$
\frac{dy}{dx} = \cos(ax+b) \cdot a = \boxed{a\cos(ax+b)}
$$

**Pattern 3**: $y = \cos(ax+b)$

$$
\frac{dy}{dx} = -\sin(ax+b) \cdot a = \boxed{-a\sin(ax+b)}
$$

**Pattern 4**: $y = e^{ax+b}$

Let $u = ax+b$, then $y = e^u$, $\frac{dy}{du} = e^u$, $\frac{du}{dx} = a$, so:

$$
\frac{dy}{dx} = e^{ax+b} \cdot a = \boxed{a e^{ax+b}}
$$

**Pattern 5**: $y = \ln(ax+b)$

Let $u = ax+b$, then $y = \ln u$, $\frac{dy}{du} = \frac{1}{u}$, $\frac{du}{dx} = a$, so:

$$
\frac{dy}{dx} = \frac{1}{ax+b} \cdot a = \boxed{\frac{a}{ax+b}}
$$

**Pattern 6**: $y = \tan(ax+b)$

$$
\frac{dy}{dx} = \sec^2(ax+b) \cdot a = \boxed{a\sec^2(ax+b)}
$$

### 5.3.4 Multi-layer Chain Rule

When a function has three or more layers of composition, the chain rule can be applied multiple times in succession. For example, $y = f(g(h(x)))$:

$$
\frac{dy}{dx} = f'(g(h(x))) \cdot g'(h(x)) \cdot h'(x)
$$

Start from the outermost layer and work inward, multiplying at each step.

---

### Worked Example 5.3A (Polynomial Composite Functions)

> Find the derivatives of the following functions:
> (a) $y = (3x - 2)^5$
> (b) $y = \frac{1}{(2x+1)^3}$
> (c) $y = \sqrt{4x - 1}$
> (d) $y = (5 - 2x)^{-4}$

**Solution**:

(a) Let $u = 3x - 2$, then $y = u^5$.

$$
\frac{dy}{dx} = 5u^4 \cdot 3 = 5(3x-2)^4 \cdot 3 = 15(3x-2)^4
$$

(b) Write as $y = (2x+1)^{-3}$, let $u = 2x+1$.

$$
\frac{dy}{dx} = (-3)u^{-4} \cdot 2 = -6(2x+1)^{-4} = -\frac{6}{(2x+1)^4}
$$

(c) Write as $y = (4x-1)^{1/2}$, let $u = 4x-1$.

$$
\frac{dy}{dx} = \frac{1}{2}u^{-1/2} \cdot 4 = \frac{1}{2}(4x-1)^{-1/2} \cdot 4 = \frac{2}{\sqrt{4x-1}}
$$

(d) Let $u = 5 - 2x$, then $y = u^{-4}$.

$$
\frac{dy}{dx} = (-4)u^{-5} \cdot (-2) = 8(5-2x)^{-5} = \frac{8}{(5-2x)^5}
$$

---

### Worked Example 5.3B (Trigonometric and Exponential Composite Functions)

> Find the derivatives of the following functions:
> (a) $y = \sin\left(2x + \frac{\pi}{3}\right)$
> (b) $y = e^{-3x + 1}$
> (c) $y = \tan(5x)$
> (d) $y = \cos\left(\frac{x}{2}\right)$

**Solution**:

(a) Let $u = 2x + \frac{\pi}{3}$, then $y = \sin u$.

$$
\frac{dy}{dx} = \cos u \cdot 2 = 2\cos\left(2x + \frac{\pi}{3}\right)
$$

(b) Let $u = -3x + 1$, then $y = e^u$.

$$
\frac{dy}{dx} = e^u \cdot (-3) = -3e^{-3x+1}
$$

(c) Let $u = 5x$, then $y = \tan u$.

$$
\frac{dy}{dx} = \sec^2 u \cdot 5 = 5\sec^2(5x)
$$

(d) Let $u = \frac{x}{2}$, then $y = \cos u$.

$$
\frac{dy}{dx} = -\sin u \cdot \frac{1}{2} = -\frac{1}{2}\sin\left(\frac{x}{2}\right)
$$

---

### Worked Example 5.3C (Logarithmic Composite and Multi-layer Chain Rule)

> Find the derivatives of the following functions:
> (a) $y = \ln(3x^2 + 1)$
> (b) $y = e^{\sin x}$
> (c) $y = \sin^3 x$ (i.e., $(\sin x)^3$)
> (d) $y = \sqrt{\cos x}$

**Solution**:

(a) Let $u = 3x^2 + 1$, then $y = \ln u$.

$$
\frac{dy}{dx} = \frac{1}{u} \cdot 6x = \frac{6x}{3x^2 + 1}
$$

(b) Let $u = \sin x$, then $y = e^u$.

$$
\frac{dy}{dx} = e^u \cdot \cos x = e^{\sin x} \cdot \cos x
$$

(c) There are two layers: let $u = \sin x$, $y = u^3$, then:

$$
\frac{dy}{dx} = 3u^2 \cdot \cos x = 3\sin^2 x \cdot \cos x
$$

(d) Write as $y = (\cos x)^{1/2}$, let $u = \cos x$, $y = u^{1/2}$.

$$
\frac{dy}{dx} = \frac{1}{2}u^{-1/2} \cdot (-\sin x) = \frac{1}{2}(\cos x)^{-1/2} \cdot (-\sin x) = -\frac{\sin x}{2\sqrt{\cos x}}
$$

---

### Worked Example 5.3D (Three-layer Chain Rule)

> Find the derivative of $y = \sin^2(3x)$.

**Solution**:

There are three layers: $y = (\sin(3x))^2$

Let $v = 3x$, $u = \sin v$, $y = u^2$.

$$
\frac{dy}{dx} = \frac{dy}{du} \cdot \frac{du}{dv} \cdot \frac{dv}{dx} = (2u) \cdot (\cos v) \cdot (3)
$$

$$
= 2\sin(3x) \cdot \cos(3x) \cdot 3 = 6\sin(3x)\cos(3x) = 3\sin(6x)
$$

(The last step uses the double angle formula $\sin 2\theta = 2\sin\theta\cos\theta$.)

---

### Practice Problems 5.3

1. Find the derivative of $y = (5x + 2)^4$.
2. Find the derivative of $y = \frac{1}{\sqrt{3x - 1}}$.
3. Find the derivative of $y = e^{2x-3}$.
4. Find the derivative of $y = \ln(x^2 + 4)$.
5. Find the derivative of $y = \cos^3(2x)$.

---

## 5.4 Product Rule and Quotient Rule

When two functions are multiplied or divided, their derivatives cannot be found by simply differentiating each part separately and then multiplying or dividing. Special rules are needed.

### 5.4.1 Product Rule

Let $y = u \cdot v$, where $u$ and $v$ are both functions of $x$. Then:

$$
\boxed{\frac{dy}{dx} = u\frac{dv}{dx} + v\frac{du}{dx}}
$$

Or briefly: $(uv)' = uv' + vu'$

Memory aid: "**first times derivative of second plus second times derivative of first**" — or, more mnemonically: "differentiate the first, leave the second, plus differentiate the second, leave the first."

**Detailed derivation of the Product Rule**:

Starting from the limit definition of the derivative:

$$
(uv)' = \lim_{\delta x \to 0} \frac{u(x+\delta x)v(x+\delta x) - u(x)v(x)}{\delta x}
$$

Cleverly add and subtract $u(x+\delta x)v(x)$ in the numerator:

$$
= \lim_{\delta x \to 0} \frac{u(x+\delta x)v(x+\delta x) - u(x+\delta x)v(x) + u(x+\delta x)v(x) - u(x)v(x)}{\delta x}
$$

$$
= \lim_{\delta x \to 0} \left[ u(x+\delta x) \cdot \frac{v(x+\delta x) - v(x)}{\delta x} + v(x) \cdot \frac{u(x+\delta x) - u(x)}{\delta x} \right]
$$

As $\delta x \to 0$, $u(x+\delta x) \to u(x)$, so:

$$
(uv)' = u(x) \cdot v'(x) + v(x) \cdot u'(x) = uv' + vu'
$$

### 5.4.2 Quotient Rule

Let $y = \frac{u}{v}$, where $u$ and $v$ are both functions of $x$, and $v \neq 0$. Then:

$$
\boxed{\frac{dy}{dx} = \frac{v\frac{du}{dx} - u\frac{dv}{dx}}{v^2}}
$$

Or briefly: $\left(\frac{u}{v}\right)' = \frac{vu' - uv'}{v^2}$

Memory aid: "**bottom times derivative of top minus top times derivative of bottom, all over bottom squared**" — remember that the derivative of the top comes first, and subtract.

**Derivation of the Quotient Rule** (derived from the Product Rule):

Write $\frac{u}{v}$ as $u \cdot v^{-1}$, then use the Product Rule and Chain Rule:

$$
\frac{d}{dx}\left(\frac{u}{v}\right) = \frac{d}{dx}(u \cdot v^{-1}) = u \cdot \frac{d}{dx}(v^{-1}) + v^{-1} \cdot \frac{du}{dx}
$$

$$
= u \cdot (-1)v^{-2} \cdot \frac{dv}{dx} + \frac{1}{v} \cdot \frac{du}{dx}
= -\frac{u}{v^2}\frac{dv}{dx} + \frac{1}{v}\frac{du}{dx}
$$

Putting over a common denominator:

$$
= \frac{v\frac{du}{dx} - u\frac{dv}{dx}}{v^2}
$$

---

### Worked Example 5.4A (Product Rule Basics)

> Find the derivatives of the following functions:
> (a) $y = (x^2 + 1)(x^3 - 2x)$
> (b) $y = x\sin x$
> (c) $y = e^x \cos x$
> (d) $y = x^2\ln x$

**Solution**:

(a) Let $u = x^2 + 1$, $v = x^3 - 2x$.
Then $u' = 2x$, $v' = 3x^2 - 2$.

$$
y' = uv' + vu' = (x^2 + 1)(3x^2 - 2) + (x^3 - 2x)(2x)
$$

Expanding:

$$
= 3x^4 - 2x^2 + 3x^2 - 2 + 2x^4 - 4x^2 = 5x^4 - 3x^2 - 2
$$

(Can also verify by expanding the original expression first and then differentiating.)

(b) Let $u = x$, $v = \sin x$, then $u' = 1$, $v' = \cos x$.

$$
y' = x\cos x + \sin x \cdot 1 = x\cos x + \sin x
$$

(c) Let $u = e^x$, $v = \cos x$, then $u' = e^x$, $v' = -\sin x$.

$$
y' = e^x \cdot (-\sin x) + \cos x \cdot e^x = e^x(\cos x - \sin x)
$$

(d) Let $u = x^2$, $v = \ln x$, then $u' = 2x$, $v' = \frac{1}{x}$.

$$
y' = x^2 \cdot \frac{1}{x} + \ln x \cdot 2x = x + 2x\ln x
$$

---

### Worked Example 5.4B (Quotient Rule Basics)

> Find the derivatives of the following functions:
> (a) $y = \frac{x}{x+1}$
> (b) $y = \frac{x^2}{\sin x}$
> (c) $y = \frac{e^x}{x^2 + 1}$
> (d) $y = \frac{\ln x}{x}$

**Solution**:

(a) Let $u = x$, $v = x+1$, then $u' = 1$, $v' = 1$.

$$
y' = \frac{vu' - uv'}{v^2} = \frac{(x+1)(1) - x(1)}{(x+1)^2} = \frac{x+1-x}{(x+1)^2} = \frac{1}{(x+1)^2}
$$

(b) Let $u = x^2$, $v = \sin x$, then $u' = 2x$, $v' = \cos x$.

$$
y' = \frac{(\sin x)(2x) - (x^2)(\cos x)}{\sin^2 x} = \frac{2x\sin x - x^2\cos x}{\sin^2 x}
$$

(c) Let $u = e^x$, $v = x^2 + 1$, then $u' = e^x$, $v' = 2x$.

$$
y' = \frac{(x^2+1)e^x - e^x(2x)}{(x^2+1)^2} = \frac{e^x(x^2 + 1 - 2x)}{(x^2+1)^2} = \frac{e^x(x-1)^2}{(x^2+1)^2}
$$

(d) Let $u = \ln x$, $v = x$, then $u' = \frac{1}{x}$, $v' = 1$.

$$
y' = \frac{x \cdot \frac{1}{x} - \ln x \cdot 1}{x^2} = \frac{1 - \ln x}{x^2}
$$

---

### Worked Example 5.4C (Integrated Product and Quotient Rule)

> (a) Given $y = (x^2 + 1)\ln x$, find $\frac{dy}{dx}$.
> (b) Given $y = \frac{\sin x}{e^x}$, find $\frac{dy}{dx}$.
> (c) Given $y = \tan x$, use $\tan x = \frac{\sin x}{\cos x}$ and the quotient rule to verify $\frac{d}{dx}(\tan x) = \sec^2 x$.
> (d) Find the derivative of $y = \frac{2x-1}{x^2+3}$.

**Solution**:

(a) Product Rule. Let $u = x^2 + 1$, $v = \ln x$, then $u' = 2x$, $v' = \frac{1}{x}$.

$$
\frac{dy}{dx} = (x^2+1)\cdot\frac{1}{x} + \ln x \cdot 2x = \frac{x^2+1}{x} + 2x\ln x = x + \frac{1}{x} + 2x\ln x
$$

(b) Quotient Rule. Let $u = \sin x$, $v = e^x$, then $u' = \cos x$, $v' = e^x$.

$$
\frac{dy}{dx} = \frac{e^x\cos x - \sin x \cdot e^x}{(e^x)^2} = \frac{e^x(\cos x - \sin x)}{e^{2x}} = \frac{\cos x - \sin x}{e^x}
$$

(c) Let $u = \sin x$, $v = \cos x$, then $u' = \cos x$, $v' = -\sin x$.

$$
\frac{d}{dx}\left(\frac{\sin x}{\cos x}\right) = \frac{\cos x \cdot \cos x - \sin x \cdot (-\sin x)}{\cos^2 x}
= \frac{\cos^2 x + \sin^2 x}{\cos^2 x}
$$

By the trigonometric identity $\sin^2 x + \cos^2 x = 1$:

$$
\frac{d}{dx}(\tan x) = \frac{1}{\cos^2 x} = \sec^2 x
$$

Verification complete.

(d) Let $u = 2x-1$, $v = x^2+3$, then $u' = 2$, $v' = 2x$.

$$
y' = \frac{(x^2+3)(2) - (2x-1)(2x)}{(x^2+3)^2}
= \frac{2x^2+6 - 4x^2 + 2x}{(x^2+3)^2}
= \frac{-2x^2 + 2x + 6}{(x^2+3)^2}
= \frac{-2(x^2 - x - 3)}{(x^2+3)^2}
$$

---

### Practice Problems 5.4

1. Find the derivative of $y = x^2 e^x$.
2. Find the derivative of $y = \frac{3x}{x-2}$.
3. Find the derivative of $y = x\cos x$.
4. Find the derivative of $y = \frac{x+1}{x^2+1}$.
5. Find the derivative of $y = e^x \sin x$.

---

## 5.5 Tangents and Normals

### 5.5.1 Basic Knowledge

Given a smooth curve $y = f(x)$ and a point $P(a, f(a))$ on it:

- **Tangent**: The line that passes through $P$ with slope $f'(a)$. The tangent is the **best linear approximation** to the curve at that point.
- **Normal**: The line that passes through $P$ and is perpendicular to the tangent.

### 5.5.2 Standard Three-Step Method (When the Point of Tangency is Known)

When the problem says "the tangent at point $P$", $P$ is the point of tangency. The solution steps are:

1. **Find the coordinates of the point of tangency**: Determine $a$, compute $f(a)$, get $(a, f(a))$.
2. **Find the slope of the tangent**: $m = f'(a)$.
3. **Write the tangent equation**: Use point-slope form $y - y_0 = m(x - x_0)$:

$$
y - f(a) = f'(a)(x - a)
$$

The slope of the **normal** $m_{\perp}$ satisfies $m \cdot m_{\perp} = -1$ (when $m \neq 0$), i.e., $m_{\perp} = -\frac{1}{f'(a)}$. The equation of the normal is:

$$
y - f(a) = -\frac{1}{f'(a)}(x - a)
$$

Special cases:
- If $f'(a) = 0$ (tangent is horizontal), the normal is the vertical line $x = a$.
- If $f'(a)$ does not exist (e.g., a cusp), the tangent is vertical and the normal is horizontal.

### 5.5.3 Why is the Tangent Slope Equal to the Derivative?

Geometrically, the line connecting two points $(a, f(a))$ and $(a+\delta x, f(a+\delta x))$ on the curve has slope $\frac{f(a+\delta x) - f(a)}{\delta x}$. As $\delta x$ approaches $0$, this line approaches the tangent line, and its slope approaches the derivative $f'(a)$.

Algebraically, the tangent equation $y = f(a) + f'(a)(x-a)$ has the same function value and the same first derivative as the curve at $x=a$, making it the "best linear approximation."

### 5.5.4 Important Pitfall: When the Point of Tangency is Unknown

If the problem says "the tangent passing through point $P$" (rather than "at point $P$"), then $P$ **may not be the point of tangency**. In this case:

1. Let the point of tangency be $(a, f(a))$, where $a$ is unknown.
2. Write the tangent equation: $y - f(a) = f'(a)(x - a)$.
3. Substitute the coordinates of $P$ into the equation to obtain an equation in $a$, then solve for all possible $a$.
4. Each $a$ corresponds to one tangent.

---

### Worked Example 5.5A (Tangent and Normal When the Point of Tangency is Known)

> What are the equations of the tangent and normal to the curve $y = x^2 - 3x + 2$ at the point $(2, 0)$?

**Solution**:

Point of tangency: $(2, 0)$, i.e., $a = 2$, $f(2) = 0$.

Differentiate: $f'(x) = 2x - 3$, $f'(2) = 2(2) - 3 = 1$.

Tangent equation:

$$
y - 0 = 1(x - 2) \quad \Rightarrow \quad y = x - 2
$$

Slope of normal $m_{\perp} = -\frac{1}{1} = -1$, normal equation:

$$
y - 0 = -1(x - 2) \quad \Rightarrow \quad y = -x + 2
$$

---

### Worked Example 5.5B (Tangent and Normal with Trigonometric Functions)

> Find the equations of the tangent and normal to the curve $y = \sin x$ at the point $\left(\frac{\pi}{6}, \frac{1}{2}\right)$.

**Solution**:

Point of tangency: $\left(\frac{\pi}{6}, \frac{1}{2}\right)$.

Differentiate: $f'(x) = \cos x$, $f'\left(\frac{\pi}{6}\right) = \cos\frac{\pi}{6} = \frac{\sqrt{3}}{2}$.

Tangent equation:

$$
y - \frac{1}{2} = \frac{\sqrt{3}}{2}\left(x - \frac{\pi}{6}\right)
$$

Simplifying:

$$
y = \frac{\sqrt{3}}{2}x - \frac{\sqrt{3}\pi}{12} + \frac{1}{2}
$$

Slope of normal $m_{\perp} = -\frac{1}{\sqrt{3}/2} = -\frac{2}{\sqrt{3}}$, normal equation:

$$
y - \frac{1}{2} = -\frac{2}{\sqrt{3}}\left(x - \frac{\pi}{6}\right)
$$

---

### Worked Example 5.5C ("Passing Through" a Point — Point of Tangency Unknown)

> Find the equations of the tangents to the curve $y = x^2$ that pass through the point $P(2, 3)$.

**Solution**:

Note that $P(2, 3)$ is not on the curve $y = x^2$ (since $2^2 = 4 \neq 3$), so $P$ is not the point of tangency. Let the point of tangency be $(a, a^2)$.

$f(x) = x^2$, $f'(x) = 2x$, so $f'(a) = 2a$.

Tangent equation:

$$
y - a^2 = 2a(x - a)
$$

Substitute $P(2, 3)$:

$$
3 - a^2 = 2a(2 - a)
$$

Expanding:

$$
3 - a^2 = 4a - 2a^2
$$

Rearranging:

$$
a^2 - 4a + 3 = 0
$$

Factorising:

$$
(a - 1)(a - 3) = 0
$$

So $a = 1$ or $a = 3$.

- When $a = 1$, the point of tangency is $(1, 1)$, slope $m = 2$, tangent equation: $y - 1 = 2(x - 1)$, i.e., $y = 2x - 1$.
- When $a = 3$, the point of tangency is $(3, 9)$, slope $m = 6$, tangent equation: $y - 9 = 6(x - 3)$, i.e., $y = 6x - 9$.

Point $P(2, 3)$ has two distinct tangents to the curve.

---

### Worked Example 5.5D (Tangent and Coordinate Axes Intersections)

> Find the intersections of the tangent to the curve $y = \ln x$ at the point $(1, 0)$ with the $x$-axis and $y$-axis.

**Solution**:

$f(x) = \ln x$, $f'(x) = \frac{1}{x}$, $f'(1) = 1$.

Tangent equation: $y - 0 = 1(x - 1)$, i.e., $y = x - 1$.

Intersection with $x$-axis: set $y = 0$, $0 = x - 1$, $x = 1$, i.e., $(1, 0)$ (which is the point of tangency itself).

Intersection with $y$-axis: set $x = 0$, $y = 0 - 1 = -1$, i.e., $(0, -1)$.

---

### Practice Problems 5.5

1. Find the equations of the tangent and normal to the curve $y = x^3$ at the point $(2, 8)$.
2. Find the equation of the tangent to the curve $y = e^x$ at the point $(0, 1)$.
3. Find the equations of the tangent and normal to the curve $y = \sqrt{x}$ at the point $(4, 2)$.
4. Find the equations of the tangents to the curve $y = x^2 - 2x$ that pass through the point $(1, -4)$.

---

## 5.6 Stationary Points (Maxima and Minima)

### 5.6.1 What is a Stationary Point?

A **stationary point** is a point on the graph where the tangent is horizontal (slope zero). At a stationary point, the function value may be a local maximum, a local minimum, or neither (the latter case is not examined in IGCSE).

**Steps for finding stationary points**:
1. Find $f'(x)$.
2. Solve $f'(x) = 0$.
3. Each solution $x = a$ corresponds to a stationary point $(a, f(a))$.

### 5.6.2 Distinguishing Between Maxima and Minima

There are two methods to distinguish between maxima and minima.

**Method 1: First Derivative Test (Sign Change Method)**

Observe the sign of $f'(x)$ on either side of the stationary point $x = a$:

| $x$ slightly less than $a$ (left) | $x = a$ | $x$ slightly greater than $a$ (right) | Conclusion |
|:---:|:---:|:---:|:---:|
| $f' > 0$ (increasing) | $f' = 0$ | $f' < 0$ (decreasing) | **Local maximum** |
| $f' < 0$ (decreasing) | $f' = 0$ | $f' > 0$ (increasing) | **Local minimum** |
| $f' > 0$ (increasing) | $f' = 0$ | $f' > 0$ (increasing) | Not an extremum (not examined) |
| $f' < 0$ (decreasing) | $f' = 0$ | $f' < 0$ (decreasing) | Not an extremum (not examined) |

Why does the sign change determine the type of extremum? Imagine climbing a mountain:
- If you first go uphill ($f'>0$), reach the summit ($f'=0$), then go downhill ($f'<0$), the summit is a local maximum.
- If you first go downhill ($f'<0$), reach the valley floor ($f'=0$), then go uphill ($f'>0$), the valley floor is a local minimum.

**Method 2: Second Derivative Test**

The second derivative $f''(x)$ is the derivative of the first derivative. It tells us the rate of change of $f'(x)$.

- If $f'(a) = 0$ and $f''(a) > 0$ → **Local minimum** (the curve is "concave up" at that point, like the bottom of a bowl).
- If $f'(a) = 0$ and $f''(a) < 0$ → **Local maximum** (the curve is "concave down" at that point, like an upside-down bowl).
- If $f''(a) = 0$, the test is inconclusive, and the first derivative test must be used.

**Why can the second derivative determine the type?**
- $f''(a) > 0$ means $f'(x)$ is increasing at $x=a$. Since $f'(a)=0$, $f'$ changes from negative to positive → minimum.
- $f''(a) < 0$ means $f'(x)$ is decreasing at $x=a$. Since $f'(a)=0$, $f'$ changes from positive to negative → maximum.

### 5.6.3 Finding the Second Derivative

The second derivative is the derivative of the first derivative. In notation:

$$
f''(x) = \frac{d}{dx}(f'(x)) \quad \text{or} \quad \frac{d^2y}{dx^2} = \frac{d}{dx}\left(\frac{dy}{dx}\right)
$$

**Example**: $f(x) = x^3 - 3x^2 + 2$
- First derivative: $f'(x) = 3x^2 - 6x$
- Second derivative: $f''(x) = 6x - 6$

---

### Worked Example 5.6A (Stationary Points of a Polynomial Function)

> Find the stationary points of $f(x) = 2x^3 - 9x^2 + 12x - 3$ and determine whether they are maxima or minima.

**Solution**:

Step 1: Find $f'(x)$ and set it to zero.

$$
f'(x) = 6x^2 - 18x + 12 = 6(x^2 - 3x + 2) = 6(x-1)(x-2)
$$

Set $f'(x) = 0$: $x = 1$ or $x = 2$.

$$
f(1) = 2 - 9 + 12 - 3 = 2, \quad \text{stationary point } (1, 2)
$$
$$
f(2) = 16 - 36 + 24 - 3 = 1, \quad \text{stationary point } (2, 1)
$$

Step 2: Use the second derivative test.

$$
f''(x) = 12x - 18
$$

- $f''(1) = 12(1) - 18 = -6 < 0$ → $(1, 2)$ is a **local maximum**.
- $f''(2) = 12(2) - 18 = 6 > 0$ → $(2, 1)$ is a **local minimum**.

First derivative test verification: to the left of $x=1$, take $x=0$, $f'(0) = 12 > 0$; to the right of $x=1$, take $x=1.5$, $f'(1.5) = 6(0.5)(-0.5) = -1.5 < 0$. Sign changes from positive to negative, confirming a maximum.

---

### Worked Example 5.6B (Stationary Points with Trigonometric Functions)

> Find the stationary points of $f(x) = \sin x + \cos x$ on the interval $[0, 2\pi]$ and determine their types.

**Solution**:

$$
f'(x) = \cos x - \sin x
$$

Set $f'(x) = 0$:

$$
\cos x - \sin x = 0 \quad \Rightarrow \quad \cos x = \sin x \quad \Rightarrow \quad \tan x = 1
$$

On $[0, 2\pi]$, the solutions to $\tan x = 1$ are $x = \frac{\pi}{4}$ and $x = \frac{5\pi}{4}$.

$$
f\left(\frac{\pi}{4}\right) = \frac{\sqrt{2}}{2} + \frac{\sqrt{2}}{2} = \sqrt{2}, \quad
f\left(\frac{5\pi}{4}\right) = -\frac{\sqrt{2}}{2} - \frac{\sqrt{2}}{2} = -\sqrt{2}
$$

Find the second derivative: $f''(x) = -\sin x - \cos x$.

- $f''\left(\frac{\pi}{4}\right) = -\frac{\sqrt{2}}{2} - \frac{\sqrt{2}}{2} = -\sqrt{2} < 0$ → $\left(\frac{\pi}{4}, \sqrt{2}\right)$ is a **local maximum**.
- $f''\left(\frac{5\pi}{4}\right) = \frac{\sqrt{2}}{2} + \frac{\sqrt{2}}{2} = \sqrt{2} > 0$ → $\left(\frac{5\pi}{4}, -\sqrt{2}\right)$ is a **local minimum**.

---

### Worked Example 5.6C (Stationary Points with Exponential Functions)

> Find the stationary point of $f(x) = xe^{-x}$ and determine its type. Find the maximum value of the function.

**Solution**:

Use the Product Rule: let $u = x$, $v = e^{-x}$, then $u' = 1$, $v' = -e^{-x}$.

$$
f'(x) = x \cdot (-e^{-x}) + e^{-x} \cdot 1 = e^{-x}(1 - x)
$$

Set $f'(x) = 0$. Since $e^{-x} > 0$ for all $x$, we have $1 - x = 0$, i.e., $x = 1$.

$$
f(1) = 1 \cdot e^{-1} = \frac{1}{e}
$$

The stationary point is $\left(1, \frac{1}{e}\right)$.

Using the first derivative test: to the left of $x=1$, take $x=0$, $f'(0) = e^0(1-0) = 1 > 0$; to the right of $x=1$, take $x=2$, $f'(2) = e^{-2}(1-2) = -e^{-2} < 0$. The sign changes from positive to negative, so $\left(1, \frac{1}{e}\right)$ is a **local maximum**.

Since $xe^{-x} \to 0$ as $x \to \infty$ and $xe^{-x} \to -\infty$ as $x \to -\infty$, this local maximum is also the global maximum, with value $\frac{1}{e}$.

---

### Worked Example 5.6D (Finding Parameters from Stationary Points)

> Given that $f(x) = x^3 + ax^2 + b$ has a stationary point at $x = 2$, and the function value at this stationary point is $5$, find the constants $a$ and $b$.

**Solution**:

$f'(x) = 3x^2 + 2ax$

There is a stationary point at $x=2$, so $f'(2) = 0$:

$$
3(2)^2 + 2a(2) = 0 \quad \Rightarrow \quad 12 + 4a = 0 \quad \Rightarrow \quad a = -3
$$

The function value at the stationary point is $f(2) = 5$:

$$
f(2) = 2^3 + (-3)(2)^2 + b = 8 - 12 + b = b - 4 = 5 \quad \Rightarrow \quad b = 9
$$

Thus $a = -3$, $b = 9$. $f(x) = x^3 - 3x^2 + 9$.

---

### Practice Problems 5.6

1. Find the stationary points of $f(x) = x^3 - 6x^2 + 9x + 1$ and determine their types.
2. Find the stationary points of $f(x) = x^2 e^x$ and determine their types.
3. Given that $f(x) = x^3 + ax + b$ has a stationary point at $x = 1$ with $f(1) = 4$, find $a$ and $b$.
4. Find the extreme values of $f(x) = 2x^3 - 3x^2 - 12x + 5$.

---

## 5.7 Connected Rates of Change and Small Increments Approximation

### 5.7.1 Connected Rates of Change

Connected rates of change problems deal with the **rates of change of multiple interrelated quantities**. The core idea is: if $y$ depends on $u$ through some relationship, and $u$ in turn depends on $x$, then we can link $\frac{dy}{dx}$ to $\frac{dy}{du}$ and $\frac{du}{dx}$ through the chain rule.

$$
\frac{dy}{dx} = \frac{dy}{du} \cdot \frac{du}{dx}
$$

More generally, when the problem involves time $t$, we often use:

$$
\frac{dy}{dt} = \frac{dy}{dx} \cdot \frac{dx}{dt}
$$

**Problem-solving steps**:
1. Identify all relevant variables, determine the known rate of change and the required rate of change.
2. Establish the functional relationship between the variables (geometric formula, physical relationship, etc.).
3. Differentiate both sides of the relationship with respect to time $t$ (implicit differentiation).
4. Substitute the known values and solve for the unknown rate of change.

### 5.7.2 Small Increments and Approximations

Another important application of the derivative is using the tangent line to approximate the change in a function near a given point.

Recall the definition of the derivative:

$$
f'(a) \approx \frac{f(a + \delta x) - f(a)}{\delta x} \quad \text{(when $\delta x$ is small)}
$$

Rearranging gives:

$$
\boxed{f(a + \delta x) \approx f(a) + f'(a) \cdot \delta x}
$$

This is the **linear approximation** formula. It tells us: for a small change $\delta x$, the change in the function value is approximately equal to the derivative multiplied by the change in the independent variable.

In Leibniz notation:

$$
\delta y \approx \frac{dy}{dx} \cdot \delta x
$$

where $\delta y = f(x + \delta x) - f(x)$ is the actual change in the function value, and $\frac{dy}{dx} \cdot \delta x$ is the change along the tangent line (the approximate value).

**Why does this work?** Geometrically, the tangent line is the best approximation to the curve near the point of tangency. When $\delta x$ is small, the point $(a+\delta x, f(a+\delta x))$ on the curve is very close to the point $(a+\delta x, f(a) + f'(a)\delta x)$ on the tangent line, so we can use the change on the tangent line to approximate the change on the curve.

---

### Worked Example 5.7A (Connected Rates of Change — Area of a Circle)

> The radius of a circle is increasing at a rate of $2$ cm/s. Find the rate at which the area is increasing when the radius is $5$ cm.

**Solution**:

Let the radius be $r$ and the area be $A$. We know $\frac{dr}{dt} = 2$, and we need to find $\frac{dA}{dt}$ when $r = 5$.

Area of a circle: $A = \pi r^2$

Differentiate with respect to time $t$ (using the chain rule):

$$
\frac{dA}{dt} = \frac{dA}{dr} \cdot \frac{dr}{dt} = 2\pi r \cdot \frac{dr}{dt}
$$

Substitute the known values: $r = 5$, $\frac{dr}{dt} = 2$.

$$
\frac{dA}{dt} = 2\pi \cdot 5 \cdot 2 = 20\pi \text{ cm}^2/\text{s}
$$

So when the radius is $5$ cm, the area is increasing at a rate of $20\pi$ cm²/s.

---

### Worked Example 5.7B (Connected Rates of Change — Kinematics)

> An inverted conical container has a top radius of $4$ m and a height of $8$ m. Water is being poured in at a rate of $2$ m³/min. Find the rate at which the water level is rising when the water depth is $3$ m.

**Solution**:

Let the water depth be $h$, the radius of the water surface be $r$, and the volume of water be $V$. We know $\frac{dV}{dt} = 2$, and we need to find $\frac{dh}{dt}$ when $h = 3$.

By similar triangles: $\frac{r}{h} = \frac{4}{8} = \frac{1}{2}$, so $r = \frac{h}{2}$.

Volume of a cone:

$$
V = \frac{1}{3}\pi r^2 h = \frac{1}{3}\pi \left(\frac{h}{2}\right)^2 h = \frac{1}{3}\pi \cdot \frac{h^2}{4} \cdot h = \frac{\pi}{12}h^3
$$

Differentiate with respect to time:

$$
\frac{dV}{dt} = \frac{dV}{dh} \cdot \frac{dh}{dt} = \frac{\pi}{12} \cdot 3h^2 \cdot \frac{dh}{dt} = \frac{\pi}{4}h^2 \cdot \frac{dh}{dt}
$$

Substitute $\frac{dV}{dt} = 2$ and $h = 3$:

$$
2 = \frac{\pi}{4} \cdot 3^2 \cdot \frac{dh}{dt} = \frac{9\pi}{4} \cdot \frac{dh}{dt}
$$

Solving:

$$
\frac{dh}{dt} = \frac{2 \cdot 4}{9\pi} = \frac{8}{9\pi} \text{ m/min}
$$

So when the water depth is $3$ m, the water level is rising at a rate of $\frac{8}{9\pi}$ m/min.

---

### Worked Example 5.7C (Small Increments Approximation)

> Use differential approximation to estimate the value of $\sqrt{4.02}$.

**Solution**:

Let $f(x) = \sqrt{x}$, choose $a = 4$ (a number whose square root is easy to compute), and $\delta x = 0.02$.

$$
f(x) = x^{1/2}, \quad f'(x) = \frac{1}{2}x^{-1/2} = \frac{1}{2\sqrt{x}}
$$

$$
f(4) = \sqrt{4} = 2, \quad f'(4) = \frac{1}{2\sqrt{4}} = \frac{1}{4}
$$

Linear approximation formula:

$$
f(4 + 0.02) \approx f(4) + f'(4) \cdot 0.02
$$

$$
\sqrt{4.02} \approx 2 + \frac{1}{4} \times 0.02 = 2 + 0.005 = 2.005
$$

Compared to the exact value $2.004993\ldots$, the approximation $2.005$ has a very small error (about $7 \times 10^{-6}$).

---

### Worked Example 5.7D (Small Increments Approximation — Finding Maximum Error from Known Error)

> The volume of a sphere is given by $V = \frac{4}{3}\pi r^3$. If the maximum error in measuring the radius is $0.1$ cm, find the maximum approximate error in calculating the volume when the measured radius is $5$ cm.

**Solution**:

We know $r = 5$ and $|\delta r| \leq 0.1$.

$$
\frac{dV}{dr} = 4\pi r^2
$$

$$
\delta V \approx \frac{dV}{dr} \cdot \delta r = 4\pi r^2 \cdot \delta r
$$

Maximum error (taking absolute values):

$$
|\delta V|_{\max} \approx 4\pi \cdot 5^2 \cdot 0.1 = 4\pi \cdot 25 \cdot 0.1 = 10\pi \text{ cm}^3
$$

So the maximum approximate error in the volume is about $10\pi \approx 31.4$ cm³.

---

### Practice Problems 5.7

1. The side length of a square is increasing at a rate of $3$ cm/s. Find the rate at which the area is increasing when the side length is $10$ cm.
2. Use differential approximation to estimate $\sqrt[3]{8.03}$. (Hint: let $f(x) = \sqrt[3]{x}$)
3. Gas is expanding in a spherical container. When the radius is $2$ m, the volume is increasing at a rate of $16\pi$ m³/s. Find the rate at which the radius is increasing at that moment.

---

## 5.8 Practical Maxima and Minima Problems

### 5.8.1 Problem-solving Approach

Practical maxima and minima problems apply calculus to real-world optimisation problems — for example, how to use the least material to make a container, how to maximise profit given a certain cost, how to determine the fastest route, etc.

**Standard problem-solving steps**:

1. **Understand the problem**: Identify the quantity to be maximised or minimised (the objective function).
2. **Introduce variables**: Introduce variables to represent all relevant quantities.
3. **Establish relationships**: Use the information given in the problem (geometric relations, physical constraints, etc.) to express the objective function in terms of **a single variable**.
4. **Differentiate and find stationary points**: Differentiate the objective function, set the derivative to zero, and solve for the stationary point.
5. **Determine the type**: Use the first or second derivative test to confirm whether it is a maximum or minimum.
6. **Check reasonableness**: Verify that the stationary point lies within the domain, and answer the original question.

> ⚠️ **Key point**: Practical problems usually have constraint conditions (e.g., fixed total length, fixed area). Use the constraint to eliminate extra variables and reduce the objective function to a single-variable function.

---

### Worked Example 5.8A (Maximising Area)

> A $100$ m length of fencing is used to enclose a rectangular garden with one side against a wall (the wall is long enough). Find the maximum area of the garden and the dimensions at which it occurs.

**Solution**:

Let the two sides perpendicular to the wall have length $x$ m, and the side parallel to the wall have length $y$ m.

Total fencing length is $100$ m, constraint: $2x + y = 100$, i.e., $y = 100 - 2x$.

Garden area $A = x \cdot y = x(100 - 2x) = 100x - 2x^2$.

Note the domain: $x > 0$ and $y > 0$, i.e., $100 - 2x > 0$, $x < 50$, so $0 < x < 50$.

Differentiate:

$$
A'(x) = 100 - 4x
$$

Set $A'(x) = 0$: $100 - 4x = 0$, giving $x = 25$.

Second derivative: $A''(x) = -4 < 0$, confirming $x = 25$ is a **maximum**.

At this point, $y = 100 - 2(25) = 50$.

Maximum area: $A = 25 \times 50 = 1250$ m².

**Answer**: When the sides perpendicular to the wall are $25$ m and the side parallel to the wall is $50$ m, the maximum area is $1250$ m².

---

### Worked Example 5.8B (Maximising Volume — Open Box)

> From a rectangular sheet of cardboard measuring $30$ cm $\times$ $20$ cm, four squares of side length $x$ cm are cut from the corners, and the sides are folded up to make an open box. Find the value of $x$ that maximises the volume of the box, and find the maximum volume.

**Solution**:

After cutting squares of side $x$, the base dimensions of the box are $(30 - 2x) \times (20 - 2x)$, and the height is $x$.

Volume of the box:

$$
V(x) = x(30 - 2x)(20 - 2x) = x(600 - 60x - 40x + 4x^2) = x(600 - 100x + 4x^2)
$$

$$
V(x) = 4x^3 - 100x^2 + 600x
$$

Domain: $x > 0$, $30 - 2x > 0 \Rightarrow x < 15$, $20 - 2x > 0 \Rightarrow x < 10$, so $0 < x < 10$.

Differentiate:

$$
V'(x) = 12x^2 - 200x + 600
$$

Set $V'(x) = 0$:

$$
12x^2 - 200x + 600 = 0
$$

Divide both sides by $4$: $3x^2 - 50x + 150 = 0$

Using the quadratic formula:

$$
x = \frac{50 \pm \sqrt{2500 - 1800}}{6} = \frac{50 \pm \sqrt{700}}{6} = \frac{50 \pm 10\sqrt{7}}{6}
$$

The two solutions: $x_1 = \frac{50 + 10\sqrt{7}}{6} \approx \frac{50 + 26.46}{6} \approx 12.74$ (outside the domain $x < 10$, discard)

$$
x_2 = \frac{50 - 10\sqrt{7}}{6} \approx \frac{50 - 26.46}{6} \approx 3.92
$$

So $x = \frac{50 - 10\sqrt{7}}{6} \approx 3.92$ cm.

Verify with the second derivative: $V''(x) = 24x - 200$

$$
V''(3.92) = 24(3.92) - 200 \approx 94.08 - 200 = -105.92 < 0
$$

Confirmed as a maximum.

Maximum volume:

$$
V = 3.92 \times (30 - 7.84) \times (20 - 7.84) = 3.92 \times 22.16 \times 12.16 \approx 1056.3 \text{ cm}^3
$$

**Answer**: When the side length of the cut squares is approximately $3.92$ cm, the box volume is maximised at approximately $1056$ cm³.

---

### Worked Example 5.8C (Minimising Cost)

> A company needs to manufacture an open cylindrical bucket with a fixed volume of $V = 1000\pi$ cm³. The material for the base costs $2$ yuan/cm², and the material for the sides costs $1$ yuan/cm². Find the base radius $r$ and height $h$ that minimise the total cost, and find the minimum cost.

**Solution**:

Let the base radius be $r$ cm and the height be $h$ cm.

Volume constraint: $V = \pi r^2 h = 1000\pi$, so $h = \frac{1000}{r^2}$.

Cost: base area $\pi r^2$, price $2$ yuan/cm²; lateral surface area $2\pi r h$, price $1$ yuan/cm².

$$
C = 2 \cdot \pi r^2 + 1 \cdot 2\pi r h = 2\pi r^2 + 2\pi r \cdot \frac{1000}{r^2} = 2\pi r^2 + \frac{2000\pi}{r}
$$

Domain: $r > 0$.

Differentiate:

$$
C'(r) = 4\pi r - \frac{2000\pi}{r^2}
$$

Set $C'(r) = 0$:

$$
4\pi r - \frac{2000\pi}{r^2} = 0 \quad \Rightarrow \quad 4\pi r = \frac{2000\pi}{r^2}
$$

Divide both sides by $\pi$ ($\pi > 0$):

$$
4r = \frac{2000}{r^2} \quad \Rightarrow \quad 4r^3 = 2000 \quad \Rightarrow \quad r^3 = 500
$$

So: $r = \sqrt[3]{500} = \sqrt[3]{5 \times 100} = 5\sqrt[3]{4}$ cm.

At this point, $h = \frac{1000}{r^2} = \frac{1000}{500^{2/3}} = 2 \cdot 500^{1/3} = 2r$.

Thus $h = 2r$, i.e., the height equals the diameter when the cost is minimised.

Verify with the second derivative:

$$
C''(r) = 4\pi + \frac{4000\pi}{r^3}
$$

Substituting $r^3 = 500$: $C''(r) = 4\pi + \frac{4000\pi}{500} = 4\pi + 8\pi = 12\pi > 0$, confirmed as a minimum.

Minimum cost:

$$
C_{\min} = 6\pi \cdot 500^{2/3} \text{ yuan}
$$

Approximate calculation: $500^{2/3} = (500^{1/3})^2 \approx (7.937)^2 \approx 63$, so $C_{\min} \approx 6\pi \times 63 \approx 1188$ yuan.

**Answer**: When the base radius $r = \sqrt[3]{500}$ cm (about $7.94$ cm) and the height $h = 2r$ (about $15.88$ cm), the minimum cost is approximately $1188$ yuan.

---

### Worked Example 5.8D (Maximising Profit)

> A factory produces a product. The cost of producing $x$ units per day is $C(x) = 200 + 10x + 0.01x^2$ yuan, and the selling price is $30$ yuan per unit. Find the number of units that should be produced per day to maximise profit, and find the maximum profit.

**Solution**:

Revenue: $R(x) = 30x$

Profit: $P(x) = R(x) - C(x) = 30x - (200 + 10x + 0.01x^2) = -0.01x^2 + 20x - 200$

Domain: $x \ge 0$ and integer (in practice, positive integers, but we can use the continuous function to approximate the maximum and then round).

Differentiate:

$$
P'(x) = -0.02x + 20
$$

Set $P'(x) = 0$: $-0.02x + 20 = 0$, giving $x = 1000$.

Second derivative: $P''(x) = -0.02 < 0$, confirmed as a maximum.

Maximum profit:

$$
P(1000) = -0.01(1000)^2 + 20(1000) - 200 = -10000 + 20000 - 200 = 9800 \text{ yuan}
$$

**Answer**: Maximum profit occurs when $1000$ units are produced per day, with a maximum profit of $9800$ yuan.

---

### Practice Problems 5.8

1. A $120$ m length of fencing is used to enclose a rectangular garden (not against a wall). Find the maximum area and the dimensions at which it occurs.
2. Find the shortest distance from the curve $y = x^2 - 4x + 5$ to the origin $(0,0)$.
   (Hint: distance squared $d^2 = x^2 + y^2$, substitute $y$ and minimise)
3. An open cylindrical can has a fixed volume $V$ (constant). Find the ratio of the base radius $r$ to the height $h$ that minimises the surface area.

---

## Chapter Summary (Quick Reference Table)

| Topic | Formula/Method | Section |
|--------|-----------|:----:|
| Limit definition of derivative | $\displaystyle f'(x) = \lim_{\delta x \to 0} \frac{f(x+\delta x) - f(x)}{\delta x}$ | 5.1 |
| Power Rule | $\frac{d}{dx}(x^n) = nx^{n-1}$ ($n$ any rational number) | 5.2 |
| Trigonometric derivatives | $\frac{d}{dx}(\sin x) = \cos x$, $\frac{d}{dx}(\cos x) = -\sin x$, $\frac{d}{dx}(\tan x) = \sec^2 x$ | 5.2 |
| Exponential & logarithmic derivatives | $\frac{d}{dx}(e^x) = e^x$, $\frac{d}{dx}(\ln x) = \frac{1}{x}$, $\frac{d}{dx}(a^x) = a^x\ln a$ | 5.2 |
| Chain Rule | $\frac{dy}{dx} = \frac{dy}{du} \cdot \frac{du}{dx}$ | 5.3 |
| Product Rule | $(uv)' = uv' + vu'$ | 5.4 |
| Quotient Rule | $\left(\frac{u}{v}\right)' = \frac{vu' - uv'}{v^2}$ | 5.4 |
| Tangent equation | $y - f(a) = f'(a)(x - a)$ | 5.5 |
| Normal equation | $y - f(a) = -\frac{1}{f'(a)}(x - a)$ ($f'(a) \neq 0$) | 5.5 |
| Stationary points | Solve $f'(x) = 0$ | 5.6 |
| Second derivative test | $f''(a) > 0$ is minimum, $f''(a) < 0$ is maximum | 5.6 |
| Connected rates of change | $\frac{dy}{dt} = \frac{dy}{dx} \cdot \frac{dx}{dt}$ | 5.7 |
| Small increments approximation | $f(a + \delta x) \approx f(a) + f'(a)\delta x$, $\delta y \approx \frac{dy}{dx}\delta x$ | 5.7 |
| Practical maxima/minima | Build single-variable function $\to$ differentiate and find stationary point $\to$ determine type $\to$ answer original question | 5.8 |

---

## Answers to Practice Problems

### 5.1 Concept of Derivative and Notation

1. $f'(1) = 4$
   - $f(1+\delta x) = (1+\delta x)^2 + 2(1+\delta x) = 1 + 2\delta x + (\delta x)^2 + 2 + 2\delta x = 3 + 4\delta x + (\delta x)^2$
   - $f(1) = 1^2 + 2(1) = 3$
   - $\frac{f(1+\delta x) - f(1)}{\delta x} = \frac{4\delta x + (\delta x)^2}{\delta x} = 4 + \delta x \to 4$

2. $s'(3) = 15$ m/s
   - $s'(t) = 4t + 3$, $s'(3) = 4(3) + 3 = 15$

3. $8$
   - $\lim_{x \to 4} \frac{x^2 - 16}{x - 4} = \lim_{x \to 4} \frac{(x-4)(x+4)}{x-4} = \lim_{x \to 4} (x+4) = 8$

### 5.2 Basic Differentiation Formulas

1. $f'(x) = 12x^2 - 4x + 5$

2. $g'(x) = -\frac{6}{x^3} + \frac{1}{4x\sqrt{x}} + 2x^{-2/3}$
   - Specifically: $\frac{3}{x^2} = 3x^{-2} \to -6x^{-3}$; $-\frac{1}{2}x^{-1/2} \to \frac{1}{4}x^{-3/2}$; $6x^{1/3} \to 2x^{-2/3}$

3. $h'(x) = 5\cos x + 3\sin x + 2\sec^2 x$

4. $p'(x) = 2e^x + 4^x\ln 4 - \frac{1}{3x}$

### 5.3 Chain Rule

1. $y' = 20(5x+2)^3$
2. $y = (3x-1)^{-1/2}$, $y' = -\frac{3}{2}(3x-1)^{-3/2} = -\frac{3}{2\sqrt{(3x-1)^3}}$
3. $y' = 2e^{2x-3}$
4. $y' = \frac{2x}{x^2+4}$
5. $y' = 3\cos^2(2x) \cdot (-\sin(2x)) \cdot 2 = -6\cos^2(2x)\sin(2x) = -3\cos(2x)\sin(4x)$

### 5.4 Product Rule and Quotient Rule

1. $y' = 2xe^x + x^2e^x = xe^x(2 + x)$
2. $y' = \frac{3(x-2) - 3x(1)}{(x-2)^2} = \frac{3x-6-3x}{(x-2)^2} = -\frac{6}{(x-2)^2}$
3. $y' = \cos x - x\sin x$
4. $y' = \frac{(1)(x^2+1) - (x+1)(2x)}{(x^2+1)^2} = \frac{x^2+1 - 2x^2 - 2x}{(x^2+1)^2} = \frac{-x^2 - 2x + 1}{(x^2+1)^2}$
5. $y' = e^x\sin x + e^x\cos x = e^x(\sin x + \cos x)$

### 5.5 Tangents and Normals

1. $f(x) = x^3$, $f'(x) = 3x^2$, $f'(2) = 12$
   - Tangent: $y - 8 = 12(x - 2)$, i.e., $y = 12x - 16$
   - Normal: $y - 8 = -\frac{1}{12}(x - 2)$, i.e., $y = -\frac{1}{12}x + \frac{49}{6}$

2. $f(x) = e^x$, $f'(x) = e^x$, $f'(0) = 1$
   - Tangent: $y - 1 = 1(x - 0)$, i.e., $y = x + 1$

3. $f(x) = \sqrt{x}$, $f'(x) = \frac{1}{2\sqrt{x}}$, $f'(4) = \frac{1}{4}$
   - Tangent: $y - 2 = \frac{1}{4}(x - 4)$, i.e., $y = \frac{1}{4}x + 1$
   - Normal: $y - 2 = -4(x - 4)$, i.e., $y = -4x + 18$

4. Let the point of tangency be $(a, a^2 - 2a)$, $f'(a) = 2a - 2$.
   Tangent equation: $y - (a^2 - 2a) = (2a - 2)(x - a)$
   Substitute $(1, -4)$: $-4 - (a^2 - 2a) = (2a - 2)(1 - a)$
   Simplify: $-4 - a^2 + 2a = (2a-2)(1-a) = 2a-2 - 2a^2 + 2a = -2a^2 + 4a - 2$
   Rearranging: $-4 - a^2 + 2a = -2a^2 + 4a - 2$, bring terms: $a^2 - 2a - 2 = 0$
   So $a = 1 \pm \sqrt{3}$
   - $a = 1 + \sqrt{3}$: slope $m = 2\sqrt{3}$, tangent $y = 2\sqrt{3}x - 2\sqrt{3} - 4$
   - $a = 1 - \sqrt{3}$: slope $m = -2\sqrt{3}$, tangent $y = -2\sqrt{3}x + 2\sqrt{3} - 4$

### 5.6 Stationary Points

1. $f'(x) = 3x^2 - 12x + 9 = 3(x-1)(x-3)$
   $x = 1$: $f(1) = 5$, $f''(1) = 6-12 = -6 < 0$ → maximum
   $x = 3$: $f(3) = 1$, $f''(3) = 18-12 = 6 > 0$ → minimum

2. $f'(x) = 2xe^x + x^2e^x = xe^x(2 + x)$
   $x = 0$: $f(0) = 0$, $f''(0) = 2 > 0$ → minimum
   $x = -2$: $f(-2) = 4e^{-2}$, $f''(-2) = -2e^{-2} < 0$ → maximum

3. $f'(x) = 3x^2 + a$, $f'(1) = 3 + a = 0$ → $a = -3$
   $f(1) = 1 + (-3)(1) + b = 4$ → $b = 6$

4. $f'(x) = 6x^2 - 6x - 12 = 6(x^2 - x - 2) = 6(x-2)(x+1)$
   $x = -1$: $f(-1) = -2 - 3 + 12 + 5 = 12$, $f''(-1) = -12 - 6 = -18 < 0$ → maximum $12$
   $x = 2$: $f(2) = 16 - 12 - 24 + 5 = -15$, $f''(2) = 24 - 6 = 18 > 0$ → minimum $-15$

### 5.7 Connected Rates of Change and Small Increments Approximation

1. $A = s^2$, $\frac{dA}{dt} = 2s\frac{ds}{dt} = 2(10)(3) = 60$ cm²/s

2. $f(x) = x^{1/3}$, $f'(x) = \frac{1}{3}x^{-2/3}$, take $a = 8$, $\delta x = 0.03$
   $f(8) = 2$, $f'(8) = \frac{1}{3}(8)^{-2/3} = \frac{1}{3}\cdot\frac{1}{4} = \frac{1}{12}$
   $\sqrt[3]{8.03} \approx 2 + \frac{1}{12} \times 0.03 = 2 + 0.0025 = 2.0025$

3. $V = \frac{4}{3}\pi r^3$, $\frac{dV}{dt} = 4\pi r^2\frac{dr}{dt}$
   $16\pi = 4\pi(2)^2\frac{dr}{dt} = 16\pi\frac{dr}{dt}$ → $\frac{dr}{dt} = 1$ m/s

### 5.8 Practical Maxima and Minima Problems

1. Let length be $x$, width be $y$, $2x + 2y = 120$, $y = 60 - x$
   $A = xy = x(60-x) = 60x - x^2$
   $A'(x) = 60 - 2x = 0$ → $x = 30$, $y = 30$
   $A''(x) = -2 < 0$ → maximum
   Maximum area $= 30 \times 30 = 900$ m²

2. $d^2 = x^2 + (x^2 - 4x + 5)^2$
   Let $g(x) = d^2$, differentiate and find the minimum.
   
   Simpler approach: let $h(x) = x^2 + (x^2-4x+5)^2$
   $h'(x) = 2x + 2(x^2-4x+5)(2x-4)$
   $= 2x + 2(x^2-4x+5)(2)(x-2)$
   $= 2x + 4(x^2-4x+5)(x-2)$
   
   Set $h'(x) = 0$, we can find $x = 2$.
   $d^2 = 2^2 + (4-8+5)^2 = 4 + 1 = 5$, $d = \sqrt{5}$

3. Surface area $S = \pi r^2 + 2\pi rh$, volume $V = \pi r^2 h$ (constant), $h = \frac{V}{\pi r^2}$
   $S = \pi r^2 + 2\pi r\left(\frac{V}{\pi r^2}\right) = \pi r^2 + \frac{2V}{r}$
   $S'(r) = 2\pi r - \frac{2V}{r^2} = 0$ → $2\pi r = \frac{2V}{r^2}$ → $\pi r^3 = V$ → $r^3 = \frac{V}{\pi}$
   And $V = \pi r^2 h$, so $\pi r^3 = \pi r^2 h$ → $r = h$
   **Answer**: $r : h = 1 : 1$, i.e., the base radius equals the height for minimum surface area.

---
---








# Chapter 6: Equations and Inequalities (Graphical Methods)

## Introduction

In previous chapters, we learned algebraic methods for solving equations and inequalities — factorisation, the quadratic formula, completing the square, etc. However, many equations and inequalities are difficult to handle purely algebraically, especially those involving absolute values, cubic polynomials, and complex substitutions. **Graphical methods** provide a powerful alternative approach: using the visual representation of functions to intuitively understand the solutions of equations and the solution sets of inequalities. Graphical methods do not always give exact values, but they help us quickly grasp the overall structure of the solution and provide geometric intuition for algebraic operations.

In this chapter, we will integrate knowledge from previous chapters — particularly the **discriminant and factorisation from Chapter 3 (Quadratic Functions)**, **absolute value function graphs from Chapter 4 (Functions)**, and **differentiation tools from Chapter 5 (Differentiation)** — to systematically handle five types of problems: absolute value equations, absolute value inequalities, substitution to reduce to quadratic equations, cubic polynomial graphs and inequalities, and graphical solutions of simultaneous equations.

---

## Syllabus Mapping (Cambridge IGCSE Additional Mathematics 0606, 2028–2030)

| Syllabus Ref | Content | Corresponding Section |
|---------|------|---------|
| 4.1 | Solve equations of the form $|ax+b| = c \;(c \ge 0)$, $|ax+b| = cx+d$, $|ax+b| = |cx+d|$, $|ax^2+bx+c| = d$ (algebraic or graphical methods) | 6.1 |
| 4.2 | Solve inequalities of the form $k|ax+b| > c\;(c\ge0)$, $k|ax+b| \le c\;(c>0)$, $k|ax+b| \le |cx+d|\;(k>0)$, $|ax+b| \le cx+d$, $|ax^2+bx+c| > d$, $|ax^2+bx+c| \le d$ | 6.2 |
| 4.3 | Construct and solve quadratic equations using substitution | 6.3 |
| 4.4 | Sketch graphs of cubic polynomials (products of three linear factors) and their absolute values | 6.4 |
| 4.5 | Solve cubic inequalities of the form $f(x) \ge d$, $f(x) > d$, $f(x) \le d$, $f(x) < d$ using graphical methods | 6.4 |
| 5.1 | Solve simultaneous linear equations in two variables by elimination or substitution | 6.5 |

---

## Prerequisite Knowledge: Sets and Interval Notation

> When solving inequalities, we usually use **intervals** or **sets** to express the solution set. This section reviews basic set notation and interval representation, which form the foundation for all content in this chapter.

### Basic Concepts of Sets

A **set** is a collection of distinct, well-defined objects. The objects in a set are called **elements**.

- $a \in A$: $a$ belongs to set $A$ ($a$ is an element of $A$)
- $a \notin A$: $a$ does not belong to set $A$

**Common number sets**:

- $\mathbb{N} = \{1, 2, 3, 4, \dots\}$: Natural numbers
- $\mathbb{Z} = \{\dots, -2, -1, 0, 1, 2, \dots\}$: Integers
- $\mathbb{Q}$: Rational numbers (numbers that can be expressed as fractions)
- $\mathbb{R}$: Real numbers (including rational and irrational numbers)
- $\mathbb{R}^+$: Positive real numbers
- $\emptyset$: Empty set (a set containing no elements)

**Representation of sets**:

**Roster form**: $A = \{1, 2, 3, 4, 5\}$

**Set-builder form**: $A = \{x \mid x \text{ is an integer greater than 0 and less than 6}\}$, or more generally $A = \{x \in \mathbb{R} \mid x^2 < 4\}$ (representing all real numbers $x$ satisfying $x^2 < 4$).

### Interval Notation

An interval is a subset of the real numbers, represented by a continuous segment on the number line.

| Type | Inequality | Interval Notation | Number Line |
|---------|-----------|---------|---------|
| Closed interval | $a \le x \le b$ | $[a, b]$ | Solid dots at both ends |
| Open interval | $a < x < b$ | $(a, b)$ | Open dots at both ends |
| Left-closed right-open | $a \le x < b$ | $[a, b)$ | Solid left, open right |
| Left-open right-closed | $a < x \le b$ | $(a, b]$ | Open left, solid right |
| Infinite interval | $x \ge a$ | $[a, \infty)$ | Extends rightward |
| Infinite interval | $x > a$ | $(a, \infty)$ | Extends rightward |
| Infinite interval | $x \le b$ | $(-\infty, b]$ | Extends leftward |
| Infinite interval | $x < b$ | $(-\infty, b)$ | Extends leftward |
| All real numbers | $x \in \mathbb{R}$ | $(-\infty, \infty)$ | Entire number line |

> ⚠️ **Note**: $\infty$ (infinity) is not a number but a concept representing "unbounded extension." Therefore the end involving $\infty$ is always written with a round bracket (open interval).

### Set Operations

**Union** $A \cup B = \{x \mid x \in A \text{ or } x \in B\}$: All elements belonging to $A$ **or** $B$.

**Intersection** $A \cap B = \{x \mid x \in A \text{ and } x \in B\}$: All elements belonging to both $A$ **and** $B$.

**Example**: Let $A = \{x \mid x < 1\}$, $B = \{x \mid x \ge -2\}$.

- $A \cap B = \{x \mid -2 \le x < 1\} = [-2, 1)$
- $A \cup B = \mathbb{R} = (-\infty, \infty)$

**Example**: Solving $x^2 - 5x + 6 > 0$ gives $x < 2$ or $x > 3$, with solution set expressed in interval notation as $(-\infty, 2) \cup (3, \infty)$. Here $\cup$ represents the "union" of the two intervals — $x$ can satisfy either one.

---

## 6.1 Absolute Value Equations

### 6.1.1 Definition and Geometric Meaning of Absolute Value

Geometrically, the absolute value $|A|$ represents the **distance** from point $A$ to the origin on the number line. Algebraically, it is defined as:

$$
|x| = \begin{cases}
x, & x \ge 0 \\
-x, & x < 0
\end{cases}
$$

Important properties of absolute value:
- $|A| \ge 0$ for all real numbers $A$
- $|A|^2 = A^2$
- $|AB| = |A| \cdot |B|$
- $\left|\dfrac{A}{B}\right| = \dfrac{|A|}{|B|}$ ($B \neq 0$)

The core idea behind solving absolute value equations is **removing the absolute value sign**, usually achieved through case analysis or squaring both sides.

### 6.1.2 Type $|ax + b| = c \quad (c \ge 0)$

This is the simplest absolute value equation. By definition, $|ax + b| = c$ is equivalent to:

$$
ax + b = c \quad \text{or} \quad ax + b = -c
$$

---

**Example 1**: Solve $|3x - 7| = 5$.

**Solution**:

$$
3x - 7 = 5 \quad \text{or} \quad 3x - 7 = -5
$$

$$
3x = 12 \quad \text{or} \quad 3x = 2
$$

$$
x = 4 \quad \text{or} \quad x = \frac{2}{3}
$$

Verification: $|3(4) - 7| = |12 - 7| = 5$ ✓, $|3(\frac{2}{3}) - 7| = |2 - 7| = 5$ ✓.

---

**Example 2**: Solve $|5 - 2x| = 9$.

**Solution**:

$$
5 - 2x = 9 \quad \text{or} \quad 5 - 2x = -9
$$

$$
-2x = 4 \quad \text{or} \quad -2x = -14
$$

$$
x = -2 \quad \text{or} \quad x = 7
$$

Verification: $|5 - 2(-2)| = |5 + 4| = 9$ ✓, $|5 - 2(7)| = |5 - 14| = 9$ ✓.

---

**Example 3**: Solve $|4x + 3| = 0$.

**Solution**:

$$
4x + 3 = 0
$$

$$
x = -\frac{3}{4}
$$

Note: When $c = 0$, there is only one solution, because $4x + 3$ equals both $0$ and $-0$ (the same). Verification: $|4(-\frac{3}{4}) + 3| = |-3 + 3| = 0$ ✓.

---

### 6.1.3 Type $|ax + b| = cx + d$

When the right-hand side also contains a variable, we cannot simply split into two equations — we must ensure the right-hand side is non-negative (absolute value is always non-negative, so the right-hand side must also be non-negative).

**Method 1: Case analysis** (based on the sign of $ax + b$).

**Method 2: Squaring both sides** to obtain a quadratic equation, then checking the solutions.

---

**Example 4**: Solve $|2x - 3| = x + 1$.

**Solution (Case analysis)**:

**Case 1**: $2x - 3 \ge 0$, i.e., $x \ge \frac{3}{2}$.
Then $|2x - 3| = 2x - 3$, and the equation becomes:

$$
2x - 3 = x + 1 \Rightarrow x = 4
$$

Check the condition: $4 \ge \frac{3}{2}$ ✓.

**Case 2**: $2x - 3 < 0$, i.e., $x < \frac{3}{2}$.
Then $|2x - 3| = -(2x - 3) = -2x + 3$, and the equation becomes:

$$
-2x + 3 = x + 1 \Rightarrow -3x = -2 \Rightarrow x = \frac{2}{3}
$$

Check the condition: $\frac{2}{3} < \frac{3}{2}$ ✓.

Therefore the solutions are $x = 4$ and $x = \frac{2}{3}$.

**Solution (Squaring and checking)**:

Square both sides: $(2x - 3)^2 = (x + 1)^2$

$$
4x^2 - 12x + 9 = x^2 + 2x + 1
$$

$$
3x^2 - 14x + 8 = 0
$$

$$
(3x - 2)(x - 4) = 0
$$

$$
x = \frac{2}{3} \quad \text{or} \quad x = 4
$$

Verification: For $x = 4$, the right-hand side $4 + 1 = 5 > 0$ ✓; for $x = \frac{2}{3}$, the right-hand side $\frac{2}{3} + 1 = \frac{5}{3} > 0$ ✓. Both solutions are valid.

---

**Example 5**: Solve $|x + 2| = 2x - 1$.

**Solution**:

**Case 1**: $x + 2 \ge 0$, i.e., $x \ge -2$.

$$
x + 2 = 2x - 1 \Rightarrow 3 = x \Rightarrow x = 3
$$

Check: $3 \ge -2$ ✓. Verify the right-hand side: $2(3) - 1 = 5 > 0$ ✓.

**Case 2**: $x + 2 < 0$, i.e., $x < -2$.

$$
-(x + 2) = 2x - 1 \Rightarrow -x - 2 = 2x - 1 \Rightarrow -1 = 3x \Rightarrow x = -\frac{1}{3}
$$

Check the condition: $-\frac{1}{3} < -2$? No! $-\frac{1}{3} > -2$, so this solution is invalid.

Therefore the only solution is $x = 3$.

---

**Example 6**: Solve $|3x + 1| = 2 - x$.

**Solution**:

**Case 1**: $3x + 1 \ge 0$, i.e., $x \ge -\frac{1}{3}$.

$$
3x + 1 = 2 - x \Rightarrow 4x = 1 \Rightarrow x = \frac{1}{4}
$$

Check: $\frac{1}{4} \ge -\frac{1}{3}$ ✓. Right-hand side: $2 - \frac{1}{4} = \frac{7}{4} > 0$ ✓.

**Case 2**: $3x + 1 < 0$, i.e., $x < -\frac{1}{3}$.

$$
-(3x + 1) = 2 - x \Rightarrow -3x - 1 = 2 - x \Rightarrow -2x = 3 \Rightarrow x = -\frac{3}{2}
$$

Check: $-\frac{3}{2} < -\frac{1}{3}$ ✓. Right-hand side: $2 - (-\frac{3}{2}) = \frac{7}{2} > 0$ ✓.

Therefore the solutions are $x = \frac{1}{4}$ and $x = -\frac{3}{2}$.

---

### 6.1.4 Type $|ax + b| = |cx + d|$

When two absolute values are equal, it means the two expressions are either equal or opposites. No case analysis conditions are needed.

$$
|ax + b| = |cx + d| \quad \Longleftrightarrow \quad ax + b = cx + d \quad \text{or} \quad ax + b = -(cx + d)
$$

---

**Example 7**: Solve $|2x + 5| = |x - 3|$.

**Solution**:

$$
2x + 5 = x - 3 \quad \text{or} \quad 2x + 5 = -(x - 3)
$$

**Equation 1**: $2x + 5 = x - 3 \Rightarrow x = -8$

**Equation 2**: $2x + 5 = -x + 3 \Rightarrow 3x = -2 \Rightarrow x = -\frac{2}{3}$

Therefore the solutions are $x = -8$ and $x = -\frac{2}{3}$.

Verification: $|2(-8) + 5| = |-11| = 11$, $|(-8) - 3| = |-11| = 11$ ✓.
$|2(-\frac{2}{3}) + 5| = |-\frac{4}{3} + 5| = |\frac{11}{3}| = \frac{11}{3}$, $|-\frac{2}{3} - 3| = |-\frac{11}{3}| = \frac{11}{3}$ ✓.

---

**Example 8**: Solve $|5x - 2| = |3x + 4|$.

**Solution**:

$$
5x - 2 = 3x + 4 \quad \text{or} \quad 5x - 2 = -(3x + 4)
$$

**Equation 1**: $5x - 2 = 3x + 4 \Rightarrow 2x = 6 \Rightarrow x = 3$

**Equation 2**: $5x - 2 = -3x - 4 \Rightarrow 8x = -2 \Rightarrow x = -\frac{1}{4}$

Therefore the solutions are $x = 3$ and $x = -\frac{1}{4}$.

---

**Example 9**: Solve $|x + 1| = |2x - 5|$.

**Solution**:

$$
x + 1 = 2x - 5 \quad \text{or} \quad x + 1 = -(2x - 5)
$$

**Equation 1**: $x + 1 = 2x - 5 \Rightarrow 6 = x \Rightarrow x = 6$

**Equation 2**: $x + 1 = -2x + 5 \Rightarrow 3x = 4 \Rightarrow x = \frac{4}{3}$

Therefore the solutions are $x = 6$ and $x = \frac{4}{3}$.

---

### 6.1.5 Type $|ax^2 + bx + c| = d$

When the expression inside the absolute value is a quadratic function, the approach is the same: removing the absolute value gives two quadratic equations.

---

**Example 10**: Solve $|x^2 - 4x + 3| = 3$.

**Solution**:

$$
x^2 - 4x + 3 = 3 \quad \text{or} \quad x^2 - 4x + 3 = -3
$$

**Equation 1**: $x^2 - 4x = 0 \Rightarrow x(x - 4) = 0 \Rightarrow x = 0$ or $x = 4$

**Equation 2**: $x^2 - 4x + 6 = 0$

Discriminant $\Delta = (-4)^2 - 4(1)(6) = 16 - 24 = -8 < 0$, no real solutions.

Therefore the solutions are $x = 0$ and $x = 4$.

---

**Example 11**: Solve $|2x^2 - 5x - 3| = 2$.

**Solution**:

$$
2x^2 - 5x - 3 = 2 \quad \text{or} \quad 2x^2 - 5x - 3 = -2
$$

**Equation 1**: $2x^2 - 5x - 5 = 0$

$$
x = \frac{5 \pm \sqrt{25 - 4(2)(-5)}}{2(2)} = \frac{5 \pm \sqrt{25 + 40}}{4} = \frac{5 \pm \sqrt{65}}{4}
$$

**Equation 2**: $2x^2 - 5x - 1 = 0$

$$
x = \frac{5 \pm \sqrt{25 - 4(2)(-1)}}{4} = \frac{5 \pm \sqrt{25 + 8}}{4} = \frac{5 \pm \sqrt{33}}{4}
$$

Therefore there are four solutions: $x = \frac{5 \pm \sqrt{65}}{4}$ and $x = \frac{5 \pm \sqrt{33}}{4}$.

---

**Example 12**: Solve $|x^2 - 9| = 7$.

**Solution**:

$$
x^2 - 9 = 7 \quad \text{or} \quad x^2 - 9 = -7
$$

**Equation 1**: $x^2 = 16 \Rightarrow x = \pm 4$

**Equation 2**: $x^2 = 2 \Rightarrow x = \pm \sqrt{2}$

Therefore the solutions are $x = 4, -4, \sqrt{2}, -\sqrt{2}$.

---

## 6.2 Absolute Value Inequalities

The core idea of absolute value inequalities: **transform the absolute value inequality into a system of inequalities without absolute value**, then solve using the number line or graphs.

### 6.2.1 Basic Types $|ax + b| > c$ and $|ax + b| \le c$

**Core rules** ($c > 0$):

$$
|ax + b| > c \quad \Longleftrightarrow \quad ax + b < -c \quad \text{or} \quad ax + b > c
$$

$$
|ax + b| \le c \quad \Longleftrightarrow \quad -c \le ax + b \le c
$$

> Memory aid: "**Greater than → outside, less than → middle**."

For $k|ax + b| > c$ ($k > 0$, $c \ge 0$), first divide both sides by $k$ to get the standard form: $|ax + b| > \frac{c}{k}$.

---

**Example 1**: Solve $|2x - 5| > 3$.

**Solution**:

"Greater than → outside":

$$
2x - 5 < -3 \quad \text{or} \quad 2x - 5 > 3
$$

$$
2x < 2 \quad \text{or} \quad 2x > 8
$$

$$
x < 1 \quad \text{or} \quad x > 4
$$

Solution set: $x \in (-\infty, 1) \cup (4, \infty)$.

---

**Example 2**: Solve $3|2x + 1| \le 15$.

**Solution**:

First divide by $3$: $|2x + 1| \le 5$

"Less than → middle":

$$
-5 \le 2x + 1 \le 5
$$

Left: $-5 \le 2x + 1 \Rightarrow -6 \le 2x \Rightarrow x \ge -3$
Right: $2x + 1 \le 5 \Rightarrow 2x \le 4 \Rightarrow x \le 2$

Therefore the solution set is $-3 \le x \le 2$, i.e., $x \in [-3, 2]$.

---

**Example 3**: Solve $2|4 - x| > 10$.

**Solution**:

Divide by $2$: $|4 - x| > 5$

"Greater than → outside":

$$
4 - x < -5 \quad \text{or} \quad 4 - x > 5
$$

$$
-x < -9 \quad \text{or} \quad -x > 1
$$

$$
x > 9 \quad \text{or} \quad x < -1
$$

Solution set: $x \in (-\infty, -1) \cup (9, \infty)$.

---

### 6.2.2 Type $k|ax + b| \le |cx + d| \quad (k > 0)$

When both sides have absolute values, the most reliable method is **squaring both sides**, using the property $|A|^2 = A^2$ to obtain an inequality without absolute values.

---

**Example 4**: Solve $|2x - 1| \le |x + 3|$.

**Solution**:

Square both sides (the inequality sign remains unchanged since both sides are non-negative):

$$
(2x - 1)^2 \le (x + 3)^2
$$

$$
4x^2 - 4x + 1 \le x^2 + 6x + 9
$$

$$
3x^2 - 10x - 8 \le 0
$$

Solve $3x^2 - 10x - 8 = 0$:

$$
x = \frac{10 \pm \sqrt{100 + 96}}{6} = \frac{10 \pm \sqrt{196}}{6} = \frac{10 \pm 14}{6}
$$

$$
x = \frac{24}{6} = 4 \quad \text{or} \quad x = \frac{-4}{6} = -\frac{2}{3}
$$

The coefficient of $x^2$ is $3 > 0$, so the parabola opens upward, and $3x^2 - 10x - 8 \le 0$ is satisfied between the roots:

$$
-\frac{2}{3} \le x \le 4
$$

i.e., $x \in \left[-\frac{2}{3}, 4\right]$.

---

**Example 5**: Solve $2|x + 2| > |3x - 1|$.

**Solution**:

Square both sides:

$$
4(x + 2)^2 > (3x - 1)^2
$$

$$
4(x^2 + 4x + 4) > 9x^2 - 6x + 1
$$

$$
4x^2 + 16x + 16 > 9x^2 - 6x + 1
$$

$$
0 > 5x^2 - 22x - 15
$$

$$
5x^2 - 22x - 15 < 0
$$

Solve $5x^2 - 22x - 15 = 0$:

$$
x = \frac{22 \pm \sqrt{484 + 300}}{10} = \frac{22 \pm \sqrt{784}}{10} = \frac{22 \pm 28}{10}
$$

$$
x = \frac{50}{10} = 5 \quad \text{or} \quad x = \frac{-6}{10} = -\frac{3}{5}
$$

The coefficient of $x^2$ is $5 > 0$, so the solution of $5x^2 - 22x - 15 < 0$ is:

$$
-\frac{3}{5} < x < 5
$$

i.e., $x \in \left(-\frac{3}{5}, 5\right)$.

---

**Example 6**: Solve $3|x - 1| \le 2|x + 2|$.

**Solution**:

Square both sides:

$$
9(x - 1)^2 \le 4(x + 2)^2
$$

$$
9(x^2 - 2x + 1) \le 4(x^2 + 4x + 4)
$$

$$
9x^2 - 18x + 9 \le 4x^2 + 16x + 16
$$

$$
5x^2 - 34x - 7 \le 0
$$

Solve $5x^2 - 34x - 7 = 0$:

$$
x = \frac{34 \pm \sqrt{1156 + 140}}{10} = \frac{34 \pm \sqrt{1296}}{10} = \frac{34 \pm 36}{10}
$$

$$
x = \frac{70}{10} = 7 \quad \text{or} \quad x = \frac{-2}{10} = -\frac{1}{5}
$$

The coefficient of $x^2$ is $5 > 0$, so the solution of $5x^2 - 34x - 7 \le 0$ is:

$$
-\frac{1}{5} \le x \le 7
$$

i.e., $x \in \left[-\frac{1}{5}, 7\right]$.

---

### 6.2.3 Type $|ax + b| \le cx + d$

The right-hand side of this type of inequality is a linear expression. There are two methods: algebraic case analysis and graphical method.

**Algebraic case analysis**: Discuss based on the sign of $ax + b$, solve and check whether it satisfies the condition.

**Graphical method**: Draw the graphs of $y = |ax + b|$ and $y = cx + d$, and find the intervals where the former lies below (or above) the latter.

---

**Example 7**: Solve $|x - 3| \le 2x + 1$.

**Solution (Algebraic case analysis)**:

**Case 1**: $x - 3 \ge 0$, i.e., $x \ge 3$.

$$
x - 3 \le 2x + 1 \Rightarrow -4 \le x
$$

Combining with $x \ge 3$ gives $x \ge 3$.

**Case 2**: $x - 3 < 0$, i.e., $x < 3$.

$$
-(x - 3) \le 2x + 1 \Rightarrow -x + 3 \le 2x + 1 \Rightarrow 2 \le 3x \Rightarrow x \ge \frac{2}{3}
$$

Combining with $x < 3$ gives $\frac{2}{3} \le x < 3$.

Taking the union of both cases: $x \ge \frac{2}{3}$, i.e., $x \in \left[\frac{2}{3}, \infty\right)$.

---

**Example 8**: Solve $|2x + 5| > x + 4$.

**Solution**:

**Case 1**: $2x + 5 \ge 0$, i.e., $x \ge -\frac{5}{2}$.

$$
2x + 5 > x + 4 \Rightarrow x > -1
$$

Combining with $x \ge -\frac{5}{2}$ gives $x > -1$.

**Case 2**: $2x + 5 < 0$, i.e., $x < -\frac{5}{2}$.

$$
-(2x + 5) > x + 4 \Rightarrow -2x - 5 > x + 4 \Rightarrow -3x > 9 \Rightarrow x < -3
$$

Combining with $x < -\frac{5}{2}$ gives $x < -3$.

Solution set: $x \in (-\infty, -3) \cup (-1, \infty)$.

---

**Example 9**: Solve $|x + 2| \le 3x - 1$.

**Solution**:

**Case 1**: $x + 2 \ge 0$, i.e., $x \ge -2$.

$$
x + 2 \le 3x - 1 \Rightarrow 3 \le 2x \Rightarrow x \ge \frac{3}{2}
$$

Combining with $x \ge -2$ gives $x \ge \frac{3}{2}$.

**Case 2**: $x + 2 < 0$, i.e., $x < -2$.

$$
-(x + 2) \le 3x - 1 \Rightarrow -x - 2 \le 3x - 1 \Rightarrow -1 \le 4x \Rightarrow x \ge -\frac{1}{4}
$$

But the condition is $x < -2$, and $-\frac{1}{4} > -2$, so there is no valid solution.

Therefore the solution set is $x \ge \frac{3}{2}$, i.e., $x \in \left[\frac{3}{2}, \infty\right)$.

---

### 6.2.4 Type $|ax^2 + bx + c| > d$ and $|ax^2 + bx + c| \le d$

Approach: Remove the absolute value to obtain two quadratic inequalities, solve each separately, then take the union or intersection.

---

**Example 10**: Solve $|x^2 - 3x| \le 4$.

**Solution**:

From $|f(x)| \le 4$ we get $-4 \le x^2 - 3x \le 4$.

**Left inequality**: $x^2 - 3x \ge -4$

$$
x^2 - 3x + 4 \ge 0
$$

Discriminant $\Delta = 9 - 16 = -7 < 0$, and the coefficient of $x^2$ is $1 > 0$, so $x^2 - 3x + 4 > 0$ holds for all $x$. The left inequality is automatically satisfied.

**Right inequality**: $x^2 - 3x \le 4$

$$
x^2 - 3x - 4 \le 0
$$

$$
(x - 4)(x + 1) \le 0
$$

Solution: $-1 \le x \le 4$.

Therefore the solution set of the original inequality is $x \in [-1, 4]$.

---

**Example 11**: Solve $|x^2 - 2x - 3| > 3$.

**Solution**:

From $|f(x)| > 3$ we get $x^2 - 2x - 3 < -3$ or $x^2 - 2x - 3 > 3$.

**Inequality 1**: $x^2 - 2x - 3 < -3$

$$
x^2 - 2x < 0 \Rightarrow x(x - 2) < 0 \Rightarrow 0 < x < 2
$$

**Inequality 2**: $x^2 - 2x - 3 > 3$

$$
x^2 - 2x - 6 > 0
$$

Solve $x^2 - 2x - 6 = 0$:

$$
x = \frac{2 \pm \sqrt{4 + 24}}{2} = \frac{2 \pm \sqrt{28}}{2} = \frac{2 \pm 2\sqrt{7}}{2} = 1 \pm \sqrt{7}
$$

The coefficient of $x^2$ is $1 > 0$, so $x^2 - 2x - 6 > 0$ holds for:

$$
x < 1 - \sqrt{7} \quad \text{or} \quad x > 1 + \sqrt{7}
$$

where $1 - \sqrt{7} \approx 1 - 2.646 = -1.646$, $1 + \sqrt{7} \approx 3.646$.

The solution set of the original inequality is the union of the two inequality solution sets:

$$
x \in (-\infty, 1 - \sqrt{7}) \cup (0, 2) \cup (1 + \sqrt{7}, \infty)
$$

---

**Example 12**: Solve $|2x^2 + x - 1| \le 5$.

**Solution**:

From $-5 \le 2x^2 + x - 1 \le 5$.

**Left inequality**: $2x^2 + x - 1 \ge -5$

$$
2x^2 + x + 4 \ge 0
$$

Discriminant $\Delta = 1 - 32 = -31 < 0$, coefficient of $x^2$ is $2 > 0$, always true.

**Right inequality**: $2x^2 + x - 1 \le 5$

$$
2x^2 + x - 6 \le 0
$$

Solve $2x^2 + x - 6 = 0$:

$$
x = \frac{-1 \pm \sqrt{1 + 48}}{4} = \frac{-1 \pm \sqrt{49}}{4} = \frac{-1 \pm 7}{4}
$$

$$
x = \frac{6}{4} = \frac{3}{2} \quad \text{or} \quad x = \frac{-8}{4} = -2
$$

The coefficient of $x^2$ is $2 > 0$, so $2x^2 + x - 6 \le 0$ holds for:

$$
-2 \le x \le \frac{3}{2}
$$

Therefore the solution set is $x \in \left[-2, \frac{3}{2}\right]$.

---

## 6.3 Substitution to Reduce to a Quadratic Equation

Some equations do not initially look like quadratic equations, but through clever **substitution** they can be transformed into familiar quadratic equations. The core of the substitution method is identifying a repeated structure in the expression, letting $u$ represent it, thereby simplifying the original equation.

### 6.3.1 Exponential Substitution

Equations of the form $a^{2x} + b \cdot a^x + c = 0$ can be solved by letting $u = a^x$ ($u > 0$), then $a^{2x} = (a^x)^2 = u^2$.

For equations like $3e^x = 12 - 5e^{-x}$, multiply both sides by $e^x$ and then let $u = e^x$.

---

**Example 1**: Solve $4^x - 5 \cdot 2^x + 4 = 0$.

**Solution**:

Note that $4^x = (2^2)^x = (2^x)^2$. Let $u = 2^x > 0$, then:

$$
u^2 - 5u + 4 = 0
$$

$$
(u - 1)(u - 4) = 0
$$

$$
u = 1 \quad \text{or} \quad u = 4
$$

Back-substitute $u = 2^x$:

- $2^x = 1 \Rightarrow x = 0$ (since $2^0 = 1$)
- $2^x = 4 \Rightarrow x = 2$ (since $2^2 = 4$)

Therefore the solutions are $x = 0$ and $x = 2$.

---

**Example 2**: Solve $2e^x = 7 - 3e^{-x}$.

**Solution**:

Multiply both sides by $e^x$ ($e^x > 0$, so no extraneous roots are introduced):

$$
2e^{2x} = 7e^x - 3
$$

$$
2e^{2x} - 7e^x + 3 = 0
$$

Let $u = e^x > 0$, then:

$$
2u^2 - 7u + 3 = 0
$$

$$
(2u - 1)(u - 3) = 0
$$

$$
u = \frac{1}{2} \quad \text{or} \quad u = 3
$$

Back-substitute $u = e^x$:

- $e^x = \frac{1}{2} \Rightarrow x = \ln \frac{1}{2} = -\ln 2$
- $e^x = 3 \Rightarrow x = \ln 3$

Therefore the solutions are $x = -\ln 2$ and $x = \ln 3$.

---

**Example 3**: Solve $3^{2x+1} - 10 \cdot 3^x + 3 = 0$.

**Solution**:

Note that $3^{2x+1} = 3 \cdot 3^{2x} = 3(3^x)^2$. Let $u = 3^x > 0$, then:

$$
3u^2 - 10u + 3 = 0
$$

$$
(3u - 1)(u - 3) = 0
$$

$$
u = \frac{1}{3} \quad \text{or} \quad u = 3
$$

Back-substitute $u = 3^x$:

- $3^x = \frac{1}{3} = 3^{-1} \Rightarrow x = -1$
- $3^x = 3 \Rightarrow x = 1$

Therefore the solutions are $x = -1$ and $x = 1$.

---

### 6.3.2 Logarithmic Substitution

Equations of the form $(\ln x)^2 + a \ln x + b = 0$ or $2(\ln 5x)^2 + \ln 5x - 6 = 0$ can be solved by letting $u = \ln(g(x))$.

---

**Example 4**: Solve $(\ln x)^2 - 3\ln x + 2 = 0$.

**Solution**:

Let $u = \ln x$, then:

$$
u^2 - 3u + 2 = 0
$$

$$
(u - 1)(u - 2) = 0
$$

$$
u = 1 \quad \text{or} \quad u = 2
$$

Back-substitute $u = \ln x$:

- $\ln x = 1 \Rightarrow x = e^1 = e$
- $\ln x = 2 \Rightarrow x = e^2$

Therefore the solutions are $x = e$ and $x = e^2$.

---

**Example 5**: Solve $2(\ln 5x)^2 + \ln 5x - 6 = 0$.

**Solution**:

Let $u = \ln 5x$, then:

$$
2u^2 + u - 6 = 0
$$

Factorise:

$$
2u^2 + 4u - 3u - 6 = 0
$$

$$
2u(u + 2) - 3(u + 2) = 0
$$

$$
(u + 2)(2u - 3) = 0
$$

$$
u = -2 \quad \text{or} \quad u = \frac{3}{2}
$$

Back-substitute $u = \ln 5x$:

- $\ln 5x = -2 \Rightarrow 5x = e^{-2} \Rightarrow x = \frac{1}{5}e^{-2}$
- $\ln 5x = \frac{3}{2} \Rightarrow 5x = e^{3/2} \Rightarrow x = \frac{1}{5}e^{3/2}$

Therefore the solutions are $x = \frac{1}{5}e^{-2}$ and $x = \frac{1}{5}e^{3/2}$.

---

**Example 6**: Solve $\log_3 x + \log_x 3 = 2$.

**Solution**:

Use the change of base formula: $\log_x 3 = \frac{\log_3 3}{\log_3 x} = \frac{1}{\log_3 x}$.

Let $u = \log_3 x$ (note $x > 0$ and $x \neq 1$, so $u \neq 0$), then:

$$
u + \frac{1}{u} = 2
$$

$$
u^2 + 1 = 2u
$$

$$
u^2 - 2u + 1 = 0
$$

$$
(u - 1)^2 = 0
$$

$$
u = 1
$$

Back-substitute: $\log_3 x = 1 \Rightarrow x = 3^1 = 3$.

Verification: $\log_3 3 + \log_3 3 = 1 + 1 = 2$ ✓.

---

### 6.3.3 Radical Substitution

For equations of the form $x - 6\sqrt{x} + 8 = 0$, let $u = \sqrt{x}$ ($u \ge 0$), then $x = u^2$.

More generally, for equations like $x^{\frac{2}{3}} - 4x^{\frac{1}{3}} + 2 = 0$, let $u = x^{\frac{1}{3}}$, then $x^{\frac{2}{3}} = u^2$.

---

**Example 7**: Solve $x - 7\sqrt{x} + 12 = 0$.

**Solution**:

Let $u = \sqrt{x} \ge 0$, then $x = u^2$.

$$
u^2 - 7u + 12 = 0
$$

$$
(u - 3)(u - 4) = 0
$$

$$
u = 3 \quad \text{or} \quad u = 4
$$

Back-substitute $u = \sqrt{x}$:

- $\sqrt{x} = 3 \Rightarrow x = 9$
- $\sqrt{x} = 4 \Rightarrow x = 16$

Verification: $9 - 7\sqrt{9} + 12 = 9 - 21 + 12 = 0$ ✓, $16 - 7\sqrt{16} + 12 = 16 - 28 + 12 = 0$ ✓.

---

**Example 8**: Solve $x^{\frac{2}{3}} - 4x^{\frac{1}{3}} + 3 = 0$.

**Solution**:

Let $u = x^{\frac{1}{3}}$, then $x^{\frac{2}{3}} = u^2$.

$$
u^2 - 4u + 3 = 0
$$

$$
(u - 1)(u - 3) = 0
$$

$$
u = 1 \quad \text{or} \quad u = 3
$$

Back-substitute $u = x^{\frac{1}{3}}$:

- $x^{\frac{1}{3}} = 1 \Rightarrow x = 1^3 = 1$
- $x^{\frac{1}{3}} = 3 \Rightarrow x = 3^3 = 27$

Verification: $1^{\frac{2}{3}} - 4(1)^{\frac{1}{3}} + 3 = 1 - 4 + 3 = 0$ ✓, $27^{\frac{2}{3}} - 4(27)^{\frac{1}{3}} + 3 = 9 - 12 + 3 = 0$ ✓.

---

**Example 9**: Solve $2x + 3\sqrt{x} - 2 = 0$.

**Solution**:

Let $u = \sqrt{x} \ge 0$, then $x = u^2$.

$$
2u^2 + 3u - 2 = 0
$$

$$
(2u - 1)(u + 2) = 0
$$

$$
u = \frac{1}{2} \quad \text{or} \quad u = -2
$$

$u = \sqrt{x} \ge 0$, so $u = -2$ is invalid.

Back-substitute: $\sqrt{x} = \frac{1}{2} \Rightarrow x = \frac{1}{4}$.

Verification: $2(\frac{1}{4}) + 3\sqrt{\frac{1}{4}} - 2 = \frac{1}{2} + \frac{3}{2} - 2 = 0$ ✓.

---

### 6.3.4 Fraction Substitution

For equations of the form $x^2 + \frac{1}{x^2} + a\left(x + \frac{1}{x}\right) + b = 0$, use the relationship $(x + \frac{1}{x})^2 = x^2 + 2 + \frac{1}{x^2}$ and let $u = x + \frac{1}{x}$.

---

**Example 10**: Solve $x^2 + \frac{1}{x^2} - 5\left(x + \frac{1}{x}\right) + 6 = 0$.

**Solution**:

Let $u = x + \frac{1}{x}$, then $u^2 = x^2 + 2 + \frac{1}{x^2}$, so $x^2 + \frac{1}{x^2} = u^2 - 2$.

The original equation becomes:

$$
(u^2 - 2) - 5u + 6 = 0
$$

$$
u^2 - 5u + 4 = 0
$$

$$
(u - 1)(u - 4) = 0
$$

$$
u = 1 \quad \text{or} \quad u = 4
$$

**Back-substitute $u = 1$**: $x + \frac{1}{x} = 1$

Multiply both sides by $x$ ($x \neq 0$): $x^2 + 1 = x \Rightarrow x^2 - x + 1 = 0$.

Discriminant $\Delta = 1 - 4 = -3 < 0$, no real solutions.

**Back-substitute $u = 4$**: $x + \frac{1}{x} = 4$

$$
x^2 + 1 = 4x \Rightarrow x^2 - 4x + 1 = 0
$$

$$
x = \frac{4 \pm \sqrt{16 - 4}}{2} = \frac{4 \pm \sqrt{12}}{2} = \frac{4 \pm 2\sqrt{3}}{2} = 2 \pm \sqrt{3}
$$

Therefore the solutions are $x = 2 + \sqrt{3}$ and $x = 2 - \sqrt{3}$.

---

### 6.3.5 Trigonometric Substitution (Using Identities)

For equations of the form $\sin^2 x + \sin x - 2 = 0$, let $u = \sin x$, but note the domain restriction $u \in [-1, 1]$.

---

**Example 11**: Solve $2\cos^2 x + 3\sin x - 3 = 0$, $x \in [0, 2\pi)$.

**Solution**:

Use the identity $\cos^2 x = 1 - \sin^2 x$:

$$
2(1 - \sin^2 x) + 3\sin x - 3 = 0
$$

$$
2 - 2\sin^2 x + 3\sin x - 3 = 0
$$

$$
-2\sin^2 x + 3\sin x - 1 = 0
$$

Multiply by $-1$:

$$
2\sin^2 x - 3\sin x + 1 = 0
$$

Let $u = \sin x$, $u \in [-1, 1]$:

$$
2u^2 - 3u + 1 = 0
$$

$$
(2u - 1)(u - 1) = 0
$$

$$
u = \frac{1}{2} \quad \text{or} \quad u = 1
$$

Back-substitute:

- $\sin x = \frac{1}{2}$: on $[0, 2\pi)$, $x = \frac{\pi}{6}$ or $x = \frac{5\pi}{6}$
- $\sin x = 1$: on $[0, 2\pi)$, $x = \frac{\pi}{2}$

Therefore the solutions are $x = \frac{\pi}{6}, \frac{\pi}{2}, \frac{5\pi}{6}$.

---

## 6.4 Cubic Polynomial Graphs and Inequalities

### 6.4.1 Graph Features of Products of Three Linear Factors

A cubic polynomial $f(x) = (x - a)(x - b)(x - c)$ (where $a < b < c$) has the following graph features:

- **$x$-intercepts**: $x = a, x = b, x = c$ (three real roots)
- **End behaviour**: If the leading coefficient is positive, as $x \to \infty$, $f(x) \to \infty$; as $x \to -\infty$, $f(x) \to -\infty$
- **Graph shape**: Enters from the third quadrant, crosses through $x = a, x = b, x = c$ in sequence, and enters the first quadrant
- **Sign in each interval**:

| Interval | $(-\infty, a)$ | $(a, b)$ | $(b, c)$ | $(c, \infty)$ |
|------|--------|--------|--------|--------|
| $(x-a)$ | − | + | + | + |
| $(x-b)$ | − | − | + | + |
| $(x-c)$ | − | − | − | + |
| $f(x)$ sign | − | + | − | + |

---

**Example 1**: Sketch the graph of $f(x) = (x + 2)(x - 1)(x - 3)$.

**Solution**:

**$x$-intercepts**: $f(x) = 0 \Rightarrow x = -2, 1, 3$

**$y$-intercept**: $f(0) = (0 + 2)(0 - 1)(0 - 3) = 2 \times (-1) \times (-3) = 6$, point $(0, 6)$

**End behaviour**: Expanding, the leading term is $x^3$, coefficient positive. As $x \to -\infty$, $f(x) \to -\infty$; as $x \to \infty$, $f(x) \to \infty$.

**Sign table**:

| Interval | $(-\infty, -2)$ | $(-2, 1)$ | $(1, 3)$ | $(3, \infty)$ |
|------|-------|-------|-------|-------|
| $f(x)$ | − | + | − | + |

The graph enters from the third quadrant, crosses the $x$-axis at $x = -2$ going upward, passes through $(0, 6)$, crosses the $x$-axis at $x = 1$ going downward, reaches a local minimum, then rises to cross the $x$-axis for the third time at $x = 3$, and finally extends to the top-right.

---

**Example 2**: Sketch the graph of $f(x) = (2x - 1)(x + 1)(x - 2)$.

**Solution**:

**$x$-intercepts**: $(2x - 1)(x + 1)(x - 2) = 0 \Rightarrow x = \frac{1}{2}, -1, 2$

In order: $x = -1, \frac{1}{2}, 2$

**$y$-intercept**: $f(0) = (0 - 1)(0 + 1)(0 - 2) = (-1) \times 1 \times (-2) = 2$, point $(0, 2)$

**End behaviour**: Leading term is $2x \cdot x \cdot x = 2x^3$, coefficient positive ($2 > 0$).

**Sign table**:

| Interval | $(-\infty, -1)$ | $(-1, \frac{1}{2})$ | $(\frac{1}{2}, 2)$ | $(2, \infty)$ |
|------|---------|-------------|------------|--------|
| $(2x-1)$ | − | − | + | + |
| $(x+1)$ | − | + | + | + |
| $(x-2)$ | − | − | − | + |
| $f(x)$ | − | + | − | + |

---

**Example 3**: Sketch the graph of $f(x) = -(x + 3)(x - 1)(x - 4)$.

**Solution**:

Note the leading coefficient is negative: $-(x)(x)(x) = -x^3$. $x$-intercepts are $-3, 1, 4$.

**End behaviour**: As $x \to -\infty$, $f(x) \to \infty$ (because a negative cubic term means it enters from the second quadrant); as $x \to \infty$, $f(x) \to -\infty$.

**$y$-intercept**: $f(0) = -(3)(-1)(-4) = -(3)(-1)(-4) = -(12) = -12$, point $(0, -12)$

**Sign table**:

| Interval | $(-\infty, -3)$ | $(-3, 1)$ | $(1, 4)$ | $(4, \infty)$ |
|------|---------|--------|--------|--------|
| $-(x+3)$ | + (neg × neg) | − (neg × pos) | − | − |
| $(x-1)$ | − | − | + | + |
| $(x-4)$ | − | − | − | + |
| $f(x)$ | + | − | + | − |

---

### 6.4.2 Graphs of Absolute Value Cubic Functions $y = |f(x)|$

The graph of $y = |f(x)|$ is obtained by reflecting the parts of $y = f(x)$ that lie below the $x$-axis upward about the $x$-axis:

$$
|f(x)| = \begin{cases}
f(x), & f(x) \ge 0 \\
-f(x), & f(x) < 0
\end{cases}
$$

---

**Example 4**: Sketch the graph of $y = |(x + 2)(x - 1)(x - 3)|$.

**Solution**:

First sketch the graph of $f(x) = (x + 2)(x - 1)(x - 3)$.

$f(x)$ is negative on the intervals $(-\infty, -2)$ and $(1, 3)$.

Reflect these parts upward about the $x$-axis.

Final graph features:
- $x$-intercepts remain the same: $x = -2, 1, 3$ (at these points the graph "touches" the $x$-axis but does not cross)
- The entire graph lies above or on the $x$-axis
- The troughs on $(-\infty, -2)$ and $(1, 3)$ become peaks
- The peak on $(-2, 1)$ remains above

---

**Example 5**: Sketch the graph of $y = |(x - 1)(x - 2)(x - 4)|$ and label the axis intercepts.

**Solution**:

$f(x) = (x - 1)(x - 2)(x - 4)$ has $x$-intercepts at $1, 2, 4$.

Sign of $f(x)$:

| Interval | $(-\infty, 1)$ | $(1, 2)$ | $(2, 4)$ | $(4, \infty)$ |
|------|-------|-------|-------|-------|
| $f(x)$ | − | + | − | + |

$f(x)$ is negative on $(-\infty, 1)$ and $(2, 4)$. Reflect these parts upward.

$y$-intercept: $|f(0)| = |(-1)(-2)(-4)| = |-8| = 8$, point $(0, 8)$.

---

**Example 6**: Discuss how the number of solutions of $|(x + 1)(x - 2)(x - 5)| = k$ ($k > 0$) varies with $k$.

**Solution**:

Sketch the graph of $y = |(x + 1)(x - 2)(x - 5)|$. $x$-intercepts are $-1, 2, 5$.

Sign of $f(x) = (x + 1)(x - 2)(x - 5)$:

| Interval | $(-\infty, -1)$ | $(-1, 2)$ | $(2, 5)$ | $(5, \infty)$ |
|------|--------|--------|--------|--------|
| $f(x)$ | − | + | − | + |

Negative intervals (reflected upward): $(-\infty, -1)$ and $(2, 5)$.

Let $M_1$ be the maximum value of $f(x)$ on $(-1, 2)$, and $M_2$ be the maximum value of $|f(x)|$ on $(2, 5)$ (i.e., the absolute value of the minimum of $f(x)$ on $(2,5)$).

- If $0 < k < \min(M_1, M_2)$: 6 solutions (6 intersections of the horizontal line with the graph)
- If $k = M_1$ or $k = M_2$: some intersections coincide, the number of solutions decreases
- If $k > \max(M_1, M_2)$: 2 solutions

> **Note**: This type of problem usually appears in more difficult questions and requires combining derivatives to find local extreme values.

---

### 6.4.3 Graphical Solution of Cubic Inequalities

For $f(x) \ge d$ (or $>, \le, <$), where $f(x)$ is the product of three linear factors:

**Graphical solution steps**:

1. Sketch the graph of $y = f(x)$ (label the three $x$-intercepts and the $y$-intercept)
2. Draw the horizontal line $y = d$
3. Find the intervals where $f(x)$ is above the line (for $f(x) > d$) or below the line (for $f(x) < d$)
4. Find the intersection points if necessary

---

**Example 7**: Solve $(x + 1)(x - 2)(x - 4) \ge 0$.

**Solution**:

$f(x) = (x + 1)(x - 2)(x - 4)$, $d = 0$ (i.e., comparing with the $x$-axis).

The three roots are $-1, 2, 4$, and the leading coefficient is positive.

Sign table:

| Interval | $(-\infty, -1)$ | $(-1, 2)$ | $(2, 4)$ | $(4, \infty)$ |
|------|---------|--------|--------|--------|
| $f(x)$ | − | + | − | + |

$f(x) \ge 0$ holds for $x \in [-1, 2] \cup [4, \infty)$.

---

**Example 8**: Solve $(x - 1)(x - 3)(x - 5) < 0$.

**Solution**:

The three roots are $1, 3, 5$, and the leading coefficient is positive.

Sign table:

| Interval | $(-\infty, 1)$ | $(1, 3)$ | $(3, 5)$ | $(5, \infty)$ |
|------|------|------|------|------|
| $f(x)$ | − | + | − | + |

$f(x) < 0$ holds for $x \in (-\infty, 1) \cup (3, 5)$.

---

**Example 9**: Given $f(x) = (2x + 1)(x - 2)(x - 3)$, solve $f(x) \le 0$.

**Solution**:

Zeros: $2x + 1 = 0 \Rightarrow x = -\frac{1}{2}$, and $x = 2, x = 3$.

In order: $-\frac{1}{2}, 2, 3$.

Leading coefficient: $2x \cdot x \cdot x = 2x^3$, coefficient positive.

Sign table:

| Interval | $(-\infty, -\frac{1}{2})$ | $(-\frac{1}{2}, 2)$ | $(2, 3)$ | $(3, \infty)$ |
|------|-------------|-----------|--------|--------|
| $(2x+1)$ | − | + | + | + |
| $(x-2)$ | − | − | + | + |
| $(x-3)$ | − | − | − | + |
| $f(x)$ | − | + | − | + |

$f(x) \le 0$ holds for $x \in (-\infty, -\frac{1}{2}] \cup [2, 3]$.

---

## 6.5 Simultaneous Equations

### 6.5.1 Graphical Meaning of Simultaneous Equations

The solution to two simultaneous equations $\begin{cases} y = f(x) \\ y = g(x) \end{cases}$ is the coordinates of the **intersection points** of the two function graphs.

### 6.5.2 Line with Line

The most common methods for solving systems of two linear equations are **elimination** and **substitution**.

---

**Example 1**: Solve $\begin{cases} 3x + 2y = 7 \\ 5x - 3y = 37 \end{cases}$.

**Solution (Elimination method)**:

Multiply the first equation by $3$ and the second by $2$:

$$
\begin{cases}
9x + 6y = 21 \\
10x - 6y = 74
\end{cases}
$$

Adding: $19x = 95 \Rightarrow x = 5$

Substitute into the first equation: $3(5) + 2y = 7 \Rightarrow 15 + 2y = 7 \Rightarrow 2y = -8 \Rightarrow y = -4$

Therefore the solution is $(x, y) = (5, -4)$.

---

**Example 2**: Solve $\begin{cases} 2x - 5y = 3 \\ 4x + y = 17 \end{cases}$.

**Solution (Substitution method)**:

From the second equation: $y = 17 - 4x$.

Substitute into the first equation:

$$
2x - 5(17 - 4x) = 3
$$

$$
2x - 85 + 20x = 3
$$

$$
22x = 88
$$

$$
x = 4
$$

Substitute back: $y = 17 - 4(4) = 1$

Therefore the solution is $(x, y) = (4, 1)$.

---

**Example 3**: Solve $\begin{cases} \dfrac{x}{2} + \dfrac{y}{3} = 4 \\ \dfrac{x}{4} - \dfrac{y}{2} = 0 \end{cases}$.

**Solution**:

First clear denominators. Multiply the first equation by $6$ and the second by $4$:

$$
\begin{cases}
3x + 2y = 24 \\
x - 2y = 0
\end{cases}
$$

Adding the two equations: $4x = 24 \Rightarrow x = 6$

Substitute into $x - 2y = 0 \Rightarrow 6 - 2y = 0 \Rightarrow y = 3$

Therefore the solution is $(x, y) = (6, 3)$.

---

### 6.5.3 Line with Curve

The general method is **substitution**: solve for one variable from the linear equation and substitute into the quadratic equation, obtaining a quadratic equation in one variable. The discriminant $\Delta$ determines the number of intersection points:

- $\Delta > 0$: Two distinct intersection points (intersect at two points)
- $\Delta = 0$: One intersection point (tangent)
- $\Delta < 0$: No intersection points (do not meet)

---

**Example 4**: Find the intersection points of the line $y = 2x - 1$ and the curve $y = x^2 - 2x + 2$.

**Solution**:

Set $2x - 1 = x^2 - 2x + 2$:

$$
0 = x^2 - 4x + 3
$$

$$
(x - 1)(x - 3) = 0
$$

$$
x = 1 \quad \text{or} \quad x = 3
$$

Substitute into $y = 2x - 1$:

- $x = 1$: $y = 1$, intersection point $(1, 1)$
- $x = 3$: $y = 5$, intersection point $(3, 5)$

---

**Example 5**: Find the value of $k$ such that the line $y = 3x + k$ is tangent to the curve $y = x^2 - 4x + 7$.

**Solution**:

Set $3x + k = x^2 - 4x + 7$:

$$
0 = x^2 - 7x + 7 - k
$$

Tangency condition: $\Delta = 0$

$$
\Delta = (-7)^2 - 4(1)(7 - k) = 49 - 28 + 4k = 21 + 4k = 0
$$

$$
k = -\frac{21}{4}
$$

When $k = -\frac{21}{4}$, the line is tangent to the curve.

Point of tangency: $x^2 - 7x + 7 - (-\frac{21}{4}) = x^2 - 7x + 7 + \frac{21}{4} = x^2 - 7x + \frac{49}{4} = (x - \frac{7}{2})^2 = 0$

So $x = \frac{7}{2}$, $y = 3(\frac{7}{2}) - \frac{21}{4} = \frac{42}{4} - \frac{21}{4} = \frac{21}{4}$.

The point of tangency is $(\frac{7}{2}, \frac{21}{4})$.

---

**Example 6**: Determine the relative position of the line $y = 2x + 5$ and the circle $x^2 + (y - 1)^2 = 5$.

**Solution**:

Substitute $y = 2x + 5$:

$$
x^2 + (2x + 5 - 1)^2 = 5
$$

$$
x^2 + (2x + 4)^2 = 5
$$

$$
x^2 + 4x^2 + 16x + 16 = 5
$$

$$
5x^2 + 16x + 11 = 0
$$

Discriminant $\Delta = 16^2 - 4(5)(11) = 256 - 220 = 36 > 0$

Therefore the line intersects the circle at two distinct points.

Solve $5x^2 + 16x + 11 = 0$:

$$
x = \frac{-16 \pm \sqrt{36}}{10} = \frac{-16 \pm 6}{10}
$$

$$
x = -1 \quad \text{or} \quad x = -\frac{11}{5}
$$

Corresponding $y = 2(-1) + 5 = 3$ and $y = 2(-\frac{11}{5}) + 5 = -\frac{22}{5} + 5 = \frac{3}{5}$.

The intersection points are $(-1, 3)$ and $(-\frac{11}{5}, \frac{3}{5})$.

---

### 6.5.4 Curve with Curve

When both equations are quadratic (or of higher degree), substituting may yield a higher-degree equation, but it can usually be simplified through factorisation or clever substitution.

---

**Example 7**: Solve $\begin{cases} x^2 + y^2 = 10 \\ y = 3x \end{cases}$.

**Solution**:

Substitute $y = 3x$ into the circle equation:

$$
x^2 + (3x)^2 = 10
$$

$$
x^2 + 9x^2 = 10
$$

$$
10x^2 = 10
$$

$$
x^2 = 1
$$

$$
x = \pm 1
$$

Corresponding $y = 3(\pm 1) = \pm 3$.

Solutions: $(1, 3)$ and $(-1, -3)$.

---

**Example 8**: Solve $\begin{cases} x^2 + y^2 = 41 \\ xy = 20 \end{cases}$.

**Solution**:

From $xy = 20$, $y = \frac{20}{x}$ ($x \neq 0$). Substitute into the first equation:

$$
x^2 + \left(\frac{20}{x}\right)^2 = 41
$$

$$
x^2 + \frac{400}{x^2} = 41
$$

Multiply both sides by $x^2$:

$$
x^4 + 400 = 41x^2
$$

$$
x^4 - 41x^2 + 400 = 0
$$

Let $u = x^2 \ge 0$:

$$
u^2 - 41u + 400 = 0
$$

$$
(u - 16)(u - 25) = 0
$$

$$
u = 16 \quad \text{or} \quad u = 25
$$

$x^2 = 16 \Rightarrow x = \pm 4$, corresponding $y = \frac{20}{\pm 4} = \pm 5$

$x^2 = 25 \Rightarrow x = \pm 5$, corresponding $y = \frac{20}{\pm 5} = \pm 4$

Therefore the solutions are $(4, 5)$, $(-4, -5)$, $(5, 4)$, $(-5, -4)$.

---

**Example 9**: Solve $\begin{cases} y - x + 3 = 0 \\ x^2 - 3xy + y^2 + 19 = 0 \end{cases}$.

**Solution**:

From the first equation: $y = x - 3$.

Substitute into the second equation:

$$
x^2 - 3x(x - 3) + (x - 3)^2 + 19 = 0
$$

$$
x^2 - 3x^2 + 9x + x^2 - 6x + 9 + 19 = 0
$$

$$
-x^2 + 3x + 28 = 0
$$

Multiply by $-1$:

$$
x^2 - 3x - 28 = 0
$$

$$
(x - 7)(x + 4) = 0
$$

$$
x = 7 \quad \text{or} \quad x = -4
$$

Corresponding $y = 7 - 3 = 4$ and $y = -4 - 3 = -7$.

Solutions: $(7, 4)$ and $(-4, -7)$.

---

## Practice Problems

### Group A: Absolute Value Equations

**A1**: Solve $|4x - 3| = 9$.
**A2**: Solve $|5 - 3x| = 7$.
**A3**: Solve $|2x + 1| = x + 5$.
**A4**: Solve $|x - 4| = 2x - 5$.
**A5**: Solve $|3x + 2| = |x - 6|$.
**A6**: Solve $|2x - 5| = |4x + 3|$.
**A7**: Solve $|x^2 - 5x + 6| = 2$.
**A8**: Solve $|x^2 - 2x - 3| = 3$.

---

### Group B: Absolute Value Inequalities

**B1**: Solve $|3x + 1| > 7$.
**B2**: Solve $2|5 - x| \le 8$.
**B3**: Solve $|2x - 3| \le |x + 2|$.
**B4**: Solve $2|x + 1| > |3x - 2|$.
**B5**: Solve $|x + 1| \le 2x + 3$.
**B6**: Solve $|2x - 3| > x + 1$.
**B7**: Solve $|x^2 - 4| \le 5$.
**B8**: Solve $|x^2 - 3x| > 2$.

---

### Group C: Substitution Method

**C1**: Solve $2^{2x} - 6 \cdot 2^x + 8 = 0$.
**C2**: Solve $e^{2x} - 5e^x + 6 = 0$.
**C3**: Solve $5e^x = 8 - 3e^{-x}$.
**C4**: Solve $(\ln x)^2 + \ln x - 6 = 0$.
**C5**: Solve $2(\log_3 x)^2 - 5\log_3 x + 2 = 0$.
**C6**: Solve $x - 6\sqrt{x} + 5 = 0$.
**C7**: Solve $x^{\frac{2}{3}} - 2x^{\frac{1}{3}} - 3 = 0$.
**C8**: Solve $x^2 + \frac{1}{x^2} - 3\left(x + \frac{1}{x}\right) + 2 = 0$.

---

### Group D: Cubic Polynomial Graphs and Inequalities

**D1**: Sketch the graph of $f(x) = (x + 3)(x - 2)(x - 5)$, labelling the axis intercepts.
**D2**: Sketch the graph of $f(x) = (2x + 3)(x - 1)(x - 4)$.
**D3**: Sketch the graph of $y = |(x + 3)(x - 2)(x - 5)|$.
**D4**: Solve $(x + 2)(x - 1)(x - 4) \ge 0$.
**D5**: Solve $(x - 1)(x - 3)(x - 6) < 0$.
**D6**: Given $f(x) = (x + 1)(x - 2)(x - 5)$, solve $f(x) \le 0$.

---

### Group E: Simultaneous Equations

**E1**: Solve $\begin{cases} 2x + 3y = 8 \\ 5x - 2y = 1 \end{cases}$.
**E2**: Solve $\begin{cases} 4x - 3y = 11 \\ 3x + 2y = 21 \end{cases}$.
**E3**: Find the intersection points of the line $y = 3x - 2$ and the parabola $y = x^2$.
**E4**: Find the intersection points of the line $y = 2x + 1$ and the curve $y = x^2 - 3x + 5$.
**E5**: Find the value of $k$ such that the line $y = x + k$ is tangent to the curve $y = x^2 - 5x + 7$.
**E6**: Solve $\begin{cases} x^2 + y^2 = 13 \\ y = 2x - 1 \end{cases}$.
**E7**: Solve $\begin{cases} x^2 + y^2 = 25 \\ xy = 12 \end{cases}$.
**E8**: Solve $\begin{cases} x^2 - 2xy + y^2 = 1 \\ x + y = 3 \end{cases}$.

---

## Answers to Practice Problems

### Group A Answers

**A1**: $|4x - 3| = 9$
$4x - 3 = 9$ or $4x - 3 = -9$
$4x = 12$ or $4x = -6$
$x = 3$ or $x = -\frac{3}{2}$

**A2**: $|5 - 3x| = 7$
$5 - 3x = 7$ or $5 - 3x = -7$
$-3x = 2$ or $-3x = -12$
$x = -\frac{2}{3}$ or $x = 4$

**A3**: $|2x + 1| = x + 5$
Case 1 ($x \ge -\frac{1}{2}$): $2x + 1 = x + 5 \Rightarrow x = 4$ ✓
Case 2 ($x < -\frac{1}{2}$): $-(2x + 1) = x + 5 \Rightarrow -2x - 1 = x + 5 \Rightarrow -3x = 6 \Rightarrow x = -2$ ✓
Solutions: $x = 4$ and $x = -2$

**A4**: $|x - 4| = 2x - 5$
Case 1 ($x \ge 4$): $x - 4 = 2x - 5 \Rightarrow -x = -1 \Rightarrow x = 1$, but $1 \ge 4$ is false ✗
Case 2 ($x < 4$): $-(x - 4) = 2x - 5 \Rightarrow -x + 4 = 2x - 5 \Rightarrow 9 = 3x \Rightarrow x = 3$, $3 < 4$ ✓
Solution: $x = 3$

**A5**: $|3x + 2| = |x - 6|$
$3x + 2 = x - 6$ or $3x + 2 = -(x - 6)$
$2x = -8$ or $3x + 2 = -x + 6$
$x = -4$ or $4x = 4$
$x = -4$ or $x = 1$

**A6**: $|2x - 5| = |4x + 3|$
$2x - 5 = 4x + 3$ or $2x - 5 = -(4x + 3)$
$-2x = 8$ or $2x - 5 = -4x - 3$
$x = -4$ or $6x = 2$
$x = -4$ or $x = \frac{1}{3}$

**A7**: $|x^2 - 5x + 6| = 2$
$x^2 - 5x + 6 = 2$ or $x^2 - 5x + 6 = -2$
$x^2 - 5x + 4 = 0$ or $x^2 - 5x + 8 = 0$
$(x - 1)(x - 4) = 0$, $\Delta = 25 - 32 = -7 < 0$, no solution
$x = 1$ or $x = 4$

**A8**: $|x^2 - 2x - 3| = 3$
$x^2 - 2x - 3 = 3$ or $x^2 - 2x - 3 = -3$
$x^2 - 2x - 6 = 0$ or $x^2 - 2x = 0$
$x = \frac{2 \pm \sqrt{4 + 24}}{2} = 1 \pm \sqrt{7}$ or $x(x - 2) = 0 \Rightarrow x = 0$ or $x = 2$
Solutions: $x = 1 \pm \sqrt{7}, 0, 2$

---

### Group B Answers

**B1**: $|3x + 1| > 7$
$3x + 1 < -7$ or $3x + 1 > 7$
$3x < -8$ or $3x > 6$
$x < -\frac{8}{3}$ or $x > 2$
$x \in (-\infty, -\frac{8}{3}) \cup (2, \infty)$

**B2**: $2|5 - x| \le 8$
$|5 - x| \le 4$
$-4 \le 5 - x \le 4$
Left: $-4 \le 5 - x \Rightarrow x \le 9$
Right: $5 - x \le 4 \Rightarrow -x \le -1 \Rightarrow x \ge 1$
$x \in [1, 9]$

**B3**: $|2x - 3| \le |x + 2|$
$(2x - 3)^2 \le (x + 2)^2$
$4x^2 - 12x + 9 \le x^2 + 4x + 4$
$3x^2 - 16x + 5 \le 0$
$(3x - 1)(x - 5) \le 0$
$x \in [\frac{1}{3}, 5]$

**B4**: $2|x + 1| > |3x - 2|$
$4(x + 1)^2 > (3x - 2)^2$
$4(x^2 + 2x + 1) > 9x^2 - 12x + 4$
$4x^2 + 8x + 4 > 9x^2 - 12x + 4$
$0 > 5x^2 - 20x$
$5x^2 - 20x < 0$
$5x(x - 4) < 0$
$0 < x < 4$
$x \in (0, 4)$

**B5**: $|x + 1| \le 2x + 3$
Case 1 ($x \ge -1$): $x + 1 \le 2x + 3 \Rightarrow -2 \le x$, combined with $x \ge -1$ gives $x \ge -1$
Case 2 ($x < -1$): $-(x + 1) \le 2x + 3 \Rightarrow -x - 1 \le 2x + 3 \Rightarrow -4 \le 3x \Rightarrow x \ge -\frac{4}{3}$
Combined with $x < -1$ gives $-\frac{4}{3} \le x < -1$
Union: $x \ge -\frac{4}{3}$, i.e., $x \in [-\frac{4}{3}, \infty)$

**B6**: $|2x - 3| > x + 1$
Case 1 ($x \ge \frac{3}{2}$): $2x - 3 > x + 1 \Rightarrow x > 4$, combined gives $x > 4$
Case 2 ($x < \frac{3}{2}$): $-(2x - 3) > x + 1 \Rightarrow -2x + 3 > x + 1 \Rightarrow 2 > 3x \Rightarrow x < \frac{2}{3}$, combined gives $x < \frac{2}{3}$
$x \in (-\infty, \frac{2}{3}) \cup (4, \infty)$

**B7**: $|x^2 - 4| \le 5$
$-5 \le x^2 - 4 \le 5$
Left: $x^2 - 4 \ge -5 \Rightarrow x^2 \ge -1$, always true
Right: $x^2 - 4 \le 5 \Rightarrow x^2 \le 9 \Rightarrow -3 \le x \le 3$
$x \in [-3, 3]$

**B8**: $|x^2 - 3x| > 2$
$x^2 - 3x < -2$ or $x^2 - 3x > 2$
Inequality 1: $x^2 - 3x + 2 < 0 \Rightarrow (x - 1)(x - 2) < 0 \Rightarrow 1 < x < 2$
Inequality 2: $x^2 - 3x - 2 > 0$
$x = \frac{3 \pm \sqrt{9 + 8}}{2} = \frac{3 \pm \sqrt{17}}{2}$
$x < \frac{3 - \sqrt{17}}{2}$ or $x > \frac{3 + \sqrt{17}}{2}$
where $\frac{3 - \sqrt{17}}{2} \approx -0.562$, $\frac{3 + \sqrt{17}}{2} \approx 3.562$
Solution set: $x \in (-\infty, \frac{3 - \sqrt{17}}{2}) \cup (1, 2) \cup (\frac{3 + \sqrt{17}}{2}, \infty)$

---

### Group C Answers

**C1**: $2^{2x} - 6 \cdot 2^x + 8 = 0$
Let $u = 2^x > 0$: $u^2 - 6u + 8 = 0 \Rightarrow (u - 2)(u - 4) = 0$
$u = 2$ or $u = 4$
$2^x = 2 \Rightarrow x = 1$; $2^x = 4 \Rightarrow x = 2$

**C2**: $e^{2x} - 5e^x + 6 = 0$
Let $u = e^x > 0$: $u^2 - 5u + 6 = 0 \Rightarrow (u - 2)(u - 3) = 0$
$u = 2$ or $u = 3$
$e^x = 2 \Rightarrow x = \ln 2$; $e^x = 3 \Rightarrow x = \ln 3$

**C3**: $5e^x = 8 - 3e^{-x}$
Multiply by $e^x$: $5e^{2x} = 8e^x - 3$
$5e^{2x} - 8e^x + 3 = 0$
Let $u = e^x > 0$: $5u^2 - 8u + 3 = 0 \Rightarrow (5u - 3)(u - 1) = 0$
$u = \frac{3}{5}$ or $u = 1$
$e^x = \frac{3}{5} \Rightarrow x = \ln \frac{3}{5}$; $e^x = 1 \Rightarrow x = 0$

**C4**: $(\ln x)^2 + \ln x - 6 = 0$
Let $u = \ln x$: $u^2 + u - 6 = 0 \Rightarrow (u + 3)(u - 2) = 0$
$u = -3$ or $u = 2$
$\ln x = -3 \Rightarrow x = e^{-3}$; $\ln x = 2 \Rightarrow x = e^2$

**C5**: $2(\log_3 x)^2 - 5\log_3 x + 2 = 0$
Let $u = \log_3 x$: $2u^2 - 5u + 2 = 0 \Rightarrow (2u - 1)(u - 2) = 0$
$u = \frac{1}{2}$ or $u = 2$
$\log_3 x = \frac{1}{2} \Rightarrow x = 3^{1/2} = \sqrt{3}$; $\log_3 x = 2 \Rightarrow x = 3^2 = 9$

**C6**: $x - 6\sqrt{x} + 5 = 0$
Let $u = \sqrt{x} \ge 0$: $u^2 - 6u + 5 = 0 \Rightarrow (u - 1)(u - 5) = 0$
$u = 1$ or $u = 5$
$\sqrt{x} = 1 \Rightarrow x = 1$; $\sqrt{x} = 5 \Rightarrow x = 25$

**C7**: $x^{\frac{2}{3}} - 2x^{\frac{1}{3}} - 3 = 0$
Let $u = x^{\frac{1}{3}}$: $u^2 - 2u - 3 = 0 \Rightarrow (u - 3)(u + 1) = 0$
$u = 3$ or $u = -1$
$x^{\frac{1}{3}} = 3 \Rightarrow x = 27$; $x^{\frac{1}{3}} = -1 \Rightarrow x = -1$

**C8**: $x^2 + \frac{1}{x^2} - 3\left(x + \frac{1}{x}\right) + 2 = 0$
Let $u = x + \frac{1}{x}$, then $u^2 = x^2 + 2 + \frac{1}{x^2} \Rightarrow x^2 + \frac{1}{x^2} = u^2 - 2$
$(u^2 - 2) - 3u + 2 = 0 \Rightarrow u^2 - 3u = 0 \Rightarrow u(u - 3) = 0$
$u = 0$ or $u = 3$
$u = 0$: $x + \frac{1}{x} = 0 \Rightarrow x^2 + 1 = 0$, no real solution
$u = 3$: $x + \frac{1}{x} = 3 \Rightarrow x^2 - 3x + 1 = 0 \Rightarrow x = \frac{3 \pm \sqrt{5}}{2}$

---

### Group D Answers

**D1**: $f(x) = (x + 3)(x - 2)(x - 5)$
$x$-intercepts: $-3, 2, 5$
$y$-intercept: $f(0) = 3 \times (-2) \times (-5) = 30$, point $(0, 30)$
Leading coefficient positive. As $x \to -\infty$, $f(x) \to -\infty$; as $x \to \infty$, $f(x) \to \infty$
Sign: $(-\infty, -3)$: −; $(-3, 2)$: +; $(2, 5)$: −; $(5, \infty)$: +

**D2**: $f(x) = (2x + 3)(x - 1)(x - 4)$
$x$-intercepts: $-\frac{3}{2}, 1, 4$
$y$-intercept: $f(0) = 3 \times (-1) \times (-4) = 12$, point $(0, 12)$
Leading coefficient $2 > 0$, end behaviour same as D1.
Sign: $(-\infty, -\frac{3}{2})$: −; $(-\frac{3}{2}, 1)$: +; $(1, 4)$: −; $(4, \infty)$: +

**D3**: $y = |(x + 3)(x - 2)(x - 5)|$
Reflect the negative parts of $f(x)$ on $(-\infty, -3)$ and $(2, 5)$ upward. $x$-intercepts remain at $-3, 2, 5$. $y$-intercept is $|30| = 30$. The entire graph lies above (or on) the $x$-axis.

**D4**: $(x + 2)(x - 1)(x - 4) \ge 0$
Roots: $-2, 1, 4$, leading coefficient positive.
Sign: $(-\infty, -2)$: −; $(-2, 1)$: +; $(1, 4)$: −; $(4, \infty)$: +
Solution: $x \in [-2, 1] \cup [4, \infty)$

**D5**: $(x - 1)(x - 3)(x - 6) < 0$
Roots: $1, 3, 6$, leading coefficient positive.
Sign: $(-\infty, 1)$: −; $(1, 3)$: +; $(3, 6)$: −; $(6, \infty)$: +
Solution: $x \in (-\infty, 1) \cup (3, 6)$

**D6**: $f(x) = (x + 1)(x - 2)(x - 5) \le 0$
Roots: $-1, 2, 5$, leading coefficient positive.
Sign: $(-\infty, -1)$: −; $(-1, 2)$: +; $(2, 5)$: −; $(5, \infty)$: +
Solution: $x \in (-\infty, -1] \cup [2, 5]$

---

### Group E Answers

**E1**: $\begin{cases} 2x + 3y = 8 \\ 5x - 2y = 1 \end{cases}$
Multiply the first by $2$, the second by $3$: $\begin{cases} 4x + 6y = 16 \\ 15x - 6y = 3 \end{cases}$
Adding: $19x = 19 \Rightarrow x = 1$
Substitute: $2(1) + 3y = 8 \Rightarrow 3y = 6 \Rightarrow y = 2$
Solution: $(1, 2)$

**E2**: $\begin{cases} 4x - 3y = 11 \\ 3x + 2y = 21 \end{cases}$
Multiply the first by $2$, the second by $3$: $\begin{cases} 8x - 6y = 22 \\ 9x + 6y = 63 \end{cases}$
Adding: $17x = 85 \Rightarrow x = 5$
Substitute: $4(5) - 3y = 11 \Rightarrow 20 - 3y = 11 \Rightarrow 3y = 9 \Rightarrow y = 3$
Solution: $(5, 3)$

**E3**: $y = 3x - 2$ and $y = x^2$
$x^2 = 3x - 2 \Rightarrow x^2 - 3x + 2 = 0 \Rightarrow (x - 1)(x - 2) = 0$
$x = 1$ or $x = 2$
Intersection points: $(1, 1)$ and $(2, 4)$

**E4**: $y = 2x + 1$ and $y = x^2 - 3x + 5$
$2x + 1 = x^2 - 3x + 5 \Rightarrow 0 = x^2 - 5x + 4 \Rightarrow (x - 1)(x - 4) = 0$
$x = 1$ or $x = 4$
Intersection points: $(1, 3)$ and $(4, 9)$

**E5**: $y = x + k$ tangent to $y = x^2 - 5x + 7$
$x + k = x^2 - 5x + 7 \Rightarrow 0 = x^2 - 6x + 7 - k$
$\Delta = (-6)^2 - 4(1)(7 - k) = 36 - 28 + 4k = 8 + 4k = 0$
$k = -2$

**E6**: $\begin{cases} x^2 + y^2 = 13 \\ y = 2x - 1 \end{cases}$
Substitute: $x^2 + (2x - 1)^2 = 13 \Rightarrow x^2 + 4x^2 - 4x + 1 = 13 \Rightarrow 5x^2 - 4x - 12 = 0$
$(5x + 6)(x - 2) = 0 \Rightarrow x = -\frac{6}{5}$ or $x = 2$
$y = 2(-\frac{6}{5}) - 1 = -\frac{12}{5} - 1 = -\frac{17}{5}$; $y = 2(2) - 1 = 3$
Solutions: $(-\frac{6}{5}, -\frac{17}{5})$ and $(2, 3)$

**E7**: $\begin{cases} x^2 + y^2 = 25 \\ xy = 12 \end{cases}$
From $xy = 12$, $y = \frac{12}{x}$ ($x \neq 0$)
Substitute: $x^2 + \frac{144}{x^2} = 25 \Rightarrow x^4 - 25x^2 + 144 = 0$
Let $u = x^2 \ge 0$: $u^2 - 25u + 144 = 0 \Rightarrow (u - 9)(u - 16) = 0$
$u = 9 \Rightarrow x = \pm 3$, $y = \frac{12}{\pm 3} = \pm 4$
$u = 16 \Rightarrow x = \pm 4$, $y = \frac{12}{\pm 4} = \pm 3$
Solutions: $(3, 4)$, $(-3, -4)$, $(4, 3)$, $(-4, -3)$

**E8**: $\begin{cases} x^2 - 2xy + y^2 = 1 \\ x + y = 3 \end{cases}$
Note $x^2 - 2xy + y^2 = (x - y)^2 = 1$, so $x - y = \pm 1$
Together with $x + y = 3$:
When $x - y = 1$: $\begin{cases} x + y = 3 \\ x - y = 1 \end{cases} \Rightarrow x = 2, y = 1$
When $x - y = -1$: $\begin{cases} x + y = 3 \\ x - y = -1 \end{cases} \Rightarrow x = 1, y = 2$
Solutions: $(2, 1)$ and $(1, 2)$

---

## Chapter Summary

| Topic | Core Method | Key Points |
|--------|---------|---------|
| **Sets and intervals** | Set-builder notation, interval notation | Open intervals use round brackets, closed use square brackets; $\cup$ denotes union |
| **6.1 Absolute value equations** | Case analysis or squaring both sides | $|A| = B$ requires $B \ge 0$; $|A| = |B| \iff A = \pm B$ |
| **6.2 Absolute value inequalities** | Transform into inequality systems or square | $|A| > c \iff A < -c$ or $A > c$; $|A| \le c \iff -c \le A \le c$ |
| **6.3 Substitution method** | Identify repeated structure, let $u = g(x)$ | Check existence and domain after back-substitution (e.g., $u \ge 0$, $u \neq 0$) |
| **6.4 Cubic polynomial graphs and inequalities** | Find three $x$-intercepts, sign analysis | Leading coefficient determines end behaviour; absolute value graphs reflect negative parts upward |
| **6.5 Simultaneous equations** | Substitution + discriminant | $\Delta > 0$ two intersections, $\Delta = 0$ tangent, $\Delta < 0$ no intersection |

---
---







# Chapter 7: Integration (Indefinite and Definite Integrals) [Revised and Expanded Edition]

---

## Syllabus Mapping

This chapter corresponds to the following entries from **Topic 14: Calculus** of the **Cambridge IGCSE Additional Mathematics (0606) 2028–2030 syllabus**:

| Syllabus Ref | Content | Notes |
|---------|---------|---------|
| **14.10** | Understand integration as the reverse process of differentiation | Indefinite integrals must include an arbitrary constant |
| **14.11** | Integrate sums of terms in powers of $x$ | Includes $x^n$, $\dfrac{1}{x}$, $\dfrac{1}{ax+b}$ |
| **14.12** | Integrate functions of the form | $(ax+b)^n$ (any rational $n$, including $n=-1$), $\sin(ax+b)$, $\cos(ax+b)$, $\sec^2(ax+b)$, $e^{ax+b}$ |
| **14.13** | Evaluation of definite integrals and application to plane area | Between a line and a curve, between two curves, sum of two or more areas |
| **14.14** | Application of differentiation and integration to kinematics | Relationships between displacement, velocity and acceleration (see Chapter 10) |

> ⚠️ **Important**: The syllabus explicitly states that **no formulas will be given** in the List of formulas for the Calculus section. All integration formulas must be **memorised thoroughly**. Angles in trigonometric functions must always be in **radians**.

---

## Introduction

In Chapter 5, we learned **differentiation** — given a function $f(x)$, find its rate of change $f'(x)$. Differentiation answers the question "how fast is it changing?" **Integration** is the **reverse operation** of this process: given the derivative $f'(x)$, we want to recover the original function $f(x)$. Therefore, integration is also called **antidifferentiation**.

But the significance of integration goes far beyond being just a reverse operation. From a broader perspective:

- **Geometric meaning**: Definite integrals calculate the **area** under a curve. This is the core problem that took nearly two thousand years to solve — from Archimedes' "method of exhaustion" in ancient Greece to the independent development of calculus by Newton and Leibniz in the 17th century.
- **Physical meaning**: Given velocity, find displacement; given acceleration, find velocity — these are all processes of **accumulation**. In everyday life, the odometer reading is the accumulation of speed over time.
- **Analogy**: If differentiation is like taking a photograph (capturing the change at an instant), then integration is like recording a video (accumulating the change frame by frame).

**Comparison between integration and differentiation**:

| Concept | Differentiation (Chapter 5) | Integration (Chapter 7) |
|------|----------------|----------------|
| Basic question | Given $f(x)$, find $f'(x)$ | Given $f'(x)$, find $f(x)$ |
| Geometric meaning | Find slope of tangent at a point | Find area under a curve |
| Physical meaning | Given displacement, find velocity/acceleration | Given acceleration, find velocity/displacement |
| Notation | $\dfrac{d}{dx}$ | $\displaystyle \int \cdots dx$ |
| Operation properties | Linearity, product rule, quotient rule, chain rule | Linearity (no simple product/quotient rule counterpart) |

> **Core idea**: Differentiation and integration are inverse operations. Just like addition and subtraction, multiplication and division, they are a pair of "reverse operations." Understanding this inverse relationship is the cornerstone of all of calculus.

---

## 7.1 Indefinite Integrals (Antiderivatives)

### 7.1.1 From Differentiation to Integration — The Essence of the Inverse Operation

We start with the most fundamental question.

**Question**: Given that the derivative of a function $F(x)$ is $2x$, i.e., $F'(x) = 2x$, find $F(x)$.

**Thinking process**: In Chapter 5 we learned:

$$
\frac{d}{dx}(x^2) = 2x
$$

So $x^2$ is an "antiderivative" of $2x$. But the problem is — the derivative of a constant is $0$, so $x^2 + 1$, $x^2 - 5$, $x^2 + \pi$ all have derivatives equal to $2x$. This means $2x$ has **infinitely many** antiderivatives, differing only by a constant. We denote this arbitrary constant by $C$.

Using integration notation for this process:

$$
\boxed{\int 2x \, dx = x^2 + C}
$$

Where:
- $\int$ is called the **integral sign** (an elongated S, from the Latin *summa*, meaning "sum")
- $2x$ is called the **integrand**
- $dx$ indicates integration with respect to the variable $x$
- $C$ is called the **constant of integration**

> **Formal definition**: A function $F(x)$ is called an **antiderivative** of $f(x)$ if $F'(x) = f(x)$ for all $x$ in the domain. The set of all antiderivatives of $f(x)$ is called the **indefinite integral**, denoted by $\displaystyle \int f(x) \, dx = F(x) + C$.

### 7.1.2 The Inverse Relationship Between Integration and Differentiation — Verification

Since integration is the inverse of differentiation, every integration formula can be verified by differentiation. This is the most reliable way to check whether an integration result is correct.

**Verification procedure**:
1. Differentiate the result $F(x) + C$
2. Check whether the derivative equals the integrand $f(x)$
3. If they are equal, the integration is correct

**Verification example 1**: Verify $\displaystyle \int 3x^2 \, dx = x^3 + C$

$$
\frac{d}{dx}(x^3 + C) = 3x^2 \quad \checkmark
$$

**Verification example 2**: Verify $\displaystyle \int \cos x \, dx = \sin x + C$

$$
\frac{d}{dx}(\sin x + C) = \cos x \quad \checkmark
$$

**Verification example 3**: Verify $\displaystyle \int e^{2x} \, dx = \frac{1}{2}e^{2x} + C$

$$
\frac{d}{dx}\left(\frac{1}{2}e^{2x} + C\right) = \frac{1}{2} \cdot e^{2x} \cdot 2 = e^{2x} \quad \checkmark
$$

This seemingly simple method is especially important when dealing with complex integrals — if you are unsure about a result, **verifying by differentiation** is always the most reliable check.

---

**Example 1** (Understanding the concept of antiderivatives): Given $f'(x) = 6x^2$ and $f(1) = 3$, find $f(x)$.

**Solution**:

First find the indefinite integral:

$$
f(x) = \int 6x^2 \, dx = 6 \cdot \frac{x^3}{3} + C = 2x^3 + C
$$

Use the condition $f(1) = 3$ to determine $C$:

$$
f(1) = 2(1)^3 + C = 2 + C = 3 \Rightarrow C = 1
$$

Therefore $f(x) = 2x^3 + 1$.

> This is a common question type in exams — given the derivative and an initial condition, find the original function. The key is to first integrate to obtain an expression containing $C$, then substitute the condition to solve for $C$.

---

**Example 2** (Verifying integration by differentiation): Determine whether $\displaystyle \int \frac{1}{x^2} \, dx = -\frac{1}{x} + C$ is correct.

**Solution**:

Differentiate the result:

$$
\frac{d}{dx}\left(-\frac{1}{x} + C\right) = \frac{d}{dx}(-x^{-1} + C) = x^{-2} = \frac{1}{x^2}
$$

The derivative equals the integrand, so the integration is correct.

---

**Example 3** (Finding errors through differentiation): Determine whether $\displaystyle \int (2x+1)^2 \, dx = \frac{(2x+1)^3}{3} + C$ is correct.

**Solution**:

Differentiate the result:

$$
\frac{d}{dx}\left(\frac{(2x+1)^3}{3} + C\right) = \frac{1}{3} \cdot 3(2x+1)^2 \cdot 2 = 2(2x+1)^2 \neq (2x+1)^2
$$

There is an extra factor of $2$, so the integration is **incorrect**! The correct approach is:

$$
\int (2x+1)^2 \, dx = \frac{(2x+1)^3}{2 \cdot 3} + C = \frac{(2x+1)^3}{6} + C
$$

Verification: $\dfrac{d}{dx}\left(\dfrac{(2x+1)^3}{6}\right) = \dfrac{3(2x+1)^2 \cdot 2}{6} = (2x+1)^2 \quad \checkmark$

> ⚠️ **Lesson**: For integrals of the form $(ax+b)^n$, don't forget the extra factor $\dfrac{1}{a}$! This is one of the most common mistakes made by beginners.

---

### 7.1.3 Linearity of Integration

Integration satisfies **linearity**. This property derives from the linearity of differentiation and is the most fundamental rule in integration:

$$
\boxed{\int [a f(x) + b g(x)] \, dx = a \int f(x) \, dx + b \int g(x) \, dx}
$$

where $a$ and $b$ are arbitrary constants.

**Derivation**: Let $F'(x) = f(x)$, $G'(x) = g(x)$. Then by the linearity of differentiation:

$$
\frac{d}{dx}[a F(x) + b G(x)] = a F'(x) + b G'(x) = a f(x) + b g(x)
$$

Therefore $a F(x) + b G(x)$ is an antiderivative of $a f(x) + b g(x)$, proving the equality.

This property tells us two things:
1. **A constant factor can be pulled outside the integral sign**: $\displaystyle \int c f(x) \, dx = c \int f(x) \, dx$
2. **The integral of a sum equals the sum of the integrals**: $\displaystyle \int [f(x) + g(x)] \, dx = \int f(x) \, dx + \int g(x) \, dx$

> ⚠️ **Important warning**: The linearity of integration **does not mean** that "the integral of a product equals the product of the integrals"!
>
> $$
> \int f(x)g(x) \, dx \neq \int f(x) \, dx \cdot \int g(x) \, dx
> $$
>
> Nor does it mean "the integral of a quotient equals the quotient of the integrals"!
>
> $$
> \int \frac{f(x)}{g(x)} \, dx \neq \frac{\int f(x) \, dx}{\int g(x) \, dx}
> $$
>
> Integrating products and quotients requires more advanced techniques (such as integration by parts), which are not in the IGCSE syllabus. In IGCSE 0606, when encountering a product, you must **expand** first and then integrate term by term.

---

**Example 1** (Basic application of linearity): Find $\displaystyle \int (3x^2 - 5x + 2) \, dx$.

**Solution**:

$$
\begin{aligned}
\int (3x^2 - 5x + 2) \, dx &= 3 \int x^2 \, dx - 5 \int x \, dx + 2 \int 1 \, dx \\[4pt]
&= 3 \cdot \frac{x^3}{3} - 5 \cdot \frac{x^2}{2} + 2x + C \\[4pt]
&= x^3 - \frac{5}{2}x^2 + 2x + C
\end{aligned}
$$

**Verification**: $\dfrac{d}{dx}\left(x^3 - \dfrac{5}{2}x^2 + 2x + C\right) = 3x^2 - 5x + 2$. ✓

---

**Example 2** (Expand first, then integrate — handling products): Find $\displaystyle \int (x+3)(x-2) \, dx$.

**Solution**:

First expand:

$$
(x+3)(x-2) = x^2 - 2x + 3x - 6 = x^2 + x - 6
$$

Then integrate term by term:

$$
\int (x^2 + x - 6) \, dx = \frac{x^3}{3} + \frac{x^2}{2} - 6x + C
$$

> ⚠️ **Cannot** write: $\int (x+3)(x-2) \, dx = \int (x+3) \, dx \cdot \int (x-2) \, dx$

---

**Example 3** (Expanding a polynomial then integrating): Find $\displaystyle \int (2x-1)^3 \, dx$.

**Solution**:

Method 1 (Expand):

$$
(2x-1)^3 = 8x^3 - 12x^2 + 6x - 1
$$

$$
\begin{aligned}
\int (8x^3 - 12x^2 + 6x - 1) \, dx &= 8 \cdot \frac{x^4}{4} - 12 \cdot \frac{x^3}{3} + 6 \cdot \frac{x^2}{2} - x + C \\[4pt]
&= 2x^4 - 4x^3 + 3x^2 - x + C
\end{aligned}
$$

Method 2 (Using the $(ax+b)^n$ formula directly, which will be learned in §7.2.3):

$$
\int (2x-1)^3 \, dx = \frac{(2x-1)^4}{2 \cdot 4} + C = \frac{(2x-1)^4}{8} + C
$$

The two methods give answers that look different in form but are actually equivalent (expanding both gives the same result). ✓

---

**Example 4** (Simplify a fraction before integrating): Find $\displaystyle \int \frac{x^3 + 3x^2 - 2}{x^2} \, dx$.

**Solution**:

First simplify: $\dfrac{x^3 + 3x^2 - 2}{x^2} = x + 3 - \dfrac{2}{x^2} = x + 3 - 2x^{-2}$

Then integrate term by term:

$$
\begin{aligned}
\int (x + 3 - 2x^{-2}) \, dx &= \frac{x^2}{2} + 3x - 2 \cdot \frac{x^{-1}}{-1} + C \\[4pt]
&= \frac{x^2}{2} + 3x + \frac{2}{x} + C
\end{aligned}
$$

> ⚠️ **Common mistake**: Do not try to integrate the fraction as a whole! You must first separate the fraction into a sum of individual terms before integrating term by term.

---

## 7.2 Basic Integration Formulas (Complete Derivations with Many Examples)

This section is **the most core content of this chapter**. All formulas must be memorised thoroughly, as the examination **does not provide a formula sheet**. For each formula, I will provide:
1. The formula itself
2. Derivation starting from differentiation
3. At least 3 worked examples (from basic to comprehensive)

---

### 7.2.1 Power Rule for Integration: $\displaystyle \int x^n \, dx \quad (n \neq -1)$

**Formula**:

$$
\boxed{\int x^n \, dx = \frac{x^{n+1}}{n+1} + C \quad (n \neq -1)}
$$

**Derivation**: Differentiate the right-hand side:

$$
\frac{d}{dx}\left(\frac{x^{n+1}}{n+1} + C\right) = \frac{n+1}{n+1} x^{n} = x^n
$$

The derivative equals the integrand $x^n$, proving the formula.

**Key points to understand**:
- **Add 1 to the exponent**: $n \to n+1$
- **Divide by the new exponent**: divide by $(n+1)$
- This formula holds for **all rational numbers** $n \neq -1$, including negative numbers and fractions

**Quick reference table for common exponent forms**:

| Integrand | Rewritten as power | Integration result |
|---------|-------------|---------|
| $x^5$ | $x^5$ | $\dfrac{x^6}{6}$ |
| $\dfrac{1}{x^3}$ | $x^{-3}$ | $\dfrac{x^{-2}}{-2} = -\dfrac{1}{2x^2}$ |
| $\sqrt{x}$ | $x^{1/2}$ | $\dfrac{x^{3/2}}{3/2} = \dfrac{2}{3}x^{3/2}$ |
| $\dfrac{1}{\sqrt{x}}$ | $x^{-1/2}$ | $\dfrac{x^{1/2}}{1/2} = 2\sqrt{x}$ |
| $\sqrt[3]{x^2}$ | $x^{2/3}$ | $\dfrac{x^{5/3}}{5/3} = \dfrac{3}{5}x^{5/3}$ |

---

**Example 1** (Positive integer exponent): Find $\displaystyle \int x^8 \, dx$.

**Solution**:

$$
\int x^8 \, dx = \frac{x^{8+1}}{8+1} + C = \frac{x^9}{9} + C
$$

**Verification**: $\dfrac{d}{dx}\left(\dfrac{x^9}{9}\right) = \dfrac{9x^8}{9} = x^8$. ✓

---

**Example 2** (Negative exponent): Find $\displaystyle \int \frac{1}{x^4} \, dx$.

**Solution**:

First rewrite: $\dfrac{1}{x^4} = x^{-4}$

$$
\int x^{-4} \, dx = \frac{x^{-4+1}}{-4+1} + C = \frac{x^{-3}}{-3} + C = -\frac{1}{3x^3} + C
$$

**Verification**: $\dfrac{d}{dx}\left(-\dfrac{1}{3}x^{-3}\right) = -\dfrac{1}{3} \cdot (-3)x^{-4} = x^{-4}$. ✓

> ⚠️ **Common mistake**: When $n = -4$, $n+1 = -3$ (not $-5$!). Many students mistakenly think that adding 1 makes the exponent more negative, but in fact $-4+1 = -3$. Always writing out the intermediate steps can help avoid this type of error.

---

**Example 3** (Fractional exponent — square root): Find $\displaystyle \int \sqrt{x} \, dx$.

**Solution**:

$\sqrt{x} = x^{1/2}$

$$
\int x^{1/2} \, dx = \frac{x^{1/2+1}}{1/2+1} + C = \frac{x^{3/2}}{3/2} + C = \frac{2}{3}x^{3/2} + C
$$

This can also be written as $\dfrac{2}{3}\sqrt{x^3} + C$ or $\dfrac{2}{3}x\sqrt{x} + C$.

**Verification**: $\dfrac{d}{dx}\left(\dfrac{2}{3}x^{3/2}\right) = \dfrac{2}{3} \cdot \dfrac{3}{2}x^{1/2} = x^{1/2} = \sqrt{x}$. ✓

---

**Example 4** (Fractional exponent — cube root): Find $\displaystyle \int \sqrt[3]{x} \, dx$.

**Solution**:

$\sqrt[3]{x} = x^{1/3}$

$$
\int x^{1/3} \, dx = \frac{x^{1/3+1}}{1/3+1} + C = \frac{x^{4/3}}{4/3} + C = \frac{3}{4}x^{4/3} + C
$$

---

**Example 5** (Negative fractional exponent): Find $\displaystyle \int \frac{1}{\sqrt[3]{x^2}} \, dx$.

**Solution**:

$\dfrac{1}{\sqrt[3]{x^2}} = \dfrac{1}{x^{2/3}} = x^{-2/3}$

$$
\int x^{-2/3} \, dx = \frac{x^{-2/3+1}}{-2/3+1} + C = \frac{x^{1/3}}{1/3} + C = 3x^{1/3} + C = 3\sqrt[3]{x} + C
$$

**Verification**: $\dfrac{d}{dx}(3x^{1/3}) = 3 \cdot \dfrac{1}{3}x^{-2/3} = x^{-2/3} = \dfrac{1}{\sqrt[3]{x^2}}$. ✓

---

**Example 6** (Comprehensive — mixed terms): Find $\displaystyle \int \left( 4x^3 + \frac{2}{x^5} - 3\sqrt{x} + \frac{1}{\sqrt{x}} \right) dx$.

**Solution**:

First rewrite each term in power form:

$$
4x^3 + 2x^{-5} - 3x^{1/2} + x^{-1/2}
$$

Integrate term by term:

$$
\begin{aligned}
\int 4x^3 \, dx &= 4 \cdot \frac{x^4}{4} = x^4 \\[4pt]
\int 2x^{-5} \, dx &= 2 \cdot \frac{x^{-4}}{-4} = -\frac{1}{2}x^{-4} = -\frac{1}{2x^4} \\[4pt]
\int -3x^{1/2} \, dx &= -3 \cdot \frac{x^{3/2}}{3/2} = -3 \cdot \frac{2}{3}x^{3/2} = -2x^{3/2} \\[4pt]
\int x^{-1/2} \, dx &= \frac{x^{1/2}}{1/2} = 2x^{1/2} = 2\sqrt{x}
\end{aligned}
$$

Combine the results:

$$
\int \left( 4x^3 + \frac{2}{x^5} - 3\sqrt{x} + \frac{1}{\sqrt{x}} \right) dx = x^4 - \frac{1}{2x^4} - 2x^{3/2} + 2\sqrt{x} + C
$$

---

### 7.2.2 Special Case: $\displaystyle \int \frac{1}{x} \, dx$

**Formula**:

$$
\boxed{\int \frac{1}{x} \, dx = \ln |x| + C}
$$

**Why is $n=-1$ a special case?**

Recall the power rule: $\displaystyle \int x^n \, dx = \frac{x^{n+1}}{n+1} + C$. If $n = -1$, then $n+1 = 0$, making the denominator zero — the formula breaks down! Therefore the integral of $\dfrac{1}{x}$ needs to be handled separately.

**Derivation**: Recall the derivative of $\ln x$.

When $x > 0$:

$$
\frac{d}{dx}(\ln x) = \frac{1}{x}
$$

When $x < 0$, $|x| = -x > 0$, by the chain rule:

$$
\frac{d}{dx}[\ln (-x)] = \frac{1}{-x} \cdot (-1) = \frac{1}{x}
$$

Both cases can be uniformly written as $\dfrac{d}{dx}(\ln |x|) = \dfrac{1}{x}$, therefore $\displaystyle \int \frac{1}{x} \, dx = \ln |x| + C$.

> ⚠️ **The absolute value sign cannot be omitted!** It ensures the formula still holds when $x$ is negative.

**Comparison with the Power Rule**:

$$
\int x^2 \, dx = \frac{x^3}{3} + C, \quad \int x^1 \, dx = \frac{x^2}{2} + C, \quad \int x^0 \, dx = x + C, \quad \int x^{-1} \, dx = \ln|x| + C
$$

Note that $x^0 = 1$, whose integral is $x$, not $\ln|x|$ — only $x^{-1}$ gives $\ln|x|$.

---

**Example 1** (Basic form): Find $\displaystyle \int \frac{5}{x} \, dx$.

**Solution**:

$$
\int \frac{5}{x} \, dx = 5 \int \frac{1}{x} \, dx = 5\ln |x| + C
$$

---

**Example 2** (Mixed with power functions): Find $\displaystyle \int \left( x^3 - \frac{2}{x} \right) dx$.

**Solution**:

$$
\int \left( x^3 - \frac{2}{x} \right) dx = \frac{x^4}{4} - 2\ln|x| + C
$$

---

**Example 3** (Simplify before integrating — common exam type): Find $\displaystyle \int \frac{x^2 + 3x - 1}{x} \, dx$.

**Solution**:

First simplify:

$$
\frac{x^2 + 3x - 1}{x} = x + 3 - \frac{1}{x}
$$

Then integrate:

$$
\int \left( x + 3 - \frac{1}{x} \right) dx = \frac{x^2}{2} + 3x - \ln|x| + C
$$

> ⚠️ **Common mistake**: Some students try to apply the power rule directly to $\dfrac{x^2+3x-1}{x}$ as a whole — this is not allowed! You must first simplify it into a sum of individual terms.

---

**Example 4** (Carefully distinguish $\dfrac{1}{x}$ from $x^{-2}$): Find $\displaystyle \int \frac{x^3 - 2x^2 + 1}{x^2} \, dx$.

**Solution**:

Simplify:

$$
\frac{x^3 - 2x^2 + 1}{x^2} = x - 2 + \frac{1}{x^2} = x - 2 + x^{-2}
$$

Integrate:

$$
\int (x - 2 + x^{-2}) \, dx = \frac{x^2}{2} - 2x + \frac{x^{-1}}{-1} + C = \frac{x^2}{2} - 2x - \frac{1}{x} + C
$$

Notice that here $x^{-2}$ uses the power rule ($n=-2 \neq -1$), and only $\dfrac{1}{x} = x^{-1}$ uses $\ln|x|$. Do not confuse the two!

---

### 7.2.3 Integrating Linear Composite Forms: $\displaystyle \int (ax+b)^n \, dx$

**Formula** ($n \neq -1$):

$$
\boxed{\int (ax+b)^n \, dx = \frac{(ax+b)^{n+1}}{a(n+1)} + C \quad (n \neq -1)}
$$

When $n = -1$:

$$
\boxed{\int \frac{1}{ax+b} \, dx = \frac{1}{a} \ln |ax+b| + C}
$$

**Derivation** (using substitution thinking):

Let $u = ax+b$, then $du = a \, dx$, i.e., $dx = \dfrac{du}{a}$.

$$
\int (ax+b)^n \, dx = \int u^n \cdot \frac{du}{a} = \frac{1}{a} \int u^n \, du = \frac{1}{a} \cdot \frac{u^{n+1}}{n+1} + C = \frac{(ax+b)^{n+1}}{a(n+1)} + C
$$

**Intuitive understanding**: Compare with $\int x^n \, dx = \dfrac{x^{n+1}}{n+1}$. Here $x$ is replaced by $(ax+b)$, but an extra factor of $\dfrac{1}{a}$ appears. This $\dfrac{1}{a}$ comes from the reverse of the chain rule — because the derivative of $(ax+b)$ is $a$, so in the reverse operation we must divide by $a$.

**Memory aid**: "Add 1 to the exponent, divide by the new exponent, then divide by $a$."

---

**Example 1** (Positive integer $n$): Find $\displaystyle \int (5x+2)^3 \, dx$.

**Solution**:

Here $a=5$, $n=3$.

$$
\int (5x+2)^3 \, dx = \frac{(5x+2)^{4}}{5 \cdot 4} + C = \frac{(5x+2)^4}{20} + C
$$

**Verification**: $\dfrac{d}{dx}\left[\dfrac{(5x+2)^4}{20}\right] = \dfrac{4(5x+2)^3 \cdot 5}{20} = \dfrac{20(5x+2)^3}{20} = (5x+2)^3$. ✓

---

**Example 2** (Negative integer $n$): Find $\displaystyle \int \frac{1}{(3x-1)^4} \, dx$.

**Solution**:

Rewrite as $(3x-1)^{-4}$, $a=3$, $n=-4$.

$$
\int (3x-1)^{-4} \, dx = \frac{(3x-1)^{-3}}{3 \cdot (-3)} + C = -\frac{1}{9}(3x-1)^{-3} + C = -\frac{1}{9(3x-1)^3} + C
$$

---

**Example 3** (Fractional $n$ — radical form): Find $\displaystyle \int \sqrt{4x+3} \, dx$.

**Solution**:

$\sqrt{4x+3} = (4x+3)^{1/2}$, $a=4$, $n=\dfrac{1}{2}$.

$$
\int (4x+3)^{1/2} \, dx = \frac{(4x+3)^{3/2}}{4 \cdot (3/2)} + C = \frac{(4x+3)^{3/2}}{6} + C
$$

i.e., $\dfrac{1}{6}(4x+3)^{3/2} + C$.

---

**Example 4** ($n=-1$ case — logarithmic form): Find $\displaystyle \int \frac{1}{2x+5} \, dx$.

**Solution**:

$a=2$, use $\displaystyle \int \frac{1}{ax+b} \, dx = \frac{1}{a}\ln|ax+b| + C$.

$$
\int \frac{1}{2x+5} \, dx = \frac{1}{2} \ln|2x+5| + C
$$

**Verification**: $\dfrac{d}{dx}\left(\dfrac{1}{2}\ln|2x+5|\right) = \dfrac{1}{2} \cdot \dfrac{1}{2x+5} \cdot 2 = \dfrac{1}{2x+5}$. ✓

---

**Example 5** (Comprehensive — two terms mixed): Find $\displaystyle \int \left( \frac{1}{(3x-2)^2} + \frac{4}{x+1} \right) dx$.

**Solution**:

First term: $\displaystyle \int (3x-2)^{-2} \, dx = \frac{(3x-2)^{-1}}{3 \cdot (-1)} + C_1 = -\frac{1}{3(3x-2)} + C_1$

Second term: $\displaystyle \int \frac{4}{x+1} \, dx = 4\ln|x+1| + C_2$

Combine:

$$
\int \left( \frac{1}{(3x-2)^2} + \frac{4}{x+1} \right) dx = -\frac{1}{3(3x-2)} + 4\ln|x+1| + C
$$

---

**Example 6** (Requires simplifying before using formula): Find $\displaystyle \int \frac{2x+3}{(x+1)^2} \, dx$.

**Solution**:

This type of problem requires first decomposing the fraction into partial fractions:

$$
\frac{2x+3}{(x+1)^2} = \frac{2(x+1)+1}{(x+1)^2} = \frac{2}{x+1} + \frac{1}{(x+1)^2}
$$

Then integrate term by term:

$$
\int \frac{2}{x+1} \, dx = 2\ln|x+1|, \quad \int (x+1)^{-2} \, dx = \frac{(x+1)^{-1}}{-1} = -\frac{1}{x+1}
$$

Result:

$$
\int \frac{2x+3}{(x+1)^2} \, dx = 2\ln|x+1| - \frac{1}{x+1} + C
$$

---

### 7.2.4 Integrating Exponential Functions: $\displaystyle \int e^{ax+b} \, dx$

**Formula**:

$$
\boxed{\int e^{ax+b} \, dx = \frac{1}{a} e^{ax+b} + C \quad (a \neq 0)}
$$

**Derivation**: Differentiate the right-hand side:

$$
\frac{d}{dx}\left(\frac{1}{a} e^{ax+b} + C\right) = \frac{1}{a} \cdot e^{ax+b} \cdot a = e^{ax+b}
$$

**Understanding**: Similar to the $(ax+b)^n$ case, dividing by $a$ is because the chain rule gives $(ax+b)' = a$, and the reverse operation produces the factor $\frac{1}{a}$.

In fact, these two formulas can be understood uniformly: when integrating a linear composite function $f(ax+b)$, the result always contains an extra factor $\frac{1}{a}$.

> **Additional knowledge** (for awareness only, not in IGCSE): For a general base $a^x$ ($a>0, a\neq1$), $\displaystyle \int a^x \, dx = \frac{a^x}{\ln a} + C$. This is because $\dfrac{d}{dx}(a^x) = a^x \ln a$.

---

**Example 1** (Basic): Find $\displaystyle \int e^{4x} \, dx$.

**Solution**:

$$
\int e^{4x} \, dx = \frac{1}{4} e^{4x} + C
$$

---

**Example 2** (Negative coefficient): Find $\displaystyle \int e^{-2x} \, dx$.

**Solution**:

$a = -2$, so $\dfrac{1}{a} = -\dfrac{1}{2}$.

$$
\int e^{-2x} \, dx = -\frac{1}{2} e^{-2x} + C
$$

---

**Example 3** (With constant term): Find $\displaystyle \int e^{3x-2} \, dx$.

**Solution**:

$a=3$, $b=-2$.

$$
\int e^{3x-2} \, dx = \frac{1}{3} e^{3x-2} + C
$$

---

**Example 4** (Fractional coefficient): Find $\displaystyle \int e^{\frac{x}{3} + \pi} \, dx$.

**Solution**:

$a = \dfrac{1}{3}$, $\dfrac{1}{a} = 3$.

$$
\int e^{\frac{x}{3} + \pi} \, dx = 3 e^{\frac{x}{3} + \pi} + C
$$

---

**Example 5** (Exponential and polynomial mixed): Find $\displaystyle \int (2x^4 - 3e^{2x} + e) \, dx$.

**Solution**:

Note that $e$ is a constant (Euler's number, $e \approx 2.718$), so $\int e \, dx = ex$.

$$
\begin{aligned}
\int 2x^4 \, dx &= 2 \cdot \frac{x^5}{5} = \frac{2}{5}x^5 \\[4pt]
\int -3e^{2x} \, dx &= -3 \cdot \frac{1}{2} e^{2x} = -\frac{3}{2}e^{2x} \\[4pt]
\int e \, dx &= ex
\end{aligned}
$$

Result:

$$
\int (2x^4 - 3e^{2x} + e) \, dx = \frac{2}{5}x^5 - \frac{3}{2}e^{2x} + ex + C
$$

---

**Example 6** (Exponential mixed — positive and negative exponents): Find $\displaystyle \int (e^{3x} + e^{-3x}) \, dx$.

**Solution**:

$$
\int e^{3x} \, dx = \frac{1}{3}e^{3x}, \quad \int e^{-3x} \, dx = -\frac{1}{3}e^{-3x}
$$

Result:

$$
\int (e^{3x} + e^{-3x}) \, dx = \frac{1}{3}e^{3x} - \frac{1}{3}e^{-3x} + C = \frac{1}{3}(e^{3x} - e^{-3x}) + C
$$

---

### 7.2.5 Integrating Trigonometric Functions

The three basic trigonometric integration formulas are all derived by reversing the derivative formulas learned in Chapter 5.

**Quick reference table**:

| Derivative formula | Corresponding integral formula |
|---------|------------|
| $\dfrac{d}{dx}(\sin x) = \cos x$ | $\displaystyle \int \cos x \, dx = \sin x + C$ |
| $\dfrac{d}{dx}(\cos x) = -\sin x$ | $\displaystyle \int \sin x \, dx = -\cos x + C$ |
| $\dfrac{d}{dx}(\tan x) = \sec^2 x$ | $\displaystyle \int \sec^2 x \, dx = \tan x + C$ |

For the more general $ax+b$ form, all three formulas follow the "divide by $a$" pattern.

---

#### (1) $\displaystyle \int \sin(ax+b) \, dx$

**Formula**:

$$
\boxed{\int \sin(ax+b) \, dx = -\frac{1}{a} \cos(ax+b) + C}
$$

**Derivation**: Assume the antiderivative is $k \cos(ax+b)$. Differentiating gives:

$$
\frac{d}{dx}[k \cos(ax+b)] = k \cdot [-\sin(ax+b)] \cdot a = -ak \sin(ax+b)
$$

We want $-ak = 1$, i.e., $k = -\dfrac{1}{a}$. Therefore the antiderivative is $-\dfrac{1}{a}\cos(ax+b)$.

**Verification**:

$$
\frac{d}{dx}\left(-\frac{1}{a}\cos(ax+b) + C\right) = -\frac{1}{a} \cdot [-\sin(ax+b)] \cdot a = \sin(ax+b) \quad \checkmark
$$

**Key points to remember**:
- $\sin$ integrates to $-\cos$ (note the negative sign)
- Then divide by $a$

---

**Example 1** (Basic): Find $\displaystyle \int \sin(2x) \, dx$.

**Solution**:

$$
\int \sin(2x) \, dx = -\frac{1}{2} \cos(2x) + C
$$

---

**Example 2** (With phase shift): Find $\displaystyle \int \sin(3x + \pi) \, dx$.

**Solution**:

$a=3$, $b=\pi$.

$$
\int \sin(3x + \pi) \, dx = -\frac{1}{3} \cos(3x + \pi) + C
$$

Using $\cos(\theta+\pi) = -\cos\theta$, this simplifies to $\dfrac{1}{3}\cos(3x) + C$, though this is not necessary.

---

**Example 3** (With coefficient): Find $\displaystyle \int -5\sin\left(\frac{x}{2}\right) dx$.

**Solution**:

$a = \dfrac{1}{2}$, $\dfrac{1}{a} = 2$.

$$
\int -5\sin\left(\frac{x}{2}\right) dx = -5 \cdot \left(-2\cos\left(\frac{x}{2}\right)\right) + C = 10\cos\left(\frac{x}{2}\right) + C
$$

---

#### (2) $\displaystyle \int \cos(ax+b) \, dx$

**Formula**:

$$
\boxed{\int \cos(ax+b) \, dx = \frac{1}{a} \sin(ax+b) + C}
$$

**Derivation**: Assume the antiderivative is $k \sin(ax+b)$. Differentiating gives:

$$
\frac{d}{dx}[k \sin(ax+b)] = k \cdot \cos(ax+b) \cdot a = ak \cos(ax+b)
$$

Set $ak = 1$, giving $k = \dfrac{1}{a}$.

**Verification**:

$$
\frac{d}{dx}\left(\frac{1}{a}\sin(ax+b) + C\right) = \frac{1}{a} \cdot \cos(ax+b) \cdot a = \cos(ax+b) \quad \checkmark
$$

**Key points to remember**:
- $\cos$ integrates to $\sin$ (no negative sign)
- Then divide by $a$

---

**Example 1** (Basic): Find $\displaystyle \int \cos(5x) \, dx$.

**Solution**:

$$
\int \cos(5x) \, dx = \frac{1}{5} \sin(5x) + C
$$

---

**Example 2** (With phase shift and coefficient): Find $\displaystyle \int 3\cos(2x-1) \, dx$.

**Solution**:

$$
\int 3\cos(2x-1) \, dx = 3 \cdot \frac{1}{2} \sin(2x-1) + C = \frac{3}{2} \sin(2x-1) + C
$$

---

**Example 3** (Using even function property): Find $\displaystyle \int \cos(-3x) \, dx$.

**Solution**:

Using $\cos(-\theta) = \cos\theta$ (cosine is an even function):

$$
\int \cos(-3x) \, dx = \int \cos(3x) \, dx = \frac{1}{3} \sin(3x) + C
$$

Or directly using the formula with $a=-3$:

$$
\int \cos(-3x) \, dx = \frac{1}{-3} \sin(-3x) + C = -\frac{1}{3}[-\sin(3x)] + C = \frac{1}{3}\sin(3x) + C
$$

Both methods give the same result.

---

#### (3) $\displaystyle \int \sec^2(ax+b) \, dx$

**Formula**:

$$
\boxed{\int \sec^2(ax+b) \, dx = \frac{1}{a} \tan(ax+b) + C}
$$

**Derivation**: $\dfrac{d}{dx}(\tan x) = \sec^2 x$, therefore:

$$
\frac{d}{dx}\left(\frac{1}{a} \tan(ax+b)\right) = \frac{1}{a} \cdot \sec^2(ax+b) \cdot a = \sec^2(ax+b)
$$

**Key points to remember**:
- $\sec^2$ integrates to $\tan$ (no negative sign)
- Then divide by $a$

---

**Example 1** (Basic): Find $\displaystyle \int \sec^2(3x) \, dx$.

**Solution**:

$$
\int \sec^2(3x) \, dx = \frac{1}{3} \tan(3x) + C
$$

---

**Example 2** (With phase shift): Find $\displaystyle \int \sec^2\left(2x - \frac{\pi}{4}\right) dx$.

**Solution**:

$$
\int \sec^2\left(2x - \frac{\pi}{4}\right) dx = \frac{1}{2} \tan\left(2x - \frac{\pi}{4}\right) + C
$$

---

**Example 3** (Comprehensive): Find $\displaystyle \int (2\sec^2 x - 3\sec^2(4x)) \, dx$.

**Solution**:

$$
\int 2\sec^2 x \, dx = 2\tan x, \quad \int -3\sec^2(4x) \, dx = -3 \cdot \frac{1}{4} \tan(4x) = -\frac{3}{4}\tan(4x)
$$

Result:

$$
\int (2\sec^2 x - 3\sec^2(4x)) \, dx = 2\tan x - \frac{3}{4}\tan(4x) + C
$$

---

### 7.2.6 Super Comprehensive Examples (Complete Skills Check)

The following examples cover all types of integration techniques in this chapter. It is recommended to try them yourself first before checking the solutions.

---

**Example 1** (Six-term mix — all types): Find $\displaystyle \int \left( 8x^7 - \frac{3}{x^4} + 5e^{2x} + 2\sin 3x - 4\cos\left(\frac{x}{2}\right) + 6\sec^2(5x) \right) dx$.

**Solution**:

Process each term:

| Term | Integration process | Result |
|---|---------|------|
| $8x^7$ | $8 \cdot \dfrac{x^8}{8}$ | $x^8$ |
| $-\dfrac{3}{x^4} = -3x^{-4}$ | $-3 \cdot \dfrac{x^{-3}}{-3}$ | $\dfrac{1}{x^3}$ |
| $5e^{2x}$ | $5 \cdot \dfrac{1}{2}e^{2x}$ | $\dfrac{5}{2}e^{2x}$ |
| $2\sin 3x$ | $2 \cdot \left(-\dfrac{1}{3}\cos 3x\right)$ | $-\dfrac{2}{3}\cos 3x$ |
| $-4\cos\left(\dfrac{x}{2}\right)$ | $-4 \cdot \dfrac{1}{1/2}\sin\left(\dfrac{x}{2}\right) = -4 \cdot 2\sin\left(\dfrac{x}{2}\right)$ | $-8\sin\left(\dfrac{x}{2}\right)$ |
| $6\sec^2(5x)$ | $6 \cdot \dfrac{1}{5}\tan(5x)$ | $\dfrac{6}{5}\tan(5x)$ |

Combine:

$$
\boxed{x^8 + \frac{1}{x^3} + \frac{5}{2}e^{2x} - \frac{2}{3}\cos 3x - 8\sin\left(\frac{x}{2}\right) + \frac{6}{5}\tan(5x) + C}
$$

---

**Example 2** (Expand first, then integrate — polynomial product): Find $\displaystyle \int (x^2 - 1)(x^2 + 2) \, dx$.

**Solution**:

Expand: $(x^2 - 1)(x^2 + 2) = x^4 + 2x^2 - x^2 - 2 = x^4 + x^2 - 2$

Integrate:

$$
\int (x^4 + x^2 - 2) \, dx = \frac{x^5}{5} + \frac{x^3}{3} - 2x + C
$$

---

**Example 3** (Simplify fraction first, then integrate): Find $\displaystyle \int \frac{2x^4 - 3x^2 + 5x - 1}{x^2} \, dx$.

**Solution**:

Simplify:

$$
\frac{2x^4 - 3x^2 + 5x - 1}{x^2} = 2x^2 - 3 + \frac{5}{x} - \frac{1}{x^2} = 2x^2 - 3 + 5x^{-1} - x^{-2}
$$

Integrate:

$$
\begin{aligned}
\int (2x^2 - 3 + 5x^{-1} - x^{-2}) \, dx &= 2 \cdot \frac{x^3}{3} - 3x + 5\ln|x| - \frac{x^{-1}}{-1} + C \\[4pt]
&= \frac{2}{3}x^3 - 3x + 5\ln|x| + \frac{1}{x} + C
\end{aligned}
$$

---

**Example 4** ($(ax+b)^n$ mixed with trigonometric and exponential): Find $\displaystyle \int \left( (3x+1)^4 + \frac{2}{5x-3} - \sin\left(4x-\frac{\pi}{6}\right) \right) dx$.

**Solution**:

First term: $\displaystyle \int (3x+1)^4 \, dx = \frac{(3x+1)^5}{3 \cdot 5} + C_1 = \frac{(3x+1)^5}{15} + C_1$

Second term: $\displaystyle \int \frac{2}{5x-3} \, dx = 2 \cdot \frac{1}{5} \ln|5x-3| + C_2 = \frac{2}{5}\ln|5x-3| + C_2$

Third term: $\displaystyle \int -\sin\left(4x-\frac{\pi}{6}\right) dx = -\left(-\frac{1}{4}\right)\cos\left(4x-\frac{\pi}{6}\right) + C_3 = \frac{1}{4}\cos\left(4x-\frac{\pi}{6}\right) + C_3$

Combine:

$$
\int \left( (3x+1)^4 + \frac{2}{5x-3} - \sin\left(4x-\frac{\pi}{6}\right) \right) dx = \frac{(3x+1)^5}{15} + \frac{2}{5}\ln|5x-3| + \frac{1}{4}\cos\left(4x-\frac{\pi}{6}\right) + C
$$

---

## 7.3 Definite Integrals

### 7.3.1 From Indefinite to Definite Integrals — The Fundamental Theorem of Calculus

An **indefinite integral** $\displaystyle \int f(x) \, dx$ gives a **family of functions** (containing an arbitrary constant $C$), while a **definite integral** $\displaystyle \int_a^b f(x) \, dx$ gives a **numerical value** — it represents the "accumulated effect" of the function $f(x)$ over the interval $[a, b]$.

The bridge connecting them is the **Fundamental Theorem of Calculus (FTC)**, also known as the **Newton-Leibniz formula**:

$$
\boxed{\int_a^b f(x) \, dx = F(b) - F(a)}
$$

where $F'(x) = f(x)$, i.e., $F(x)$ is any antiderivative of $f(x)$.

**Intuitive derivation**:

Consider the function $A(x) = \int_a^x f(t) \, dt$, which represents the accumulated area from $a$ to $x$. When $x$ increases by a small amount $h$:

$$
A(x+h) - A(x) \approx f(x) \cdot h
$$

Therefore:

$$
\lim_{h \to 0} \frac{A(x+h) - A(x)}{h} = f(x)
$$

i.e., $A'(x) = f(x)$. So $A(x)$ is an antiderivative of $f(x)$. Let $F(x)$ be any antiderivative of $f(x)$, then $F(x) = A(x) + C$. Hence:

$$
F(b) - F(a) = [A(b) + C] - [A(a) + C] = A(b) - A(a) = A(b) - 0 = \int_a^b f(x) \, dx
$$

**Common notation**:

$$
\int_a^b f(x) \, dx = \big[ F(x) \big]_{a}^{b} = \big[ F(x) \big]_{x=a}^{x=b} = F(b) - F(a)
$$

> ⚠️ **Key distinction**: In definite integrals, **do not add the constant of integration $C$**, because it cancels out when computing $F(b)-F(a)$.

---

### 7.3.2 Properties of Definite Integrals

**Property 1 (Linearity)**:

$$
\int_a^b [c f(x) + d g(x)] \, dx = c \int_a^b f(x) \, dx + d \int_a^b g(x) \, dx
$$

**Property 2 (Interval additivity)** — one of the most important properties:

$$
\int_a^b f(x) \, dx = \int_a^c f(x) \, dx + \int_c^b f(x) \, dx
$$

This theorem is crucial for handling cases where the function changes sign. When $f(x)$ changes sign on $[a,b]$, we need to split the interval at the zeros — this is precisely the application of Property 2.

**Property 3 (Reverse interval)**:

$$
\int_a^b f(x) \, dx = -\int_b^a f(x) \, dx
$$

**Derivation**: $\int_a^b f(x) \, dx = F(b)-F(a) = -[F(a)-F(b)] = -\int_b^a f(x) \, dx$.

**Property 4 (Zero interval)**:

$$
\int_a^a f(x) \, dx = 0
$$

**Property 5 (Comparison property)**: If $f(x) \geq g(x)$ on $[a,b]$, then:

$$
\int_a^b f(x) \, dx \geq \int_a^b g(x) \, dx
$$

---

### 7.3.3 Procedure for Computing Definite Integrals

General steps for computing definite integrals:

1. **Find the antiderivative**: Find an antiderivative $F(x)$ of the integrand $f(x)$ (without adding $C$)
2. **Substitute the limits**: Compute $F(b) - F(a)$
3. **Simplify the result**: Give the final numerical value or simplified expression

---

**Example 1** (Simple power function — geometric verification): Evaluate $\displaystyle \int_1^4 (2x+1) \, dx$.

**Solution**:

First find the antiderivative: $\displaystyle \int (2x+1) \, dx = x^2 + x + C$

So:

$$
\int_1^4 (2x+1) \, dx = \big[ x^2 + x \big]_{1}^{4} = (16 + 4) - (1 + 1) = 20 - 2 = 18
$$

**Geometric verification**: $y=2x+1$ is a straight line. At $x=1$, $y=3$; at $x=4$, $y=9$; interval length $3$. Trapezoid area $= \dfrac{3+9}{2} \times 3 = 18$, consistent with the integration result. ✓

---

**Example 2** (Quadratic function): Evaluate $\displaystyle \int_{-1}^{2} (x^2 - 2x + 3) \, dx$.

**Solution**:

$$
\begin{aligned}
\int_{-1}^{2} (x^2 - 2x + 3) \, dx &= \left[ \frac{x^3}{3} - x^2 + 3x \right]_{-1}^{2} \\[4pt]
&= \left( \frac{8}{3} - 4 + 6 \right) - \left( -\frac{1}{3} - 1 - 3 \right) \\[4pt]
&= \left( \frac{8}{3} + 2 \right) - \left( -\frac{1}{3} - 4 \right) \\[4pt]
&= \frac{14}{3} - \left( -\frac{13}{3} \right) = \frac{27}{3} = 9
\end{aligned}
$$

---

**Example 3** (Trigonometric function): Evaluate $\displaystyle \int_0^{\pi} \cos x \, dx$.

**Solution**:

$$
\int_0^{\pi} \cos x \, dx = \big[ \sin x \big]_{0}^{\pi} = \sin \pi - \sin 0 = 0 - 0 = 0
$$

**Geometric meaning**: The cosine function on $[0,\pi]$ is positive on $[0,\pi/2]$ and negative on $[\pi/2,\pi]$. The positive and negative areas exactly cancel out, so the signed area is zero.

---

**Example 4** (Exponential and $1/x$ mixed): Evaluate $\displaystyle \int_1^2 \left( e^{3x} + \frac{2}{x} \right) dx$.

**Solution**:

$$
\begin{aligned}
\int_1^2 \left( e^{3x} + \frac{2}{x} \right) dx &= \left[ \frac{1}{3} e^{3x} + 2\ln|x| \right]_1^2 \\[4pt]
&= \left( \frac{1}{3} e^{6} + 2\ln 2 \right) - \left( \frac{1}{3} e^{3} + 2\ln 1 \right) \\[4pt]
&= \frac{1}{3}(e^6 - e^3) + 2\ln 2
\end{aligned}
$$

(Note that $\ln 1 = 0$)

---

**Example 5** ($(ax+b)^n$ form — comparison of two methods): Evaluate $\displaystyle \int_0^1 (3x+2)^4 \, dx$.

**Solution**:

Method 1 (Using the formula directly): $a=3$, $n=4$.

$$
\int (3x+2)^4 \, dx = \frac{(3x+2)^5}{3 \cdot 5} = \frac{(3x+2)^5}{15}
$$

$$
\int_0^1 (3x+2)^4 \, dx = \left[ \frac{(3x+2)^5}{15} \right]_0^1 = \frac{5^5}{15} - \frac{2^5}{15} = \frac{3125}{15} - \frac{32}{15} = \frac{3093}{15} = \frac{1031}{5}
$$

Method 2 (Expand): $(3x+2)^4 = 81x^4 + 216x^3 + 216x^2 + 96x + 16$

$$
\int_0^1 (81x^4 + 216x^3 + 216x^2 + 96x + 16) \, dx = \left[ \frac{81x^5}{5} + 54x^4 + 72x^3 + 48x^2 + 16x \right]_0^1
$$

$$
= \frac{81}{5} + 54 + 72 + 48 + 16 = \frac{81}{5} + 190 = \frac{81}{5} + \frac{950}{5} = \frac{1031}{5}
$$

Both methods give the same result. ✓

---

**Example 6** (Definite integral with $\ln$): Evaluate $\displaystyle \int_2^4 \frac{1}{x-1} \, dx$.

**Solution**:

$$
\int_2^4 \frac{1}{x-1} \, dx = \big[ \ln|x-1| \big]_2^4 = \ln 3 - \ln 1 = \ln 3
$$

---

### 7.3.4 Definite Integrals and Signed Area

The definite integral $\int_a^b f(x) \, dx$ gives the **signed area**:

- When $f(x) \geq 0$, the integral value is positive, equal to the actual area between the curve and the $x$-axis
- When $f(x) \leq 0$, the integral value is negative, and its absolute value equals the actual area
- When $f(x)$ changes sign, the positive and negative parts cancel each other out

**Example**: Evaluate $\displaystyle \int_{-2}^{3} (x-1) \, dx$ and explain its geometric meaning.

**Solution**:

$$
\int_{-2}^{3} (x-1) \, dx = \left[ \frac{x^2}{2} - x \right]_{-2}^3 = \left( \frac{9}{2} - 3 \right) - \left( 2 + 2 \right) = \frac{3}{2} - 4 = -\frac{5}{2}
$$

The result is $-\dfrac{5}{2}$, indicating that on the interval $[-2,3]$, the area below the $x$-axis is $\dfrac{5}{2}$ square units more than the area above. The function $y=x-1$ crosses the $x$-axis at $x=1$; on $[-2,1]$ the curve is below the axis, and on $[1,3]$ the curve is above.

---

**Example 2** (Using symmetry to simplify computation): Evaluate $\displaystyle \int_{-a}^{a} x^3 \, dx$.

**Solution**:

Since $x^3$ is an odd function ($(-x)^3 = -x^3$), its integral over the symmetric interval $[-a,a]$ is zero:

$$
\int_{-a}^{a} x^3 \, dx = \left[ \frac{x^4}{4} \right]_{-a}^{a} = \frac{a^4}{4} - \frac{a^4}{4} = 0
$$

> **General rules**: The definite integral of an odd function over a symmetric interval is zero; the definite integral of an even function over a symmetric interval equals twice the integral over the half-interval.
> - $f$ is odd: $\int_{-a}^{a} f(x) \, dx = 0$
> - $f$ is even: $\int_{-a}^{a} f(x) \, dx = 2\int_{0}^{a} f(x) \, dx$

---

## 7.4 Plane Area

This section is one of the most important geometric applications of definite integrals. We will systematically learn how to use integration to compute the area of various plane figures.

### 7.4.1 Area Between a Curve and the $x$-axis

**Case 1**: $f(x) \geq 0$ on $[a,b]$

$$
A = \int_a^b f(x) \, dx
$$

**Case 2**: $f(x) \leq 0$ on $[a,b]$

$$
A = -\int_a^b f(x) \, dx = \int_a^b |f(x)| \, dx
$$

**Case 3**: $f(x)$ changes sign on $[a,b]$ (general case)

$$
A = \int_a^b |f(x)| \, dx
$$

**Standard solution procedure**:
1. **Solve $f(x) = 0$**: Find all intersection points of the curve with the $x$-axis
2. **Split the interval**: Use the zeros to divide the integration interval into several subintervals
3. **Determine the sign**: On each subinterval, take a test point to determine whether $f(x)$ is positive or negative
4. **Integrate by segments**: Integrate directly on positive intervals; take the absolute value (add a negative sign) on negative intervals
5. **Sum**: Add the areas of all subintervals

---

**Example 1** (Entirely above the $x$-axis): Find the area bounded by the curve $y = x^2 + 1$ and the $x$-axis from $x=0$ to $x=2$.

**Solution**:

On $[0,2]$, $x^2 + 1 \geq 1 > 0$, so integrate directly:

$$
A = \int_0^2 (x^2 + 1) \, dx = \left[ \frac{x^3}{3} + x \right]_0^2 = \left( \frac{8}{3} + 2 \right) - 0 = \frac{14}{3}
$$

---

**Example 2** (Entirely below the $x$-axis): Find the area bounded by the curve $y = -e^x$ and the $x$-axis from $x=-1$ to $x=1$.

**Solution**:

On $[-1,1]$, $-e^x < 0$, so the area is:

$$
A = -\int_{-1}^{1} (-e^x) \, dx = \int_{-1}^{1} e^x \, dx = \big[ e^x \big]_{-1}^{1} = e - e^{-1}
$$

---

**Example 3** (Sign change — piecewise approach): Find the total area bounded by the curve $y = x^2 - 1$ and the $x$-axis on $[-2, 2]$.

**Solution**:

**Step 1**: Find zeros. $x^2 - 1 = 0 \Rightarrow x = \pm 1$.

**Step 2**: The interval $[-2,2]$ is split by the three points $-2,-1,1,2$ into three subintervals: $[-2,-1]$, $[-1,1]$, $[1,2]$.

**Step 3**: Determine the sign.
- On $[-2,-1]$, take $x=-1.5$: $f(-1.5) = 2.25-1 = 1.25 > 0$, above the axis
- On $[-1,1]$, take $x=0$: $f(0) = -1 < 0$, below the axis
- On $[1,2]$, take $x=1.5$: $f(1.5) = 2.25-1 = 1.25 > 0$, above the axis

**Step 4**:

$$
\begin{aligned}
A &= \int_{-2}^{-1} (x^2-1) \, dx + \int_{-1}^{1} -(x^2-1) \, dx + \int_{1}^{2} (x^2-1) \, dx \\[4pt]
&= \left[ \frac{x^3}{3} - x \right]_{-2}^{-1} + \left[ -\frac{x^3}{3} + x \right]_{-1}^{1} + \left[ \frac{x^3}{3} - x \right]_{1}^{2}
\end{aligned}
$$

First part: $\left( -\frac{1}{3} + 1 \right) - \left( -\frac{8}{3} + 2 \right) = \frac{2}{3} - \left( -\frac{2}{3} \right) = \frac{4}{3}$

Second part: $\left( -\frac{1}{3} + 1 \right) - \left( \frac{1}{3} - 1 \right) = \frac{2}{3} - \left( -\frac{2}{3} \right) = \frac{4}{3}$

Third part: $\left( \frac{8}{3} - 2 \right) - \left( \frac{1}{3} - 1 \right) = \frac{2}{3} - \left( -\frac{2}{3} \right) = \frac{4}{3}$

Total area:

$$
A = \frac{4}{3} + \frac{4}{3} + \frac{4}{3} = 4
$$

---

**Example 4** (Typical exam question — downward-opening parabola): Find the area bounded by the curve $y = 9 - x^2$ and the $x$-axis.

**Solution**:

Intersections with the $x$-axis: $9 - x^2 = 0 \Rightarrow x = \pm 3$.

On $[-3,3]$, $9 - x^2 \geq 0$, so:

$$
\begin{aligned}
A &= \int_{-3}^{3} (9 - x^2) \, dx = \left[ 9x - \frac{x^3}{3} \right]_{-3}^{3} \\[4pt]
&= \left( 27 - 9 \right) - \left( -27 + 9 \right) \\[4pt]
&= 18 - (-18) = 36
\end{aligned}
$$

The area is $36$ square units.

---

**Example 5** (Cubic function — three zeros, two intervals): Find the total area bounded by the curve $y = x^3 - 4x$ and the $x$-axis on $[-2,2]$.

**Solution**:

**Step 1**: $x^3 - 4x = x(x^2-4) = x(x-2)(x+2) = 0$, zeros at $x = -2, 0, 2$.

**Step 2**: The interval is split into $[-2,0]$ and $[0,2]$.

**Step 3**:
- On $[-2,0]$, take $x=-1$: $f(-1) = -1 + 4 = 3 > 0$
- On $[0,2]$, take $x=1$: $f(1) = 1 - 4 = -3 < 0$

**Step 4**:

$$
\begin{aligned}
A &= \int_{-2}^{0} (x^3 - 4x) \, dx + \int_{0}^{2} -(x^3 - 4x) \, dx \\[4pt]
&= \left[ \frac{x^4}{4} - 2x^2 \right]_{-2}^{0} + \left[ -\frac{x^4}{4} + 2x^2 \right]_{0}^{2}
\end{aligned}
$$

First part: $(0) - \left( \frac{16}{4} - 8 \right) = -(4-8) = 4$

Second part: $\left( -\frac{16}{4} + 8 \right) - 0 = (-4+8) = 4$

Total area: $A = 4 + 4 = 8$

---

### 7.4.2 Area Between a Line and a Curve

**Core method**: If on the interval $[a,b]$, the curve $y = f(x)$ lies above the line $y = g(x)$ (i.e., $f(x) \geq g(x)$), then the area between them is:

$$
\boxed{A = \int_a^b [f(x) - g(x)] \, dx}
$$

**Solution procedure**:
1. Find intersection points: solve $f(x) = g(x)$
2. Determine the integration interval
3. Determine which function is above and which is below (take a test point in the interval)
4. Integrate the difference (upper minus lower)

---

**Example 1** (Curve above): Find the area bounded by the curve $y = x^2 + 1$ and the line $y = x + 3$.

**Solution**:

**Step 1**: Intersection points: $x^2 + 1 = x + 3 \Rightarrow x^2 - x - 2 = 0 \Rightarrow (x-2)(x+1) = 0$, giving $x = -1$ or $x = 2$.

**Step 2**: The interval is $[-1,2]$.

**Step 3**: Test with $x=0$: $f(0) = 1$, $g(0) = 3$, so $g(x) = x+3$ is above.

**Step 4**:

$$
\begin{aligned}
A &= \int_{-1}^{2} [(x+3) - (x^2+1)] \, dx \\[4pt]
&= \int_{-1}^{2} (2 + x - x^2) \, dx \\[4pt]
&= \left[ 2x + \frac{x^2}{2} - \frac{x^3}{3} \right]_{-1}^{2} \\[4pt]
&= \left( 4 + 2 - \frac{8}{3} \right) - \left( -2 + \frac{1}{2} + \frac{1}{3} \right) \\[4pt]
&= \frac{10}{3} - \left( -\frac{7}{6} \right) = \frac{10}{3} + \frac{7}{6} = \frac{27}{6} = \frac{9}{2}
\end{aligned}
$$

---

**Example 2** (Line above — classic problem): Find the area bounded by the line $y = 2x$ and the curve $y = x^2$.

**Solution**:

Intersection points: $x^2 = 2x \Rightarrow x^2 - 2x = 0 \Rightarrow x(x-2) = 0$, giving $x=0$ and $x=2$.

On $[0,2]$, test with $x=1$: $f(1)=1$, $g(1)=2$, so $y=2x$ is above.

$$
A = \int_0^2 (2x - x^2) \, dx = \left[ x^2 - \frac{x^3}{3} \right]_0^2 = \left( 4 - \frac{8}{3} \right) - 0 = \frac{4}{3}
$$

---

**Example 3** (Root function and line): Find the area bounded by the curve $y = \sqrt{x}$ and the line $y = \dfrac{x}{2}$.

**Solution**:

Intersection points: $\sqrt{x} = \dfrac{x}{2} \Rightarrow 2\sqrt{x} = x \Rightarrow x = 2\sqrt{x} \Rightarrow x - 2\sqrt{x} = 0 \Rightarrow \sqrt{x}(\sqrt{x} - 2) = 0$, giving $x=0$ or $x=4$.

On $[0,4]$, test with $x=1$: $\sqrt{1}=1$, $\dfrac{1}{2}=0.5$, so $y=\sqrt{x}$ is above.

$$
\begin{aligned}
A &= \int_0^4 \left( \sqrt{x} - \frac{x}{2} \right) dx = \int_0^4 \left( x^{1/2} - \frac{x}{2} \right) dx \\[4pt]
&= \left[ \frac{2}{3}x^{3/2} - \frac{x^2}{4} \right]_0^4 = \left( \frac{2}{3} \cdot 8 - \frac{16}{4} \right) - 0 = \frac{16}{3} - 4 = \frac{4}{3}
\end{aligned}
$$

---

### 7.4.3 Area Between Two Curves

When two curves $y = f(x)$ and $y = g(x)$ have multiple intersection points over an interval, piecewise handling is required — on each subinterval, determine which curve is above and which is below.

---

**Example 1** (Symmetric curves): Find the area bounded by $y = x^2$ and $y = 4 - x^2$.

**Solution**:

Intersection points: $x^2 = 4 - x^2 \Rightarrow 2x^2 = 4 \Rightarrow x^2 = 2 \Rightarrow x = \pm\sqrt{2}$.

On $[-\sqrt{2}, \sqrt{2}]$, test with $x=0$: $f(0)=0$, $g(0)=4$, so $y=4-x^2$ is above.

$$
\begin{aligned}
A &= \int_{-\sqrt{2}}^{\sqrt{2}} [(4 - x^2) - x^2] \, dx = \int_{-\sqrt{2}}^{\sqrt{2}} (4 - 2x^2) \, dx \\[4pt]
&= \left[ 4x - \frac{2x^3}{3} \right]_{-\sqrt{2}}^{\sqrt{2}} \\[4pt]
&= \left( 4\sqrt{2} - \frac{4\sqrt{2}}{3} \right) - \left( -4\sqrt{2} + \frac{4\sqrt{2}}{3} \right) \\[4pt]
&= \frac{8\sqrt{2}}{3} - \left( -\frac{8\sqrt{2}}{3} \right) = \frac{16\sqrt{2}}{3}
\end{aligned}
$$

---

**Example 2** (Upper/lower relationship changes — needs piecewise splitting): Find the total area bounded by $y = x^3$ and $y = x$.

**Solution**:

Intersection points: $x^3 = x \Rightarrow x^3 - x = 0 \Rightarrow x(x-1)(x+1) = 0$, giving $x = -1, 0, 1$.

The interval is split into $[-1,0]$ and $[0,1]$.

- On $[-1,0]$, test with $x=-0.5$: $f(-0.5) = -0.125$, $g(-0.5) = -0.5$, $y=x^3$ is above (since $-0.125 > -0.5$)
- On $[0,1]$, test with $x=0.5$: $f(0.5)=0.125$, $g(0.5)=0.5$, $y=x$ is above

$$
\begin{aligned}
A &= \int_{-1}^{0} (x^3 - x) \, dx + \int_{0}^{1} (x - x^3) \, dx \\[4pt]
&= \left[ \frac{x^4}{4} - \frac{x^2}{2} \right]_{-1}^{0} + \left[ \frac{x^2}{2} - \frac{x^4}{4} \right]_{0}^{1} \\[4pt]
&= \left(0 - \left(\frac{1}{4} - \frac{1}{2}\right)\right) + \left(\left(\frac{1}{2} - \frac{1}{4}\right) - 0\right) \\[4pt]
&= \frac{1}{4} + \frac{1}{4} = \frac{1}{2}
\end{aligned}
$$

---

### 7.4.4 Sum of Multiple Areas (Syllabus Focus)

The syllabus explicitly requires "a sum of two areas." The key step in such problems is **correctly splitting the interval**.

---

**Example 1** (Cubic function with $x$-axis — three segments): Find the total area bounded by the curve $y = x^3 - x^2 - 2x$ and the $x$-axis.

**Solution**:

Factorise: $x^3 - x^2 - 2x = x(x^2 - x - 2) = x(x-2)(x+1)$, zeros at $x = -1, 0, 2$.

- On $[-1,0]$, $f(-0.5) = 0.625 > 0$
- On $[0,2]$, $f(1) = -2 < 0$

$$
\begin{aligned}
A &= \int_{-1}^{0} (x^3 - x^2 - 2x) \, dx + \int_{0}^{2} -(x^3 - x^2 - 2x) \, dx \\[4pt]
&= \left[ \frac{x^4}{4} - \frac{x^3}{3} - x^2 \right]_{-1}^{0} + \left[ -\frac{x^4}{4} + \frac{x^3}{3} + x^2 \right]_{0}^{2}
\end{aligned}
$$

First part: $(0) - \left( \frac{1}{4} + \frac{1}{3} - 1 \right) = -\left( -\frac{5}{12} \right) = \frac{5}{12}$

Second part: $\left( -\frac{16}{4} + \frac{8}{3} + 4 \right) - 0 = \left( -4 + 4 \right) + \frac{8}{3} = \frac{8}{3}$

Total area: $A = \dfrac{5}{12} + \dfrac{8}{3} = \dfrac{5}{12} + \dfrac{32}{12} = \dfrac{37}{12}$

---

**Example 2** (Quadratic function — three segments): Find the total area bounded by the curve $y = x^2 - 4x + 3$ and the $x$-axis on $[0,4]$.

**Solution**:

Zeros: $x^2 - 4x + 3 = (x-1)(x-3) = 0$, giving $x=1, 3$.

The interval $[0,4]$ is split into $[0,1]$, $[1,3]$, $[3,4]$.

- $[0,1]$: $f(0.5) = 1.25 > 0$
- $[1,3]$: $f(2) = -1 < 0$
- $[3,4]$: $f(3.5) = 1.25 > 0$

$$
\begin{aligned}
A &= \int_0^1 (x^2 - 4x + 3) dx + \int_1^3 -(x^2 - 4x + 3) dx + \int_3^4 (x^2 - 4x + 3) dx \\[4pt]
&= \left[ \frac{x^3}{3} - 2x^2 + 3x \right]_0^1 + \left[ -\frac{x^3}{3} + 2x^2 - 3x \right]_1^3 + \left[ \frac{x^3}{3} - 2x^2 + 3x \right]_3^4 \\[4pt]
&= \frac{4}{3} + \frac{4}{3} + \frac{4}{3} = 4
\end{aligned}
$$

---

### 7.4.5 Summary of Strategies for Plane Area Problems

| Scenario | Identifying Feature | Method |
|------|---------|------|
| Curve above $x$-axis | $f(x) \geq 0$ | $A = \int_a^b f(x) \, dx$ |
| Curve below $x$-axis | $f(x) \leq 0$ | $A = -\int_a^b f(x) \, dx$ |
| Curve crosses $x$-axis | $f(x)$ changes sign | Split at zeros, take absolute values separately |
| Line and curve | Two functions given | $A = \int_a^b [f(x)-g(x)] \, dx$ (upper minus lower) |
| Two curves, multiple intersections | Multiple intersection points | Piecewise handling, upper minus lower on each segment |
| Sum of multiple areas | Three or more subintervals | Integrate each separately, then add |

---

### 7.5 Application of Definite Integrals to Kinematics

> **Syllabus reference 14.14**: Use differentiation and integration to solve kinematics problems (displacement, velocity, acceleration).

In Chapter 5, we learned to use **differentiation** to find velocity and acceleration from displacement. **Integration** provides the reverse path: given acceleration, find velocity; given velocity, find displacement.

**Core relationships** (to be discussed in detail in Chapter 10):

$$
a(t) = \frac{dv}{dt}, \quad v(t) = \frac{ds}{dt}
$$

Reverse:

$$
v(t) = \int a(t) \, dt, \quad s(t) = \int v(t) \, dt
$$

---

**Example 1** (Given acceleration, find velocity and displacement): A particle moves along a straight line with acceleration $a(t) = 12t^2 - 6$. At $t=0$, the velocity is $v=2$ and the displacement is $s=1$. Find $v(t)$ and $s(t)$.

**Solution**:

$$
v(t) = \int (12t^2 - 6) \, dt = 4t^3 - 6t + C
$$

From $v(0) = 2$, we get $C = 2$, so $v(t) = 4t^3 - 6t + 2$.

$$
s(t) = \int (4t^3 - 6t + 2) \, dt = t^4 - 3t^2 + 2t + D
$$

From $s(0) = 1$, we get $D = 1$, so $s(t) = t^4 - 3t^2 + 2t + 1$.

---

**Example 2** (Finding displacement from $v(t)$): A particle's velocity is $v(t) = t^2 - 5t + 6$. Find the net displacement from $t=1$ to $t=4$.

**Solution**:

Net displacement $= \displaystyle \int_1^4 (t^2 - 5t + 6) \, dt = \left[ \frac{t^3}{3} - \frac{5t^2}{2} + 6t \right]_1^4$

$$
= \left( \frac{64}{3} - \frac{80}{2} + 24 \right) - \left( \frac{1}{3} - \frac{5}{2} + 6 \right) = \left( \frac{64}{3} - 40 + 24 \right) - \left( \frac{1}{3} + \frac{1}{2} \right)
$$

$$
= \left( \frac{64}{3} - 16 \right) - \frac{5}{6} = \frac{16}{3} - \frac{5}{6} = \frac{32}{6} - \frac{5}{6} = \frac{27}{6} = \frac{9}{2}
$$

The net displacement is $\dfrac{9}{2}$ units in the positive direction.

---

(More content on kinematics will be discussed in depth in Chapter 10.)

---

## Chapter Core Formula Quick Reference Table

| Integrand | Indefinite Integral | Conditions/Notes |
|---------|---------|---------|
| $x^n$ | $\displaystyle \frac{x^{n+1}}{n+1} + C$ | $n \neq -1$ |
| $\dfrac{1}{x}$ | $\displaystyle \ln|x| + C$ | Memorise separately; power rule fails |
| $e^{ax+b}$ | $\displaystyle \frac{1}{a}e^{ax+b} + C$ | $a \neq 0$ |
| $\sin(ax+b)$ | $\displaystyle -\frac{1}{a}\cos(ax+b) + C$ | $a \neq 0$ |
| $\cos(ax+b)$ | $\displaystyle \frac{1}{a}\sin(ax+b) + C$ | $a \neq 0$ |
| $\sec^2(ax+b)$ | $\displaystyle \frac{1}{a}\tan(ax+b) + C$ | $a \neq 0$ |
| $(ax+b)^n$ | $\displaystyle \frac{(ax+b)^{n+1}}{a(n+1)} + C$ | $n \neq -1$ |
| $\dfrac{1}{ax+b}$ | $\displaystyle \frac{1}{a}\ln|ax+b| + C$ | $a \neq 0$ |
| Definite integral $\int_a^b f(x) \, dx$ | $F(b) - F(a)$ | $F'(x) = f(x)$, no $C$ |
| Plane area (upper $-$ lower) | $\displaystyle \int_a^b [f(x)-g(x)] \, dx$ | First confirm $f(x) \geq g(x)$ |
| Area for sign-changing curve with $x$-axis | Split at zeros, take absolute values | First find zeros |

---

## Practice Problems

The following practice problems are graded by difficulty, covering all knowledge points in this chapter. **Answers are at the end.**

---

### Group A: Basic Indefinite Integrals

1. $\displaystyle \int x^9 \, dx$
2. $\displaystyle \int \frac{1}{x^5} \, dx$
3. $\displaystyle \int \sqrt[5]{x} \, dx$
4. $\displaystyle \int \frac{1}{\sqrt[3]{x}} \, dx$
5. $\displaystyle \int (4x^3 - 3x^2 + 2x - 1) \, dx$
6. $\displaystyle \int \frac{6}{x} \, dx$
7. $\displaystyle \int e^{7x} \, dx$
8. $\displaystyle \int e^{-\frac{x}{3}} \, dx$
9. $\displaystyle \int \sin(4x) \, dx$
10. $\displaystyle \int \cos\left(\frac{x}{3}\right) dx$
11. $\displaystyle \int \sec^2(6x) \, dx$
12. $\displaystyle \int (5x-2)^3 \, dx$

---

### Group B: Advanced Indefinite Integrals

13. $\displaystyle \int \left( 2x^6 - 5x^{-4} + \frac{3}{x^2} \right) dx$
14. $\displaystyle \int \left( \frac{1}{3x} + e^{4x} \right) dx$
15. $\displaystyle \int \left( \sin\frac{x}{2} + \cos 2x \right) dx$
16. $\displaystyle \int \frac{1}{(2x+3)^3} \, dx$
17. $\displaystyle \int \left( 2e^{3x-1} - 5\sin\left(2x+\frac{\pi}{4}\right) + 3\sec^2(1-2x) \right) dx$
18. $\displaystyle \int \frac{x^4 + 2x^2 - 3}{x^2} \, dx$
19. $\displaystyle \int (e^x - 1)^2 \, dx$
20. $\displaystyle \int \frac{5}{\sqrt{3x+2}} \, dx$
21. $\displaystyle \int \left( \frac{3}{2x-1} + \frac{1}{(x+2)^4} \right) dx$
22. $\displaystyle \int \frac{2x^2+3x+1}{x} \, dx$

---

### Group C: Definite Integrals

23. $\displaystyle \int_0^4 3x \, dx$
24. $\displaystyle \int_1^3 (2x-1) \, dx$
25. $\displaystyle \int_{-1}^2 (x^2 + 2) \, dx$
26. $\displaystyle \int_0^{\pi/2} \cos x \, dx$
27. $\displaystyle \int_0^2 e^{3x} \, dx$
28. $\displaystyle \int_1^4 \frac{3}{\sqrt{x}} \, dx$
29. $\displaystyle \int_0^{\pi/3} \sec^2 x \, dx$
30. $\displaystyle \int_{-1}^1 (x^5 - x^3) \, dx$ (use symmetry)
31. $\displaystyle \int_0^1 (4x-1)^3 \, dx$
32. $\displaystyle \int_0^{\pi/4} \sin\left(2x+\frac{\pi}{4}\right) dx$
33. $\displaystyle \int_2^5 \frac{2}{x-1} \, dx$
34. $\displaystyle \int_0^1 (e^{2x} + e^{-x}) \, dx$

---

### Group D: Plane Area

35. Find the area bounded by the curve $y = x^2 + 2$ and the $x$-axis from $x=0$ to $x=2$.
36. Find the area bounded by the curve $y = 4 - x^2$ and the $x$-axis.
37. Find the total area bounded by the curve $y = x^2 - 2x - 3$ and the $x$-axis.
38. Find the total area bounded by the curve $y = x^2 - 2x$ and the $x$-axis on $[-1, 3]$.
39. Find the area bounded by the line $y = 2x + 3$ and the curve $y = x^2$.
40. Find the area bounded by the curve $y = x^2 - 4x + 5$ and the line $y = x + 1$.
41. Find the area bounded by the curves $y = x^2$ and $y = 2x - x^2$.
42. Find the total area bounded by $y = x^3 - 4x$ and the $x$-axis.
43. Find the area bounded by $y = 4x - x^2$ and the line $y = x$.
44. Find the area bounded by $y = x^2$ and the line $y = 4$.

---

## Answers to Practice Problems

### Group A Answers

1. $\displaystyle \frac{x^{10}}{10} + C$
2. $\displaystyle -\frac{1}{4x^4} + C$
   **Detailed**: $\int x^{-5} dx = \dfrac{x^{-4}}{-4} = -\dfrac{1}{4x^4}$
3. $\displaystyle \frac{5}{6}x^{6/5} + C$
   **Detailed**: $\sqrt[5]{x} = x^{1/5}$, $\int x^{1/5} dx = \dfrac{x^{6/5}}{6/5} = \dfrac{5}{6}x^{6/5}$
4. $\displaystyle \frac{3}{2}x^{2/3} + C$
   **Detailed**: $\dfrac{1}{\sqrt[3]{x}} = x^{-1/3}$, $\int x^{-1/3} dx = \dfrac{x^{2/3}}{2/3} = \dfrac{3}{2}x^{2/3}$
5. $\displaystyle x^4 - x^3 + x^2 - x + C$
6. $6\ln|x| + C$
7. $\displaystyle \frac{1}{7}e^{7x} + C$
8. $\displaystyle -3e^{-\frac{x}{3}} + C$
   **Detailed**: $\int e^{-\frac{x}{3}} dx = \dfrac{1}{-1/3} e^{-\frac{x}{3}} = -3e^{-\frac{x}{3}}$
9. $\displaystyle -\frac{1}{4}\cos(4x) + C$
10. $\displaystyle 3\sin\left(\frac{x}{3}\right) + C$
    **Detailed**: $\int \cos\left(\frac{x}{3}\right) dx = \dfrac{1}{1/3}\sin\left(\frac{x}{3}\right) = 3\sin\left(\frac{x}{3}\right)$
11. $\displaystyle \frac{1}{6}\tan(6x) + C$
12. $\displaystyle \frac{(5x-2)^4}{20} + C$
    **Detailed**: $\int (5x-2)^3 dx = \dfrac{(5x-2)^4}{5 \cdot 4} = \dfrac{(5x-2)^4}{20}$

---

### Group B Answers

13. $\displaystyle \frac{2}{7}x^7 + \frac{5}{3x^3} - \frac{3}{x} + C$
    **Detailed**: $\int 2x^6 dx = \frac{2}{7}x^7$, $\int -5x^{-4} dx = -5 \cdot \frac{x^{-3}}{-3} = \frac{5}{3}x^{-3} = \frac{5}{3x^3}$, $\int 3x^{-2} dx = 3 \cdot \frac{x^{-1}}{-1} = -\frac{3}{x}$
14. $\displaystyle \frac{1}{3}\ln|x| + \frac{1}{4}e^{4x} + C$
15. $\displaystyle -2\cos\frac{x}{2} + \frac{1}{2}\sin 2x + C$
    **Detailed**: $\int \sin\frac{x}{2} dx = -\dfrac{1}{1/2}\cos\frac{x}{2} = -2\cos\frac{x}{2}$, $\int \cos 2x dx = \frac{1}{2}\sin 2x$
16. $\displaystyle -\frac{1}{4(2x+3)^2} + C$
    **Detailed**: $\int (2x+3)^{-3} dx = \dfrac{(2x+3)^{-2}}{2 \cdot (-2)} = -\dfrac{1}{4}(2x+3)^{-2} = -\dfrac{1}{4(2x+3)^2}$
17. $\displaystyle \frac{2}{3}e^{3x-1} + \frac{5}{2}\cos\left(2x+\frac{\pi}{4}\right) - \frac{3}{2}\tan(1-2x) + C$
    **Detailed**: $\int 2e^{3x-1} dx = 2 \cdot \frac{1}{3}e^{3x-1} = \frac{2}{3}e^{3x-1}$
    $\int -5\sin(2x+\frac{\pi}{4}) dx = -5 \cdot (-\frac{1}{2})\cos(2x+\frac{\pi}{4}) = \frac{5}{2}\cos(2x+\frac{\pi}{4})$
    $\int 3\sec^2(1-2x) dx = 3 \cdot \frac{1}{-2}\tan(1-2x) = -\frac{3}{2}\tan(1-2x)$
18. $\displaystyle \frac{x^3}{3} + 2x + \frac{3}{x} + C$
    **Detailed**: $\dfrac{x^4+2x^2-3}{x^2} = x^2 + 2 - 3x^{-2}$, integrating gives $\frac{x^3}{3} + 2x + \frac{3}{x} + C$
19. $\displaystyle \frac{1}{2}e^{2x} - 2e^x + x + C$
    **Detailed**: $(e^x-1)^2 = e^{2x} - 2e^x + 1$, $\int e^{2x} dx = \frac{1}{2}e^{2x}$, $\int -2e^x dx = -2e^x$, $\int 1 dx = x$
20. $\displaystyle \frac{10}{3}\sqrt{3x+2} + C$
    **Detailed**: $\int 5(3x+2)^{-1/2} dx = 5 \cdot \dfrac{(3x+2)^{1/2}}{3 \cdot (1/2)} = 5 \cdot \dfrac{2}{3}\sqrt{3x+2} = \frac{10}{3}\sqrt{3x+2}$
21. $\displaystyle \frac{3}{2}\ln|2x-1| - \frac{1}{3(x+2)^3} + C$
    **Detailed**: $\int \frac{3}{2x-1} dx = 3 \cdot \frac{1}{2}\ln|2x-1| = \frac{3}{2}\ln|2x-1|$
    $\int (x+2)^{-4} dx = \dfrac{(x+2)^{-3}}{-3} = -\dfrac{1}{3(x+2)^3}$
22. $\displaystyle x^2 + 3x + \ln|x| + C$
    **Detailed**: $\dfrac{2x^2+3x+1}{x} = 2x + 3 + \frac{1}{x}$, integrating gives $x^2 + 3x + \ln|x| + C$

---

### Group C Answers

23. $24$
    **Detailed**: $\int_0^4 3x \, dx = \left[\frac{3x^2}{2}\right]_0^4 = \frac{48}{2} = 24$
24. $6$
    **Detailed**: $\int_1^3 (2x-1) dx = [x^2 - x]_1^3 = (9-3) - (1-1) = 6$
25. $9$
    **Detailed**: $\int_{-1}^2 (x^2+2) dx = \left[\frac{x^3}{3}+2x\right]_{-1}^2 = \left(\frac{8}{3}+4\right) - \left(-\frac{1}{3}-2\right) = \frac{20}{3} + \frac{7}{3} = \frac{27}{3} = 9$
26. $1$
    **Detailed**: $\int_0^{\pi/2} \cos x \, dx = [\sin x]_0^{\pi/2} = 1 - 0 = 1$
27. $\displaystyle \frac{1}{3}(e^6 - 1)$
    **Detailed**: $\int_0^2 e^{3x} dx = \left[\frac{1}{3}e^{3x}\right]_0^2 = \frac{1}{3}e^6 - \frac{1}{3}e^0 = \frac{1}{3}(e^6-1)$
28. $6$
    **Detailed**: $\int_1^4 3x^{-1/2} dx = [6\sqrt{x}]_1^4 = 6 \cdot 2 - 6 \cdot 1 = 12 - 6 = 6$
29. $\sqrt{3}$
    **Detailed**: $\int_0^{\pi/3} \sec^2 x \, dx = [\tan x]_0^{\pi/3} = \sqrt{3} - 0 = \sqrt{3}$
30. $0$
    **Detailed**: $x^5 - x^3$ is odd, integral over symmetric interval $[-1,1]$ is zero.
31. $5$
    **Detailed**: $\int_0^1 (4x-1)^3 dx = \left[\frac{(4x-1)^4}{4 \cdot 4}\right]_0^1 = \left[\frac{(4x-1)^4}{16}\right]_0^1 = \frac{3^4}{16} - \frac{(-1)^4}{16} = \frac{81}{16} - \frac{1}{16} = \frac{80}{16} = 5$
32. $\displaystyle \frac{\sqrt{2}}{2}$
    **Detailed**: $\int_0^{\pi/4} \sin(2x+\frac{\pi}{4}) dx = \left[-\frac{1}{2}\cos(2x+\frac{\pi}{4})\right]_0^{\pi/4}$
    $= -\frac{1}{2}\left[\cos(\frac{\pi}{2}+\frac{\pi}{4}) - \cos\frac{\pi}{4}\right] = -\frac{1}{2}\left[-\frac{\sqrt{2}}{2} - \frac{\sqrt{2}}{2}\right] = -\frac{1}{2}(-\sqrt{2}) = \frac{\sqrt{2}}{2}$
33. $2\ln 4 = 4\ln 2$
    **Detailed**: $\int_2^5 \frac{2}{x-1} dx = [2\ln|x-1|]_2^5 = 2\ln 4 - 2\ln 1 = 2\ln 4 = 4\ln 2$
34. $\displaystyle \frac{1}{2}(e^2 + 1) - \frac{1}{e}$
    **Detailed**: $\int_0^1 (e^{2x} + e^{-x}) dx = \left[\frac{1}{2}e^{2x} - e^{-x}\right]_0^1 = \left(\frac{1}{2}e^2 - e^{-1}\right) - \left(\frac{1}{2} - 1\right) = \frac{1}{2}e^2 - \frac{1}{e} + \frac{1}{2} = \frac{1}{2}(e^2+1) - \frac{1}{e}$

---

### Group D Answers

35. $\displaystyle \frac{20}{3}$
    **Detailed**: $A = \int_0^2 (x^2+2) dx = \left[\frac{x^3}{3}+2x\right]_0^2 = \frac{8}{3} + 4 = \frac{20}{3}$
36. $\displaystyle \frac{32}{3}$
    **Detailed**: Intersects $x$-axis at $x=\pm2$. $A = \int_{-2}^2 (4-x^2) dx = \left[4x-\frac{x^3}{3}\right]_{-2}^2 = (8-\frac{8}{3}) - (-8+\frac{8}{3}) = \frac{16}{3} + \frac{16}{3} = \frac{32}{3}$
37. $\displaystyle \frac{32}{3}$
    **Detailed**: $x^2-2x-3 = (x-3)(x+1)=0$, zeros $x=-1,3$. On $[-1,3]$, $f(x)\leq0$.
    $A = -\int_{-1}^3 (x^2-2x-3) dx = \int_{-1}^3 (-x^2+2x+3) dx = \left[-\frac{x^3}{3}+x^2+3x\right]_{-1}^3$
    $= (-9+9+9) - (\frac{1}{3}+1-3) = 9 - (-\frac{5}{3}) = \frac{32}{3}$
38. $\displaystyle 4$
    **Detailed**: $x^2-2x = x(x-2)=0$, zeros $x=0,2$.
    On $[-1,0]$ $f(x)\geq0$, on $[0,2]$ $f(x)\leq0$, on $[2,3]$ $f(x)\geq0$.
    $A = \int_{-1}^0 (x^2-2x) dx + \int_0^2 -(x^2-2x) dx + \int_2^3 (x^2-2x) dx$
    $= \left[\frac{x^3}{3}-x^2\right]_{-1}^0 + \left[-\frac{x^3}{3}+x^2\right]_0^2 + \left[\frac{x^3}{3}-x^2\right]_2^3$
    $= \frac{4}{3} + \frac{4}{3} + \frac{4}{3} = 4$
39. $\displaystyle \frac{32}{3}$
    **Detailed**: Intersection: $x^2 = 2x+3 \Rightarrow x^2-2x-3=0 \Rightarrow (x-3)(x+1)=0$, $x=-1,3$.
    On $[-1,3]$, $y=2x+3$ is above.
    $A = \int_{-1}^3 [(2x+3)-x^2] dx = \left[x^2+3x-\frac{x^3}{3}\right]_{-1}^3$
    $= (9+9-9) - (1-3+\frac{1}{3}) = 9 - (-\frac{5}{3}) = \frac{32}{3}$
40. $\displaystyle \frac{9}{2}$
    **Detailed**: Intersection: $x^2-4x+5 = x+1 \Rightarrow x^2-5x+4=0 \Rightarrow (x-1)(x-4)=0$, $x=1,4$.
    On $[1,4]$, $y=x+1$ is above (test $x=2$: $f(2)=1$, $g(2)=3$).
    $A = \int_1^4 [(x+1)-(x^2-4x+5)] dx = \int_1^4 (-x^2+5x-4) dx$
    $= \left[-\frac{x^3}{3}+\frac{5x^2}{2}-4x\right]_1^4$
    $= \left(-\frac{64}{3}+40-16\right) - \left(-\frac{1}{3}+\frac{5}{2}-4\right)$
    $= \frac{8}{3} - \left(-\frac{11}{6}\right) = \frac{8}{3} + \frac{11}{6} = \frac{27}{6} = \frac{9}{2}$
41. $\displaystyle \frac{1}{3}$
    **Detailed**: Intersection: $x^2 = 2x-x^2 \Rightarrow 2x^2-2x=0 \Rightarrow 2x(x-1)=0$, $x=0,1$.
    On $[0,1]$, $y=2x-x^2$ is above (test $x=0.5$: $0.25$ vs $0.75$).
    $A = \int_0^1 [(2x-x^2)-x^2] dx = \int_0^1 (2x-2x^2) dx = \left[x^2-\frac{2x^3}{3}\right]_0^1 = 1 - \frac{2}{3} = \frac{1}{3}$
42. $\displaystyle 8$
    **Detailed**: $x^3-4x = x(x-2)(x+2)=0$, zeros $x=-2,0,2$.
    On $[-2,0]$ $f(x)\geq0$, on $[0,2]$ $f(x)\leq0$.
    $A = \int_{-2}^0 (x^3-4x)dx + \int_0^2 -(x^3-4x)dx$
    $= \left[\frac{x^4}{4}-2x^2\right]_{-2}^0 + \left[-\frac{x^4}{4}+2x^2\right]_0^2$
    $= (0-(4-8)) + ((-4+8)-0) = 4 + 4 = 8$
43. $\displaystyle \frac{9}{2}$
    **Detailed**: Intersection: $4x-x^2 = x \Rightarrow 3x-x^2=0 \Rightarrow x(3-x)=0$, $x=0,3$.
    On $[0,3]$, $y=4x-x^2$ is above.
    $A = \int_0^3 [(4x-x^2)-x] dx = \int_0^3 (3x-x^2) dx = \left[\frac{3x^2}{2}-\frac{x^3}{3}\right]_0^3 = \frac{27}{2} - 9 = \frac{9}{2}$
44. $\displaystyle \frac{32}{3}$
    **Detailed**: Intersection: $x^2 = 4 \Rightarrow x = \pm 2$.
    On $[-2,2]$, $y=4$ is above.
    $A = \int_{-2}^2 (4 - x^2) dx = \left[4x - \frac{x^3}{3}\right]_{-2}^2 = (8-\frac{8}{3}) - (-8+\frac{8}{3}) = \frac{16}{3} + \frac{16}{3} = \frac{32}{3}$

---

## Appendix: Common Mistakes and Pitfall Guide

| # | Type of Mistake | ❌ Incorrect | ✅ Correct | Reason |
|---|---------|-----------|-----------|------|
| 1 | Forgetting $+C$ | $\int 2x \, dx = x^2$ | $\int 2x \, dx = x^2 + C$ | Indefinite integral is a family of functions, not a single function |
| 2 | Misapplying power rule to $1/x$ | $\int x^{-1} dx = \frac{x^0}{0}$ | $\int \frac{1}{x} dx = \ln\|x\| + C$ | When $n=-1$, denominator is zero, formula fails |
| 3 | Omitting $1/a$ in $(ax+b)^n$ | $\int (2x+1)^3 = \frac{(2x+1)^4}{4}$ | $\int (2x+1)^3 = \frac{(2x+1)^4}{8}$ | Reverse chain rule produces factor $1/a$ |
| 4 | Wrong sign for $\sin$ integral | $\int \sin(2x) = \frac{1}{2}\cos(2x)$ | $\int \sin(2x) = -\frac{1}{2}\cos(2x)$ | Antiderivative of $\sin$ is $-\cos$, not $\cos$ |
| 5 | Adding $C$ in definite integrals | $\int_1^2 2x = [x^2+C]_1^2$ | $\int_1^2 2x = [x^2]_1^2 = 4-1=3$ | $C$ cancels out in subtraction, no need to write |
| 6 | Not splitting area for sign changes | Directly compute $\int_{-2}^2 (x^2-1) dx$ | Split at $x=\pm1$ and take absolute values | Definite integral gives signed area, not actual area |
| 7 | Wrong identification of upper/lower function | Assume $f$ is above | Use a test point to confirm | Area must be positive; upper minus lower must not be reversed |
| 8 | Integrating a product separately | $\int (x+1)(x-1)dx = \int(x+1)dx \cdot \int(x-1)dx$ | Expand first, then integrate | No product rule for integration |
| 9 | Omitting absolute value in $\ln$ | $\int\frac{1}{x}dx = \ln x + C$ | $\int\frac{1}{x}dx = \ln\|x\| + C$ | $\ln x$ is undefined when $x<0$ |
| 10 | Angle mode for trig functions | Calculator in degree mode | Must use radian mode | Integration formulas are derived using radians |

---

### 🔧 Quick Self-Check List

Ask yourself these questions before solving a problem:

- [ ] Did I add the constant of integration $C$? (indefinite integrals)
- [ ] Did I omit $C$ for definite integrals?
- [ ] Did I check for the special case $n=-1$?
- [ ] Did I divide by $a$ for $(ax+b)^n$?
- [ ] Did I add a negative sign for $\sin$ integrals?
- [ ] For area problems, did I check whether the curve is above or below the $x$-axis?
- [ ] For area between two curves, did I confirm which one is above?
- [ ] Do I need to split the interval for piecewise handling?

> **Final advice**: After completing every integration, develop the habit of **verifying by differentiation**. This not only helps you find errors but also deepens your understanding of the core idea that "integration is the reverse operation of differentiation."

---

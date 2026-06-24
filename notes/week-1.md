---
title: "Week 1 Notes — Mathematics 1 for Data Science"
author: "Vishal (Instructor)"
layout: default
math: true
---

# Week 1 Notes
## Natural Numbers, Integers, Rationals & Real Numbers

**Course:** Mathematics 1 for Data Science  
**Prepared by:** Vishal (Instructor)

---

## Table of Contents

- [Lecture 1 — Natural Numbers & Their Operations](#lecture-1--natural-numbers--their-operations)
- [Lecture 2 — Rational Numbers](#lecture-2--rational-numbers)
- [Lecture 3 — Real & Complex Numbers](#lecture-3--real--complex-numbers)
- [Lecture 4 — Introduction to Sets](#lecture-4--introduction-to-sets)
- [Lecture 5 — Set Comprehension, Intervals & Set Operations](#lecture-5--set-comprehension-intervals--set-operations)
- [Lecture 5A — Set Comprehension: Examples & Practice](#lecture-5a--set-comprehension-examples--practice)
- [Lecture 5B — Set Operations & Counting with Venn Diagrams](#lecture-5b--set-operations--counting-with-venn-diagrams)
- [Lecture 6 — Relations](#lecture-6--relations)
- [Lecture 7 — Functions](#lecture-7--functions)
- [Lecture 7A — Relations as Tables & the Join Operation](#lecture-7a--relations-as-tables--the-join-operation)
- [Lecture 7B — Function Examples: Ranges & Growth](#lecture-7b--function-examples-ranges--growth)

---

## Lecture 1 — Natural Numbers & Their Operations

### 1. Numbers: Starting from the Basics

Numbers are abstract concepts used for counting. When we see 7 balls and 7 pencils, the number "7" captures what is common — the quantity.

> **Natural Numbers ℕ**
>
> **ℕ = {0, 1, 2, 3, 4, 5, …}**
>
> The natural numbers are the counting numbers, starting from 0.

> **Note:** Some textbooks define ℕ = {1, 2, 3, …} (excluding 0). To emphasise that 0 is included, we sometimes write ℕ₀.

Zero (of Indian origin) is arguably the most important number — without it, our place-value number system would not work.

---

### 2. Operations on Natural Numbers

The four basic operations: addition, subtraction, multiplication, division.

**Key question:** When we perform an operation on two natural numbers, do we always get a natural number back? This property is called **closure**.

| Operation | Closed in ℕ? | Why / Why not |
|-----------|:-----------:|----------------|
| Addition | ✓ | Sum of two naturals is always natural |
| Multiplication | ✓ | Product of two naturals is always natural |
| Subtraction | ✗ | 5 − 6 = −1 ∉ ℕ (goes below zero) |
| Division | ✗ | 7 ÷ 2 = 3.5 ∉ ℕ (not an integer) |

Subtraction failing closure motivates the extension to integers.

---

### 3. Integers ℤ

> **Integers**
>
> **ℤ = {…, −3, −2, −1, 0, 1, 2, 3, …}**
>
> The integers extend the natural numbers by adding negative numbers symmetrically around zero.

ℕ ⊂ ℤ — every natural number is an integer, but not vice versa.

**The Number Line**

```
←————————————————————————————————————→
−5  −4  −3  −2  −1   0   1   2   3   4   5
   Negative         Zero        Positive
                              Increasing →
```

Numbers increase from left to right. The integers extend to −∞ on the left and +∞ on the right.

---

### 4. Multiplication: Repeated Addition

> **Multiplication**
>
> M × N means: take M objects and make N copies of them.
>
> M × N = M + M + M + ⋯ + M  *(N times)*
>
> Multiplication is repeated addition.

**Example:** 7 × 4 = 7 + 7 + 7 + 7 = 28

**Notation:** M × N can also be written as M · N or simply MN (when using variable names, not digits).

#### Sign Rules for Multiplication

| Signs | Result | Example |
|-------|:------:|---------|
| (+) × (+) | + | 7 × 4 = 28 |
| (−) × (+) | − | (−7) × 4 = −28 |
| (+) × (−) | − | 7 × (−4) = −28 |
| (−) × (−) | + | (−7) × (−4) = 28 |

**Rule:** Even number of minus signs ⇒ positive. Odd number ⇒ negative.

---

### 5. Exponentiation: Repeated Multiplication

> **Exponentiation**
>
> Mᴷ = M × M × M × ⋯ × M  *(K times)*
>
> Exponentiation is repeated multiplication, just as multiplication is repeated addition.

| Notation | Means | Name | Geometric interpretation |
|----------|-------|------|--------------------------|
| M² | M × M | M squared | Area of an M × M square |
| M³ | M × M × M | M cubed | Volume of an M × M × M cube |
| Mᴷ | M multiplied K times | M to the power K | No geometric name for K > 3 |

**Hierarchy:** Addition →*(repeat)*→ Multiplication →*(repeat)*→ Exponentiation

---

### 6. Division: Repeated Subtraction

> **Division as Repeated Subtraction**
>
> To compute 20 ÷ 5: start with 20, keep subtracting 5 until you reach 0.
>
> 20 → 15 → 10 → 5 → 0  *(4 rounds)*
>
> So 20 ÷ 5 = 4.

If the subtraction doesn't reach exactly 0, what's left over is the **remainder**.

**Example with remainder:** 19 ÷ 5:

19 → 14 → 9 → 4  *(3 rounds, 4 left over)*

Quotient = 3, Remainder = 4.

---

### 7. The Modulus (Remainder) Operation

> **Modulus**
>
> `a mod b` = remainder when `a` is divided by `b`

**Examples:** `19 mod 5 = 4`,  `20 mod 5 = 0`,  `7 mod 3 = 1`

---

### 8. Divisibility and Factors

> **Divisibility**
>
> `a` divides `b` (written **a | b**) if `b mod a = 0` — that is, `a` goes into `b` with no remainder.
>
> Equivalently: `b = k · a` for some integer `k` (i.e., `b` is a multiple of `a`).
>
> **Notation:** `a | b` means "a divides b". `a ∤ b` means "a does not divide b".

**Examples:** `4 | 20` (because 4 × 5 = 20),  `7 | 63` (because 7 × 9 = 63),  `32 | 1024` (because 32 × 32 = 1024).

`4 ∤ 19`,  `9 ∤ 100`.

#### Factors Come in Pairs

If `a | b` and `b = k · a`, then `k` is also a factor of `b`. So factors come in **pairs** `(a, k)` where `a · k = b`.

**Example — Factors of 12:** (1, 12), (2, 6), (3, 4) — six factors total (even count).

**Exception — Perfect squares:** For 36 = 6 × 6, the pair (6, 6) contributes only one distinct factor. So 36 has an **odd** number of distinct factors: (1, 36), (2, 18), (3, 12), (4, 9), (6).

> **Rule:** Non-square integers have an **even** number of factors. Perfect squares have an **odd** number of factors.

---

### 9. Prime Numbers

> **Prime Number**
>
> A prime `p` is an integer greater than 1 with exactly **two** factors: 1 and `p` itself.

**Note:** 1 is not a prime (it has only one factor: itself). The smallest prime is 2.

**First few primes:** 2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, …

After 2, no even number can be prime (all even numbers are divisible by 2).

#### Sieve of Eratosthenes

An algorithm to find all primes up to N:

1. List all numbers from 2 to N.
2. The first unmarked number (2) is prime. Mark all its multiples as non-prime.
3. The next unmarked number (3) is prime. Mark all its multiples.
4. Repeat: the next unmarked number is always prime; mark its multiples.
5. Continue until all numbers are either marked prime or marked as multiples.

This systematically generates all primes up to N without missing any.

---

### 10. Prime Factorization (Fundamental Theorem of Arithmetic)

> **Unique Prime Factorization**
>
> Every integer n > 1 can be written as a product of prime numbers in **exactly one way** (up to the order of factors):
>
> n = p₁^a₁ · p₂^a₂ · p₃^a₃ ⋯ pₖ^aₖ
>
> where p₁ < p₂ < ⋯ < pₖ are distinct primes and aᵢ ≥ 1.

**Examples:**
- 12 = 2 × 2 × 3 = 2² × 3
- 126 = 2 × 3 × 3 × 7 = 2 × 3² × 7
- 1024 = 2¹⁰

Although 12 can be factored as 2 × 6 or 4 × 3 or 1 × 12, the prime factorization 2² × 3 is **unique**.

---

### 11. Summary

| Concept | Key Point |
|---------|-----------|
| ℕ = {0, 1, 2, …} | Natural numbers (counting, starts at 0) |
| ℤ = {…, −2, −1, 0, 1, 2, …} | Integers (naturals + negatives) |
| Multiplication | Repeated addition |
| Exponentiation | Repeated multiplication |
| Division | Repeated subtraction; quotient + remainder |
| `a mod b` | Remainder of a ÷ b |
| `a \| b` | a divides b (no remainder) |
| Factors | Come in pairs; odd count ⟺ perfect square |
| Prime p | Exactly 2 factors: 1 and p; smallest is 2 |
| Prime factorization | Every integer has a unique prime decomposition |

### 12. Key Takeaways

1. **Natural numbers** ℕ = {0, 1, 2, …} are for counting. **Integers** ℤ extend ℕ with negatives.
2. Subtraction is not closed in ℕ (can produce negatives), motivating the extension to ℤ.
3. **Hierarchy:** addition → multiplication (repeated addition) → exponentiation (repeated multiplication). Division is repeated subtraction.
4. The **modulus** `a mod b` gives the remainder. If the remainder is 0, then `a | b` (a divides b).
5. Factors come in **pairs**. Non-squares have even factor count; perfect squares have odd factor count.
6. **Primes** have exactly two factors (1 and themselves). 1 is not prime; 2 is the smallest prime.
7. The **Sieve of Eratosthenes** generates all primes up to N by iteratively marking multiples.
8. Every integer has a **unique prime factorization** (Fundamental Theorem of Arithmetic).

---

## Lecture 2 — Rational Numbers

### 1. Why Rational Numbers?

Division is not closed in ℤ: there is no integer k such that 5k = 19. To handle such cases, we extend integers to fractions.

**Example:** 19 ÷ 5 = 3⅘ — this is a rational number.

---

### 2. Definition of Rational Numbers ℚ

> **Rational Numbers**
>
> **ℚ = { p/q | p, q ∈ ℤ, q ≠ 0 }**
>
> A rational number is a ratio of two integers (hence the name "rational").

`p` is the **numerator** (top), `q` is the **denominator** (bottom).

**Hierarchy:** ℕ ⊂ ℤ ⊂ ℚ — every integer `n` is rational (write it as `n/1`).

---

### 3. Non-Unique Representation

Unlike integers (where 7 can only be written as 7), a rational number has many equivalent representations:

```
3/5 = 6/10 = 30/50 = 60/100 = ⋯
```

Multiplying both numerator and denominator by the same nonzero integer gives an equivalent fraction:

```
p/q = (p·k)/(q·k)   for any k ≠ 0
```

#### Why Non-Uniqueness Is Useful

**Addition:** To add fractions with different denominators, convert to a common denominator:

```
3/5 + 3/4 = 12/20 + 15/20 = 27/20
```

**Comparison:** To compare fractions, make denominators equal:

```
3/5 < 3/4  ⟺  12/20 < 15/20  ✓
```

The common denominator need not be the smallest common multiple — any common multiple works. For instance, using 100: 60/100 < 75/100 gives the same conclusion.

---

### 4. Reduced Form and GCD

> **Reduced (Canonical) Form**
>
> A fraction `p/q` is in **reduced form** if p and q share no common factor other than 1, i.e.:
>
> **gcd(p, q) = 1**
>
> To reduce a fraction: divide both numerator and denominator by their **greatest common divisor (GCD)**.

#### Finding the GCD via Prime Factorization

**Example:** Reduce 18/60.

- 18 = 2 × 3²
- 60 = 2² × 3 × 5
- Common prime factors: one 2 and one 3 ⇒ gcd(18, 60) = 2 × 3 = 6

```
18/60 = (18 ÷ 6)/(60 ÷ 6) = 3/10
```

Check: 3 = 3 × 1, 10 = 2 × 5. No common factors ⇒ reduced form. ✓

#### GCD Algorithm (via Prime Factorization)

1. Find the prime factorization of both numbers.
2. For each prime, take the **minimum** of the exponents from both factorizations.
3. Multiply these together ⇒ GCD.

> **Note:** This is intuitive but not the most efficient method. Euclid's algorithm is faster for large numbers.

---

### 5. Density of Rational Numbers

> **Rationals Are Dense**
>
> Between any two distinct rational numbers, there is always another rational number.
>
> **Proof:** Given m/n < p/q, their average ½(m/n + p/q) is also rational and lies strictly between them. Since you can repeat this process infinitely, there are infinitely many rationals between any two rationals.

#### Discrete vs. Dense

| Property | Integers ℤ | Rationals ℚ |
|----------|:----------:|:-----------:|
| "Next" element? | Yes (m + 1 follows m) | No |
| Gap between neighbours? | Yes (nothing between m and m+1) | No (always one in between) |
| Type | Discrete | Dense |

**Key contrast:** For integers, we can always say "the next one is m + 1" with nothing in between. For rationals, there is no such thing as "the next" rational number.

---

### 6. Summary

| Concept | Key Point |
|---------|-----------|
| ℚ = {p/q : p, q ∈ ℤ, q ≠ 0} | Rationals = ratios of integers |
| Non-unique representation | 3/5 = 6/10 = 30/50 = ⋯ |
| Common denominator | Needed for addition and comparison |
| Reduced form | gcd(p, q) = 1; use prime factorization |
| gcd(18, 60) = 6 | Common primes: 2 × 3 = 6 |
| Dense | Always a rational between any two rationals |
| Discrete vs. dense | ℤ is discrete, ℚ is dense |

### 7. Key Takeaways

1. Division not being closed in ℤ motivates the extension to rational numbers ℚ = {p/q}.
2. Rational numbers have non-unique representations (p/q = pk/qk). This is useful for finding common denominators.
3. Addition and comparison of fractions require a common denominator (any common multiple of the two denominators works).
4. The reduced form (canonical representation) has gcd(p, q) = 1. Find the GCD via prime factorization and divide both numerator and denominator.
5. Rationals are **dense**: between any two rationals there is always another (take their average). There is no "next" rational number.
6. Integers are **discrete**: m + 1 is the next integer after m, with nothing in between.
7. **Number system hierarchy:** ℕ ⊂ ℤ ⊂ ℚ — each extension fixes a closure failure (subtraction, then division).

---

## Lecture 3 — Real & Complex Numbers

### 1. Do Rationals Fill the Number Line?

The rationals ℚ are dense — between any two rationals there is another rational. Does this mean all points on the number line are rational?

**No.** There are "gaps" in ℚ that only become visible when we consider operations like the square root.

---

### 2. Square Roots and Perfect Squares

> **Square Root**
>
> The square root of M is the number r such that r × r = M.

For perfect squares (1, 4, 9, 16, 25, …), the square root is an integer:

```
√1 = 1,  √4 = 2,  √9 = 3,  √16 = 4,  √25 = 5,  √256 = 16
```

**Question:** What about √M when M is not a perfect square?

**Example:** √10 lies between 3 and 4 (since 3² = 9 and 4² = 16). Is it rational?

---

### 3. Irrational Numbers

> **√2 Is Irrational**
>
> √2 cannot be written as p/q for any integers p and q.
>
> Yet √2 is a perfectly real, measurable quantity: by Pythagoras's theorem, the diagonal of a unit square has length √(1² + 1²) = √2.

So √2 is on the number line but is not rational — it is an **irrational number**.

**General rule:** For any integer M that is not a perfect square, √M is irrational. This includes √2, √3, √5, √6, √7, √8, √10, …

---

### 4. Famous Irrational Numbers

| Number | Approx. value | Where it appears |
|--------|:-------------:|-----------------|
| π | 3.14159265… | Ratio of circumference to diameter of any circle |
| e | 2.71828182… | Base of natural logarithms |
| √2 | 1.41421356… | Diagonal of a unit square |

All three have infinite, non-repeating decimal expansions (a hallmark of irrational numbers).

---

### 5. Real Numbers ℝ

> **Real Numbers**
>
> **ℝ = Rational numbers ∪ Irrational numbers**
>
> The real numbers ℝ include every point on the number line — all rationals and all irrationals.

**Density:** Like ℚ, the real numbers are dense. Between any two reals r and r′ (r < r′), the average (r + r′)/2 is a real number strictly between them.

---

### 6. Complex Numbers (Preview)

**Why do we need yet more numbers?**

**Problem:** √(−1) has no real solution. By the sign rule for multiplication, any number multiplied by itself gives a positive result — so no real number squared gives −1.

**Solution:** Define a new number **i = √(−1)** and build the **complex numbers ℂ**, which extend ℝ.

*(Complex numbers are not needed for this course.)*

---

### 7. The Complete Number System Hierarchy

```
ℕ ⊂ ℤ ⊂ ℚ ⊂ ℝ ⊂ ℂ
```

| Step | What was added | Operation that was failing |
|------|---------------|---------------------------|
| ℕ → ℤ | Negative numbers | Subtraction not closed in ℕ |
| ℤ → ℚ | Fractions | Division not closed in ℤ |
| ℚ → ℝ | Irrational numbers | Square roots of non-squares |
| ℝ → ℂ | Imaginary numbers | Square roots of negatives |

#### Discrete vs. Dense

| Number system | Type | "Next" exists? |
|:-------------:|:----:|:--------------:|
| ℕ (naturals) | Discrete | Yes (n + 1) |
| ℤ (integers) | Discrete | Yes (m + 1) |
| ℚ (rationals) | Dense | No (take average) |
| ℝ (reals) | Dense | No (take average) |

---

### 8. Key Takeaways

1. **Irrational numbers** are real numbers that cannot be written as p/q. Examples: √2, √3, π, e.
2. √M is irrational for every non-perfect-square integer M.
3. √2 is geometrically real (diagonal of a unit square) but algebraically not rational.
4. **ℝ = ℚ ∪ {irrationals}** — the real numbers fill the entire number line.
5. Real numbers are dense (same argument as rationals: take the average).
6. **Complex numbers ℂ** extend ℝ to allow √(−1), but are not needed for this course.
7. **Complete hierarchy:** ℕ ⊂ ℤ ⊂ ℚ ⊂ ℝ ⊂ ℂ. Each extension fixes a missing operation.

---

## Lecture 4 — Introduction to Sets

### 1. What Is a Set?

A **set** is a collection of items (called **elements** or **members**). Sets are written with curly braces, elements separated by commas.

**Examples:**
- Days of the week: {Sun, Mon, Tue, Wed, Thu, Fri, Sat} — 7 elements
- Factors of 24: {1, 2, 3, 4, 6, 8, 12, 24} — 8 elements
- Primes below 15: {2, 3, 5, 7, 11, 13} — 6 elements
- ℕ, ℤ, ℚ, ℝ — all infinite sets of numbers

**Key properties of sets:**
- **No ordering:** {Kohli, Dhoni, Pujara} = {Pujara, Kohli, Dhoni}
- **No duplicates:** Adding Kohli a second time does not change the set.
- **Mixed types allowed:** A set can contain people, instruments, animals, numbers — anything.

---

### 2. Notation: Element Of (∈)

> **Membership**
>
> `x ∈ X` means "x is an element of set X"
>
> `x ∉ X` means "x is not an element of set X"
>
> **Examples:** 0 ∈ ℕ,  5 ∈ ℤ,  √2 ∉ ℚ

---

### 3. Cardinality

The **cardinality** of a set is the number of elements it contains, written |X|.

For finite sets, just count. For infinite sets, measuring cardinality is more subtle (a separate topic).

**Examples:** |{factors of 24}| = 8,  |ℕ| = ∞

#### Surprising Finite Sets: Platonic Solids

Regular polygons (2D) are infinite in number (triangle, square, pentagon, … for any number of sides). But their 3D counterparts — **Platonic solids** (where every face is an identical regular polygon meeting at equal angles) — number exactly **5**:

| Solid | Faces | Face shape |
|-------|:-----:|:----------:|
| Tetrahedron | 4 | Triangle |
| Cube | 6 | Square |
| Octahedron | 8 | Triangle |
| Dodecahedron | 12 | Pentagon |
| Icosahedron | 20 | Triangle |

---

### 4. Subsets

> **Subset**
>
> `X ⊆ Y` means every element of X is also an element of Y.
>
> **Proper subset:** `X ⊂ Y` means X ⊆ Y and X ≠ Y.

**Examples:**
- {Kohli, Pujara} ⊂ {Kohli, Dhoni, Pujara}
- Primes ⊂ ℕ (not all naturals are prime)
- ℕ ⊂ ℤ ⊂ ℚ ⊂ ℝ (proper subsets at each level)

**Two important facts:**
1. Every set is a subset of itself: X ⊆ X (trivially, every element of X is in X).
2. **Set equality:** X = Y if and only if X ⊆ Y *and* Y ⊆ X.

#### Venn Diagrams

Sets and subset relationships are visualised using **Venn diagrams** — circles where one circle inside another indicates a subset:

```
┌──────────────────── ℝ ────────────────────┐
│  ┌─────────────── ℚ ───────────────┐      │
│  │  ┌────────── ℤ ──────────┐      │      │
│  │  │  ┌────── ℕ ──────┐   │      │      │
│  │  │  │               │   │      │      │
│  │  │  └───────────────┘   │      │      │
│  │  └──────────────────────┘      │      │
│  └─────────────────────────────────┘      │
└────────────────────────────────────────────┘
```

---

### 5. The Empty Set

> **Empty Set ∅**
>
> The empty set **∅** is the set with no elements. It is the "zero" of set theory.
>
> **∅ is a subset of every set:** ∅ ⊆ X for all X.
>
> **Why?** The statement "every element of ∅ is in X" is *vacuously true* — there are no elements to contradict it. (Like saying "all 3-legged birds have pink beaks" — true because no 3-legged birds exist.)

**Important distinction:** ∅ ≠ {∅}
- ∅ has **0** elements.
- {∅} has **1** element (namely, the empty set itself).

---

### 6. Power Set

> **Power Set**
>
> The power set of X, written **𝒫(X)** or **2^X**, is the set of all subsets of X.
>
> If |X| = n, then **|𝒫(X)| = 2ⁿ**

**Example:** X = {a, b}. Subsets: ∅, {a}, {b}, {a, b}. So 𝒫(X) = {∅, {a}, {b}, {a, b}}, with |𝒫(X)| = 2² = 4.

𝒫(∅) = {∅} (one element: the empty set itself). |𝒫(∅)| = 2⁰ = 1.

#### Why 2ⁿ Subsets?

**Argument 1 (Choices):** For each of the n elements, choose to include or exclude it from the subset. That gives 2 × 2 × ⋯ × 2 = **2ⁿ** possible subsets.

**Argument 2 (Binary numbers):** Each subset corresponds to an n-bit binary string, where bit i is 1 if xᵢ is included, 0 if excluded.

**Example:** X = {a, b, c, d}. The binary string `0110` means: exclude a, include b, include c, exclude d → subset {b, c}.

| Binary | Decimal | Subset of {a, b, c, d} |
|:------:|:-------:|:----------------------:|
| 0000 | 0 | ∅ |
| 0001 | 1 | {d} |
| 0101 | 5 | {b, d} |
| 1111 | 15 | {a, b, c, d} |

There are exactly 2⁴ = 16 four-bit binary numbers (0000 to 1111), so exactly 16 subsets.

---

### 7. A Note on Russell's Paradox

Can we collect all sets into one "set of all sets"? Bertrand Russell showed this leads to a contradiction (**Russell's Paradox**). In practice, for the collections of numbers and objects we use in this course, this is not a concern.

---

### 8. Key Takeaways

1. A **set** is an unordered collection of distinct elements. Notation: {a, b, c}.
2. `x ∈ X` means x belongs to X; `x ∉ X` means it does not.
3. **Cardinality** |X| = number of elements. Can be finite or infinite.
4. `X ⊆ Y` (subset): every element of X is in Y. `X ⊂ Y` (proper subset): X ⊆ Y and X ≠ Y.
5. X = Y iff X ⊆ Y and Y ⊆ X.
6. The **empty set ∅** has no elements and is a subset of every set (vacuous truth).
7. ∅ ≠ {∅}: the first has 0 elements, the second has 1.
8. The **power set** 𝒫(X) contains all subsets of X. If |X| = n, then |𝒫(X)| = 2ⁿ.
9. The 2ⁿ count follows from: each element has 2 choices (include/exclude), or equivalently, subsets biject with n-bit binary strings.

---

## Lecture 5 — Set Comprehension, Intervals & Set Operations

### 1. Set Comprehension: Defining Subsets of Infinite Sets

We cannot list all elements of an infinite set. Instead, we describe subsets using a condition applied to a known set — this is called **set comprehension**.

> **Set Comprehension Notation**
>
> `{ x ∈ S | condition on x }`
>
> Read as: "the set of all x in S such that [condition] holds."

**Three parts:**
1. **Starting set S** (e.g., ℤ, ℕ, ℝ) — we must begin from a known set.
2. **Condition** (the filter) — decides which elements to keep.
3. **Collector** `{x | …}` — gathers all elements satisfying the condition.

**Examples:**

Even integers:
```
{ x ∈ ℤ | x mod 2 = 0 }
```
Take all integers, keep only those divisible by 2.

Perfect squares:
```
{ m ∈ ℕ | √m ∈ ℕ }
```
Take all natural numbers, keep only those whose square root is also a natural number. Gives {1, 4, 9, 16, 25, …}.

Rationals in reduced form:
```
{ p/q | p, q ∈ ℤ, q ≠ 0, gcd(p, q) = 1 }
```
Keep only fractions where numerator and denominator share no common factor other than 1.

---

### 2. Intervals: Subsets of ℝ

Intervals describe ranges of real numbers between two endpoints. They are defined using set comprehension with inequality conditions.

#### Four Types of Intervals

| Name | Notation | Endpoints | Definition |
|------|:--------:|:---------:|------------|
| Closed | [a, b] | Both included | { r ∈ ℝ \| a ≤ r ≤ b } |
| Open | (a, b) | Both excluded | { r ∈ ℝ \| a < r < b } |
| Left-open | (a, b] | Left excluded | { r ∈ ℝ \| a < r ≤ b } |
| Right-open | [a, b) | Right excluded | { r ∈ ℝ \| a ≤ r < b } |

**Convention:** Square bracket `[ ]` = endpoint included. Round bracket `( )` = endpoint excluded.

#### Visualising on the Number Line

```
[0, 1]:   ●————————————●
          0            1

(0, 1):   ○············○
          0            1

(0, 1]:   ○············●
          0            1
```
*(Filled circle = included. Open circle = excluded.)*

> **Practical importance:** The interval [0, 1] (or (0, 1)) appears frequently in probability, where values range from 0 to 1.

---

### 3. Set Operations

#### Union (∪)

> **Union**
>
> `X ∪ Y` = all elements in X **or** Y (or both). Duplicates appear only once.
>
> `{a, b, c} ∪ {c, d, e} = {a, b, c, d, e}`
>
> Note: |X ∪ Y| ≤ |X| + |Y| (equality only if X and Y share no elements).
>
> Union is **commutative:** X ∪ Y = Y ∪ X.

#### Intersection (∩)

> **Intersection**
>
> `X ∩ Y` = all elements in **both** X and Y.
>
> `{a, b, c, d} ∩ {a, d, e, f} = {a, d}`
>
> Intersection is **commutative:** X ∩ Y = Y ∩ X.

#### Set Difference (\)

> **Set Difference**
>
> `X \ Y` (or X − Y) = all elements in X that are **not** in Y.
>
> `{a, b, c, d} \ {a, d, e, f} = {b, c}`
>
> `{a, d, e, f} \ {a, b, c, d} = {e, f}` *(different!)*
>
> Set difference is **not commutative:** X \ Y ≠ Y \ X in general.

**Examples:** ℝ \ ℚ = all irrational numbers.  ℚ \ ℤ = all non-integer rationals.

#### Complement (X̄ or Xᶜ)

> **Complement**
>
> The complement of X is everything *not* in X — relative to a specified **universe U**:
>
> X̄ = U \ X
>
> **Example:** Primes ⊂ ℕ. If U = ℕ, then the complement of the primes = composite numbers ∪ {0, 1}. If U = ℝ, the complement would also include π, e, √2, … — not what we intend!
>
> **Rule:** Always specify the universe when using complement.

---

### 4. Summary of Set Operations

| Operation | Symbol | Commutative? | Result |
|-----------|:------:|:------------:|--------|
| Union | X ∪ Y | ✓ | Elements in X or Y |
| Intersection | X ∩ Y | ✓ | Elements in both X and Y |
| Set difference | X \ Y | ✗ | Elements in X but not Y |
| Complement | X̄ | N/A | U \ X (needs universe U) |

---

### 5. Key Takeaways

1. **Set comprehension** `{x ∈ S | condition}` defines subsets of infinite sets by specifying a starting set and a filter condition.
2. Examples: even integers (`x mod 2 = 0`), perfect squares (`√m ∈ ℕ`), rationals in reduced form (`gcd(p, q) = 1`).
3. **Intervals** are subsets of ℝ between two endpoints. Square bracket = included, round bracket = excluded. Four types: [a, b], (a, b), (a, b], [a, b).
4. **Union (∪):** combines elements from both sets; commutative.
5. **Intersection (∩):** keeps only common elements; commutative.
6. **Set difference (\ ):** removes elements of the second set from the first; not commutative.
7. **Complement:** everything not in X, relative to a specified universe U. Always state the universe.

---

## Lecture 5A — Set Comprehension: Examples & Practice

### 1. Quick Review

- **Membership:** x ∈ X (element belongs to set). **Subset:** X ⊆ Y (every element of X is in Y).
- **Empty set** ∅ is a subset of every set. Every set is a subset of itself.
- **Power set:** |𝒫(X)| = 2^|X|.
- **Set comprehension:** `{f(x) | x ∈ S, condition(x)}` builds new sets from old ones.

---

### 2. Anatomy of Set Comprehension

> **Three Components**
>
> ```
> {   x²    |   x ∈ ℤ   ,   x mod 2 = 0   }
>  Transform    Generator       Filter
> ```
>
> 1. **Generator** — draws elements from an existing set (x ∈ ℤ)
> 2. **Filter** — keeps only elements satisfying a condition (x is even)
> 3. **Transform** — converts the surviving elements into the final output (x → x²)
>
> If no filter is needed, omit it. If no transform is needed, just keep x as-is (identity).

#### Worked Example: Squares of Even Integers

`{ x² | x ∈ ℤ, x mod 2 = 0 }`

**Step 1 (Generate):** All integers: …, −3, −2, −1, 0, 1, 2, 3, …

**Step 2 (Filter):** Keep only even: …, −4, −2, 0, 2, 4, …

**Step 3 (Transform):** Square each: (−4)² = 16, (−2)² = 4, 0² = 0, 2² = 4, 4² = 16, …

**Step 4 (Remove duplicates):** (−2)² = 2² = 4, so keep only one copy.

**Result:** {0, 4, 16, 36, 64, …}

---

### 3. Examples with Identity Transform

When the transform is just "keep as-is," we write x on the left side.

**Rationals in reduced form:**
```
{ p/q | p/q ∈ ℚ, gcd(p, q) = 1 }
```
Generator: all rationals. Filter: gcd = 1. Transform: identity (keep p/q as-is).

**Half-open interval [−1, 2):**
```
{ r ∈ ℝ | −1 ≤ r < 2 }
```
Generator: all reals. Filter: between −1 (included) and 2 (excluded). Transform: identity.

---

### 4. Replacing a Long List with Set Comprehension

**Task:** Cubes of the first 500 natural numbers.

- **Tedious way:** {0³, 1³, 2³, …, 499³} — must list all 500 numbers explicitly.
- **Compact way using set comprehension:**
  - Define: X = {n ∈ ℕ | n < 500}
  - Then: {n³ | n ∈ X}

This is readable, precise, and avoids the informal "…" notation.

---

### 5. Multiple Ways to Define the Same Set

#### Perfect Squares: Three Equivalent Definitions

**Version 1** (Filter on integers):
```
{ z ∈ ℤ | √z ∈ ℤ }
```
Generate all integers, keep those whose square root is also an integer.

**Version 2** (Filter on naturals):
```
{ m ∈ ℕ | √m ∈ ℕ }
```
Since squares are always ≥ 0, we can restrict to ℕ instead of ℤ.

**Version 3** (Transform, no filter):
```
{ n² | n ∈ ℕ }
```
Generate all naturals, square each one. No filter needed — every natural squared is a perfect square.

All three produce the same set: **{0, 1, 4, 9, 16, 25, …}**

> **Key insight:** A filter in one formulation can become a transform in another. The generator set matters — changing from ℤ to ℕ is valid here because squares are non-negative.

---

### 6. Extending to Other Number Systems

The concept of "perfect square" extends beyond integers:

**Rational perfect squares:**
```
{ q² | q ∈ ℚ }    e.g., (3/4)² = 9/16
```

Not every rational is a perfect square in ℚ. For example, 1/2 is not, because √(1/2) = 1/√2 is irrational.

> **Lesson:** The same set comprehension structure applies across different number systems — just change the generator set. But the resulting sets will differ depending on the domain.

---

### 7. Key Takeaways

1. Set comprehension has three parts: **generator** (source set), **filter** (condition), and **transform** (output function).
2. The transform can produce duplicates (e.g., (−2)² = 2²), which are automatically removed (sets have no duplicates).
3. If no transform is needed, use the **identity** (keep the element as-is).
4. Set comprehension replaces tedious explicit listings with compact, precise descriptions — essential for infinite sets.
5. The same set can often be defined in multiple equivalent ways by swapping filters and transforms or changing the generator.
6. Perfect squares can be defined either by **filtering** (keep if √m ∈ ℕ) or by **transforming** (square every n ∈ ℕ).
7. Changing the generator (e.g., ℤ → ℚ) extends the concept to other number systems, but the resulting set changes.

---

## Lecture 5B — Set Operations & Counting with Venn Diagrams

### 1. Recap: Set Operations via Venn Diagrams

| Operation | Symbol | Venn diagram region |
|-----------|:------:|---------------------|
| Union | X ∪ Y | Entire shaded area (both circles) |
| Intersection | X ∩ Y | Overlapping region only |
| Set difference | X \ Y | Left circle minus overlap |
| Complement | X̄ | Everything outside X (needs universe) |

---

### 2. The Four Disjoint Regions

When two sets P and B overlap within a universe U, the Venn diagram creates **four disjoint regions** that together account for every element:

```
┌──────────────── Universe U ─────────────────┐
│                                              │
│    ┌──────────────┐   ┌──────────────┐      │
│    │              │   │              │      │
│    │    P \ B     │P∩B│    B \ P     │      │
│    │              │   │              │      │
│    └──────────────┘   └──────────────┘      │
│                                    (P∪B)ᶜ  │
└──────────────────────────────────────────────┘
```

**|U| = |P \ B| + |P ∩ B| + |B \ P| + |(P ∪ B)ᶜ|**

These four regions are **mutually exclusive** (no element appears in two regions) and **exhaustive** (every element of U is in exactly one region).

---

### 3. Counting Problems with Venn Diagrams

#### Problem 1: Find the Total

> **Problem:** In a class: 30 students took Physics, 25 took Biology, 10 took both, 5 took neither. How many students are in the class?

**Solution:**

| Region | Calculation | Count |
|--------|------------|:-----:|
| P ∩ B (both) | given | 10 |
| P \ B (Physics only) | 30 − 10 | 20 |
| B \ P (Biology only) | 25 − 10 | 15 |
| (P ∪ B)ᶜ (neither) | given | 5 |
| **Total \|U\|** | 20 + 10 + 15 + 5 | **50** |

---

#### Problem 2: Find a Missing Region

> **Problem:** Class has 55 students. 32 took Physics, 11 took both Physics and Biology, 7 took neither. How many took Biology but not Physics?

**Solution:**
- |P ∩ B| = 11
- |P \ B| = 32 − 11 = 21
- |(P ∪ B)ᶜ| = 7
- Let |B \ P| = x

```
7 + 21 + 11 + x = 55  ⟹  x = 16
```

**16 students took Biology but not Physics.**

---

#### Problem 3: Find the Intersection

> **Problem:** Class has 60 students. 35 took Physics, 30 took Biology, 10 took neither. How many took both?

**Solution:**

Students taking at least one subject: |P ∪ B| = 60 − 10 = 50.

If there were no overlap, the total would be |P| + |B| = 35 + 30 = 65. But only 50 spots exist, so 65 − 50 = 15 students were **double-counted** (they take both).

```
|P ∩ B| = |P| + |B| − |P ∪ B| = 35 + 30 − 50 = 15
```

**Verification:** |P \ B| = 35 − 15 = 20,  |B \ P| = 30 − 15 = 15.  Total: 20 + 15 + 15 + 10 = 60. ✓

---

### 4. The Inclusion-Exclusion Principle

> **Inclusion-Exclusion (Two Sets)**
>
> **|A ∪ B| = |A| + |B| − |A ∩ B|**
>
> When we add |A| and |B|, elements in both sets are counted twice. Subtracting |A ∩ B| corrects for the double-counting.
>
> This formula connects all four quantities: |A|, |B|, |A ∪ B|, |A ∩ B|. Given any three, solve for the fourth.

---

### 5. Summary of the Week

| Topic | Lecture |
|-------|:-------:|
| Natural numbers, integers, operations, primes | L1 |
| Rational numbers, GCD, reduced form, density | L2 |
| Irrational numbers, reals, hierarchy ℕ ⊂ ℤ ⊂ ℚ ⊂ ℝ | L3 |
| Sets, subsets, cardinality, power set (2ⁿ) | L4 |
| Set comprehension, intervals, set operations | L5 |
| Set comprehension examples (generator/filter/transform) | L5A |
| Venn diagram counting, inclusion-exclusion | L5B |

---

### 6. Key Takeaways

1. A Venn diagram for two overlapping sets creates four disjoint regions: P \ B, P ∩ B, B \ P, and (P ∪ B)ᶜ.
2. The total is the sum of all four regions: |U| = |P \ B| + |P ∩ B| + |B \ P| + |(P ∪ B)ᶜ|.
3. Three problem types: find the total, find a missing region, find the intersection — all solved by populating the four regions and using the total equation.
4. The **inclusion-exclusion principle:** |A ∪ B| = |A| + |B| − |A ∩ B| corrects for double-counting.
5. Venn diagrams are not just illustrations — they are **computational tools** for solving counting problems systematically.

---

## Lecture 6 — Relations
### Cartesian Products, Properties & Equivalence Relations

### 1. Cartesian Product

> **Cartesian Product**
>
> The Cartesian product **A × B** is the set of all ordered pairs (a, b) where a ∈ A and b ∈ B:
>
> **A × B = { (a, b) | a ∈ A, b ∈ B }**
>
> Order matters: (0, 1) ≠ (1, 0).
>
> **|A × B| = |A| · |B|**

**Example:** A = {0, 1}, B = {2, 3}:

```
A × B = {(0, 2), (0, 3), (1, 2), (1, 3)},  |A × B| = 4
```

**Visualisation:** For number sets like ℕ × ℕ or ℝ × ℝ, the product is a grid or plane. Each pair (a, b) is a point with x-coordinate a and y-coordinate b.

#### Extension to n-tuples

The product extends to any number of sets: A₁ × A₂ × ⋯ × Aₙ produces n-tuples (a₁, a₂, …, aₙ).

**Example — Pythagorean triples:** (a, b, c) ∈ ℕ × ℕ × ℕ such that a, b, c > 0 and a² + b² = c².  E.g., (3, 4, 5), (5, 12, 13), (8, 15, 17).

---

### 2. Relations

> **Binary Relation**
>
> A relation R on sets A and B is a subset of A × B:
>
> **R ⊆ A × B**
>
> If (a, b) ∈ R, we say "a is related to b" and write aRb.
>
> A relation = Cartesian product + set comprehension (filter out the pairs of interest).

**Examples of Relations:**

- **Successor on ℕ:** {(m, n) ∈ ℕ × ℕ | n = m + 1} = {(0,1), (1,2), (17,18), …}
- **Divisibility on ℕ:** {(d, n) ∈ ℕ × ℕ | d | n} — e.g., (2, 82), (14, 56)
- **Circle of radius 5:** {(a, b) ∈ ℝ × ℝ | a² + b² = 25} — all points at distance 5 from the origin
- **Teacher–course allocation:** A ⊆ T × C where T = teachers, C = courses; (t, c) ∈ A means teacher t teaches course c
- **Mother–child:** {(m, c) ∈ P × P | m is the mother of c} where P is a set of people

---

### 3. The Identity Relation

```
Iₐ = { (a, a) | a ∈ A }
```

Every element is paired with itself. On ℕ × ℕ, this is the diagonal: (0,0), (1,1), (2,2), …

---

### 4. Properties of Binary Relations

For a relation R ⊆ A × A (both elements from the same set):

| Property | Definition | Example |
|----------|-----------|---------|
| **Reflexive** | (a, a) ∈ R for all a | Divisibility: a \| a ✓ |
| **Symmetric** | (a, b) ∈ R ⇒ (b, a) ∈ R | gcd(a, b) = 1: order doesn't matter ✓ |
| **Transitive** | (a,b) ∈ R and (b,c) ∈ R ⇒ (a,c) ∈ R | <: if 3 < 10 and 10 < 28 then 3 < 28 ✓ |
| **Antisymmetric** | (a,b) ∈ R and a ≠ b ⇒ (b,a) ∉ R | <: if a < b then b ≮ a ✓ |

> **Note:** Antisymmetry ≠ "not symmetric." Antisymmetry says: if a pair is present, the reverse must be absent (for distinct elements). It does not require every pair to be present.

---

### 5. Equivalence Relations

> **Equivalence Relation**
>
> A relation R is an **equivalence relation** if it is simultaneously:
> 1. **Reflexive:** aRa for all a.
> 2. **Symmetric:** aRb ⇒ bRa.
> 3. **Transitive:** aRb and bRc ⇒ aRc.
>
> An equivalence relation behaves like **equality**: it groups elements that are "the same" in some sense.

#### Example: Integers Modulo 5

Define a ∼ b iff (b − a) mod 5 = 0 (i.e., a and b differ by a multiple of 5).

**Checking the properties:**
- **Reflexive:** (a − a) = 0, and 0 mod 5 = 0. ✓
- **Symmetric:** if (b − a) mod 5 = 0, then (a − b) mod 5 = 0. ✓
- **Transitive:** if b − a and c − b are multiples of 5, so is c − a = (c − b) + (b − a). ✓

---

### 6. Equivalence Classes and Partitions

> **Key Result**
>
> Every equivalence relation **partitions** the set into disjoint **equivalence classes**:
> - All elements within a class are equivalent to each other.
> - No element belongs to two different classes.
> - The classes together cover the entire set.

**Example:** ℤ mod 5 partitions the integers into 5 classes:

| Remainder | Class members |
|:---------:|--------------|
| 0 | …, −10, −5, 0, 5, 10, 15, … |
| 1 | …, −9, −4, 1, 6, 11, 16, … |
| 2 | …, −8, −3, 2, 7, 12, 17, … |
| 3 | …, −7, −2, 3, 8, 13, 18, … |
| 4 | …, −6, −1, 4, 9, 14, 19, … |

**Real-world example:** A 12-hour clock partitions 24 hours into 2 equivalence classes (AM/PM). 2:00 AM and 2:00 PM look the same on the clock — they are "equivalent mod 12."

---

### 7. Key Takeaways

1. The **Cartesian product** A × B is the set of all ordered pairs (a, b). Order matters. |A × B| = |A| · |B|.
2. A **relation** R ⊆ A × B is a subset of the Cartesian product — selected pairs satisfying some condition.
3. Relations model geometric shapes (circles), allocations (teacher–course), family ties, divisibility, and more.
4. Extends to n-tuples: Pythagorean triples, square corners, etc.
5. Four key properties: **reflexive** (aRa), **symmetric** (aRb ⇒ bRa), **transitive** (chain rule), **antisymmetric** (no reverse pairs for distinct elements).
6. An **equivalence relation** (reflexive + symmetric + transitive) partitions a set into disjoint equivalence classes that behave like equality.
7. Example: ℤ mod 5 creates 5 equivalence classes based on remainder. A 12-hour clock is mod 12 equivalence.

---

## Lecture 7 — Functions
### Domain, Codomain, Range & Properties of Mappings

### 1. What Is a Function?

> **Function**
>
> A function is a rule that assigns to each input **exactly one** output.
>
> **Notation:** f : X → Y means f maps elements of the **domain** X to the **codomain** Y.
>
> For a specific input: x ↦ f(x).  Example: sq(x) = x².
>
> **Two requirements:**
> 1. **Defined everywhere:** For every x ∈ X, there exists a y such that f(x) = y.
> 2. **Unique output:** For each x, there is exactly one y = f(x).

---

### 2. Domain, Codomain, and Range

| Set | Definition | Example: f(x) = x², f : ℝ → ℝ |
|-----|-----------|--------------------------------|
| **Domain** | Set of all valid inputs | ℝ (all reals) |
| **Codomain** | Set of *possible* outputs | ℝ (all reals) |
| **Range** | Set of *actual* outputs | [0, ∞) = {r ∈ ℝ \| r ≥ 0} |

**Key:** Range ⊆ Codomain. They may or may not be equal.

---

### 3. Functions as Relations

Every function f : X → Y defines a relation:

```
Rƒ = { (x, y) ∈ X × Y | y = f(x) }
```

Plotting a function = plotting the relation Rƒ. The graph of f(x) = x² is the set of all points (x, x²) — the parabola.

**What distinguishes a function from a general relation:**
- Every x in the domain has *at least one* pair (function is defined everywhere).
- Every x has *at most one* pair (output is unique).

---

### 4. Examples of Functions

**Linear function:** f(x) = mx + c
- m = **slope** (angle/steepness),  c = **intercept** (where line crosses y-axis)
- Same slope, different intercept ⇒ parallel lines
- Negative slope ⇒ line goes downward
- Domain = ℝ, Codomain = ℝ, Range = ℝ (line spans all values)

**Square root:** f(x) = √x
- By convention, √x means the **positive** square root.
- If we took both +√x and −√x, the output would not be unique ⇒ not a function!
- Domain depends on codomain: if codomain = ℝ, then domain = [0, ∞). If codomain = ℂ, domain can be all of ℝ.

---

### 5. Properties of Functions

#### Injective (One-to-One)

> **Injective**
>
> f is **injective** if distinct inputs always produce distinct outputs:
>
> x₁ ≠ x₂  ⟹  f(x₁) ≠ f(x₂)
>
> - **Injective:** f(x) = 3.5x + 5.7 (different x → different point on the line). ✓
> - **Not injective:** f(x) = x² (because f(a) = f(−a) for all a). ✗

#### Surjective (Onto)

> **Surjective**
>
> f is **surjective** if every element of the codomain is actually hit:
>
> Range = Codomain  ⟺  ∀y ∈ Y, ∃x ∈ X : f(x) = y
>
> - **Surjective:** f(x) = mx + c with f : ℝ → ℝ (line spans all reals). ✓
> - **Not surjective:** f(x) = 5x² + 3 with codomain ℝ (range = [3, ∞) ≠ ℝ). ✗
> - **Not surjective:** f(x) = 7√x with codomain ℝ (only non-negative outputs). ✗

#### Bijective (One-to-One and Onto)

> **Bijective = Injective + Surjective**
>
> f is **bijective** if it is both injective and surjective:
> - Every input maps to a **distinct** output (injective).
> - Every output has a **unique** input that maps to it (surjective).
>
> A bijection establishes a **one-to-one correspondence** between domain and codomain.
>
> **Theorem:** f is bijective  ⟺  f is injective *and* surjective.

**Example:** f(x) = 3.5x + 5.7 with f : ℝ → ℝ is bijective.

---

### 6. Summary of Function Properties

| Function | Injective? | Surjective? | Bijective? |
|----------|:----------:|:-----------:|:----------:|
| f(x) = mx + c,  f : ℝ → ℝ | ✓ | ✓ | ✓ |
| f(x) = x²,  f : ℝ → ℝ | ✗ | ✗ | ✗ |
| f(x) = √x,  f : [0,∞) → ℝ | ✓ | ✗ | ✗ |
| f(x) = √x,  f : [0,∞) → [0,∞) | ✓ | ✓ | ✓ |

> **Note:** Whether a function is surjective (and hence bijective) depends on the choice of **codomain**!

---

### 7. Bijections and Cardinality

> **Bijections for Counting**
>
> Two sets A and B have the same cardinality (|A| = |B|) if and only if there exists a bijection f : A → B.
>
> - For **finite sets:** this is a convenience (like pairing marbles from two sacks one-by-one; both sacks empty together ⇒ same count).
> - For **infinite sets:** this is the *only* way to compare cardinalities.

**Example:** Every line y = mx + c is uniquely determined by the pair (m, c) ∈ ℝ × ℝ. This defines a bijection between lines and points in ℝ². Therefore, the number of lines equals the number of points on the plane.

> **Caution:** Two points determine a unique line, but many pairs of points determine the same line. So the map from pairs-of-points to lines is not injective — you cannot conclude |ℝ² × ℝ²| = |ℝ²| from this.

---

### 8. Key Takeaways

1. A function assigns **exactly one** output to each input. Notation: f : X → Y,  x ↦ f(x).
2. **Domain** = valid inputs. **Codomain** = possible outputs. **Range** = actual outputs. Range ⊆ Codomain.
3. Functions correspond to relations Rƒ = {(x, f(x))}. Plotting a function = plotting this relation.
4. **Injective** (one-to-one): distinct inputs ⇒ distinct outputs.
5. **Surjective** (onto): range = codomain. Every output is reachable.
6. **Bijective** = injective + surjective. Establishes one-to-one correspondence.
7. Two sets have the same cardinality iff a bijection exists between them — the only way to compare infinite sets.
8. Whether a function is surjective/bijective depends on the **codomain**. Changing the codomain can change the classification.

---

## Lecture 7A — Relations as Tables & the Join Operation

### 1. Cartesian Products Revisited

- **Recall:** A × B = {(a, b) | a ∈ A, b ∈ B}. Order matters: A × B ≠ B × A. Size: |A × B| = |A| · |B|.
- **Self-product:** B × B includes all pairs — not just (b, b) but also (b₁, b₂) where b₁ ≠ b₂.
- **Example:** A = {1, 4, 7}, B = {1, 16, 49}. A × B has 9 pairs. The relation S ⊆ A × B picking only (1,1), (4,16), (7,49) is the "squaring" relation (b = a²).
- **Beyond pairs:** A × B × A gives triples. In general, n sets give n-tuples.

---

### 2. Relations on Numbers: More Examples

#### Divisibility

```
D = { (d, n) ∈ ℕ × ℕ | d | n }
```

Contains (7, 63), (17, 85), etc. Extending the generator from ℕ to ℤ adds negative divisors (e.g., (−7, 63)).

#### Prime Powers

First define primes: Primes = {p ∈ ℕ | p ≠ 1, factors(p) = {1, p}}.

Then:
```
PrimePowers = { (p, n) ∈ Primes × ℕ | n = pᵐ for some m ∈ ℕ }
```

Contains (5, 625) since 5⁴ = 625, and (3, 1) since 3⁰ = 1 by definition.

---

### 3. Relations Beyond Numbers: Airlines Example

Let C = set of cities served by an airline. The **direct flights** relation:

```
D ⊆ C × C,   D = { (a, b) ∈ C × C | direct flight from a to b }
```

**Properties:**
- **Irreflexive:** No flight from a city to itself. (a, a) ∉ D for all a.
- **Not necessarily symmetric:** Triangular routes exist (e.g., Chennai → Madurai direct, but return via Salem).

---

### 4. Tables Are Relations

> **Key Insight: Tables = Relations**
>
> A table (as in a database or spreadsheet) is a relation. Each **row** is a tuple; each **column** draws values from a set.

**Example — Flight distances:**

| Source | Destination | Distance (km) |
|--------|-------------|:-------------:|
| Bangalore | Chennai | 290 |
| Chennai | Delhi | 1752 |
| Delhi | Mumbai | 1148 |

This table is a relation on C × C × ℕ.

**Practical benefit of knowing properties:**
- Distance is **symmetric**: Chennai–Delhi = Delhi–Chennai = 1752 km ⇒ store only **half** the entries.
- Distance to self is always 0 (**reflexive** in a trivial sense) ⇒ no need to store those rows.

---

### 5. Keys and Key-Value Pairs

> **Keys**
>
> A **key** is a column (or set of columns) whose value **uniquely identifies** each row.

**Example — Student table:**

| Roll No. (key) | Name | DOB |
|:--------------:|------|:---:|
| CS2101 | Abhay | 2003-05-12 |
| CS2102 | Pai Gauche | 2002-11-03 |
| CS2103 | Pai Gauche | 2003-01-17 |

Names can repeat (two "Pai Gauche"), but roll numbers are unique. Given a roll number, you can find exactly one row — this makes the table behave like a **function** (roll number ↦ student record).

---

### 6. The Join Operation

> **Join: Combining Two Tables on a Common Column**
>
> Given two tables (relations) that share a common column (e.g., roll number), the **join** merges rows where the shared column values match.
>
> - **Students** table: (Roll, Name, DOB)
> - **Grades** table: (Roll, Subject, Grade)
> - **Joined result:** (Roll, Name, Subject, Grade)
>
> ```
> { (r, n, s, g) | (r, n, d) ∈ Students, (r', s, g) ∈ Grades, r = r' }
> ```
>
> Only rows with matching roll numbers are combined. The key ensures the correct name is paired with the correct grades — even when two students share the same name.

**Example result:**

| Roll | Name | Subject | Grade |
|:----:|------|:-------:|:-----:|
| CS2101 | Abhay | Maths | A |
| CS2102 | Pai Gauche | Maths | A |
| CS2103 | Pai Gauche | Physics | B |

The two "Pai Gauche" entries are correctly distinguished by their different roll numbers.

---

### 7. Why Relations Matter for Data Science

| Concept | Data Science Application |
|---------|--------------------------|
| Table = Relation | Databases store data as relations |
| Key = Unique identifier | Prevents ambiguity (e.g., duplicate names) |
| Join = Combine tables | Merge data from multiple sources |
| Symmetric relation | Store only half the entries (save space) |
| Reflexive/irreflexive | Identify trivial or impossible entries |

---

### 8. Key Takeaways

1. Cartesian products are ordered (A × B ≠ B × A), extend to n-tuples, and include self-products (A × A).
2. Relations are subsets of Cartesian products, defined explicitly or via set comprehension.
3. **Tables are relations.** Every database table, spreadsheet, or data frame is a relation on a Cartesian product of column value sets.
4. A **key** uniquely identifies each row — makes the table behave like a function (key ↦ record).
5. The **join** combines two tables on matching values in a shared column. It is the fundamental operation for merging data.
6. Knowing relation properties has practical value: symmetric relations need only half the storage; irreflexive relations exclude self-pairs.

---

## Lecture 7B — Function Examples: Ranges & Growth

### 1. Recap: Functions on Numbers

A function f : X → Y maps each input x ∈ X to exactly one output f(x) ∈ Y.

**Domain** = valid inputs.  **Codomain** = possible outputs.  **Range** = actual outputs (⊆ codomain).

**Functions beyond numbers:** The "mother" function maps every person to their (unique) mother. But in this course, we focus on **functions on numbers**.

---

### 2. What Is the Range?

Even when the codomain is all of ℝ, the range may be smaller.

| Function | Range | Why |
|----------|:-----:|-----|
| f(x) = x² | [0, ∞) | Squaring always gives ≥ 0; no upper bound |
| f(x) = x³ − 3x² + 5 | (−∞, ∞) | Cubic grows to ±∞ |
| f(x) = 5 sin x | [−5, +5] | Sine oscillates in [−1, 1]; scaled by 5 |

**Bounded vs. unbounded:**
- x²: unbounded above, bounded below (by 0).
- x³ − 3x² + 5: unbounded in both directions.
- 5 sin x: bounded in both directions (range is a closed interval).

---

### 3. Where Are the Maxima and Minima?

> **Global vs. Local Extrema**
>
> **Global maximum/minimum:** The largest/smallest value the function *ever* takes.
>
> **Local maximum/minimum:** A point where the function is larger/smaller than its *immediate neighbours* (the function "turns around").

| Function | Global min | Global max | Local features |
|----------|:----------:|:----------:|----------------|
| x² | 0 (at x = 0) | None (→ ∞) | Single minimum |
| x³ − 3x² + 5 | None (→ −∞) | None (→ ∞) | Local max at x = 0, local min at x = 2 |
| 5 sin x | −5 | +5 | Periodic; infinitely many |

**The cubic example:** f(x) = x³ − 3x² + 5 has no global extrema, but it zigzags: rises to a **local maximum** at x = 0, dips to a **local minimum** at x = 2, then rises again. Finding these turning points is a key topic in calculus.

**The sine example:** 5 sin x attains its global max (+5) and global min (−5) **infinitely often**, periodically.

---

### 4. How Fast Does a Function Grow?

> **Comparing Growth Rates**
>
> Given two functions, which one **eventually dominates**?
>
> x³ − 3x² + 5 vs. x²: Initially x² may be larger, but eventually the cubic overtakes the quadratic and stays above it forever.
>
> **General principle:** Higher-degree polynomials grow faster. x³ eventually beats x², which eventually beats x.

#### Why Growth Rates Matter: A Data Science Example

Let g(y) = number of data science graduates in year y.  
Let j(y) = number of new data science jobs in year y.

- If j(y) grows faster than g(y): demand exceeds supply → more students enrol.
- If g(y) grows faster than j(y): supply exceeds demand → graduates struggle to find jobs.

Comparing growth rates of real-world quantities is a core data analysis task.

---

### 5. Summary: Three Key Questions About Functions

| Question | What we want to know |
|----------|---------------------|
| **Range** | What output values can the function actually produce? |
| **Extrema** | Where does the function reach its highest/lowest values (global or local)? |
| **Growth rate** | How fast does the function increase, and which function dominates? |

These questions will be studied in detail using calculus tools (derivatives, limits) in later weeks.

---

### 6. Key Takeaways

1. The **range** of a function may be much smaller than the codomain. x² has range [0, ∞) even though codomain is ℝ.
2. Functions can be **bounded** (5 sin x ∈ [−5, 5]) or **unbounded** (x³ → ±∞).
3. **Global extrema** are the overall max/min. **Local extrema** are turning points where the function reverses direction.
4. A cubic like x³ − 3x² + 5 has local max at x = 0 and local min at x = 2, but **no global extrema**.
5. **Growth rate comparison:** higher-degree polynomials eventually dominate lower-degree ones (x³ beats x²).
6. Comparing growth rates has real-world applications: jobs vs. graduates, revenue vs. costs, supply vs. demand.

---

*These notes are based on the video lectures from the Mathematics 1 for Data Science course offered at IIT Madras BS Degree Programme.*  
*Notes created by: Vishal (Instructor)*
---
title: Linear Algebra - Vector Spaces
published: 2026-02-05
description: 'Introduction to vector spaces, their properties, and fundamental concepts in linear algebra'
tags: [Linear Algebra, Vectors, Mathematics, Vector Spaces]
category: Mathematics
draft: false
---

# Linear Algebra - Vector Spaces

Vector spaces are fundamental structures in linear algebra that generalize the notion of vectors from geometry and physics to abstract mathematical objects.

## Definition of Vector Space

A vector space $V$ over a field $F$ (usually real numbers $\mathbb{R}$ or complex numbers $\mathbb{C}$) is a set equipped with two operations:

1. **Vector addition**: $+: V \times V \rightarrow V$
2. **Scalar multiplication**: $\cdot: F \times V \rightarrow V$

These operations must satisfy the following axioms:

## Vector Space Axioms

For all vectors $\mathbf{u}, \mathbf{v}, \mathbf{w} \in V$ and all scalars $a, b \in F$:

### Addition Axioms:
1. **Closure**: $\mathbf{u} + \mathbf{v} \in V$
2. **Commutativity**: $\mathbf{u} + \mathbf{v} = \mathbf{v} + \mathbf{u}$
3. **Associativity**: $(\mathbf{u} + \mathbf{v}) + \mathbf{w} = \mathbf{u} + (\mathbf{v} + \mathbf{w})$
4. **Identity element**: There exists $\mathbf{0} \in V$ such that $\mathbf{v} + \mathbf{0} = \mathbf{v}$
5. **Inverse element**: For each $\mathbf{v} \in V$, there exists $-\mathbf{v} \in V$ such that $\mathbf{v} + (-\mathbf{v}) = \mathbf{0}$

### Scalar Multiplication Axioms:
6. **Closure**: $a\mathbf{v} \in V$
7. **Associativity**: $a(b\mathbf{v}) = (ab)\mathbf{v}$
8. **Identity**: $1\mathbf{v} = \mathbf{v}$ (where $1$ is the multiplicative identity in $F$)

### Distributive Laws:
9. **Vector distributivity**: $a(\mathbf{u} + \mathbf{v}) = a\mathbf{u} + a\mathbf{v}$
10. **Scalar distributivity**: $(a + b)\mathbf{v} = a\mathbf{v} + b\mathbf{v}$

## Examples of Vector Spaces

### 1. Euclidean Space $\mathbb{R}^n$
The set of all ordered $n$-tuples of real numbers:
$$\mathbb{R}^n = \{(x_1, x_2, \ldots, x_n) : x_i \in \mathbb{R}\}$$

**Operations:**
- Addition: $(x_1, \ldots, x_n) + (y_1, \ldots, y_n) = (x_1 + y_1, \ldots, x_n + y_n)$
- Scalar multiplication: $c(x_1, \ldots, x_n) = (cx_1, \ldots, cx_n)$

### 2. Polynomial Space $P_n$
The set of all polynomials of degree at most $n$:
$$P_n = \{a_0 + a_1x + a_2x^2 + \cdots + a_nx^n : a_i \in \mathbb{R}\}$$

### 3. Matrix Space $M_{m \times n}$
The set of all $m \times n$ matrices with entries from $\mathbb{R}$.

### 4. Function Space $F(S, \mathbb{R})$
The set of all functions from a set $S$ to $\mathbb{R}$.

## Subspaces

A **subspace** $W$ of a vector space $V$ is a subset of $V$ that is itself a vector space under the same operations.

### Subspace Test
A non-empty subset $W \subseteq V$ is a subspace if and only if:
1. **Closure under addition**: If $\mathbf{u}, \mathbf{v} \in W$, then $\mathbf{u} + \mathbf{v} \in W$
2. **Closure under scalar multiplication**: If $\mathbf{v} \in W$ and $c \in F$, then $c\mathbf{v} \in W$

### Examples of Subspaces
- The trivial subspace $\{\mathbf{0}\}$
- Lines through the origin in $\mathbb{R}^2$ or $\mathbb{R}^3$
- Planes through the origin in $\mathbb{R}^3$
- The entire space $V$ itself

## Linear Combinations

Given vectors $\mathbf{v_1}, \mathbf{v_2}, \ldots, \mathbf{v_k} \in V$ and scalars $c_1, c_2, \ldots, c_k \in F$, a **linear combination** is:

$$c_1\mathbf{v_1} + c_2\mathbf{v_2} + \cdots + c_k\mathbf{v_k}$$

### Span
The **span** of a set of vectors $S = \{\mathbf{v_1}, \mathbf{v_2}, \ldots, \mathbf{v_k}\}$ is the set of all linear combinations of vectors in $S$:

$$\text{span}(S) = \left\{\sum_{i=1}^k c_i\mathbf{v_i} : c_i \in F\right\}$$

## Key Properties

:::important
The span of any set of vectors is always a subspace of the vector space.
:::

:::note
Every vector space contains at least two subspaces: the trivial subspace $\{\mathbf{0}\}$ and the entire space $V$.
:::

## Applications

Vector spaces appear in many areas:
- **Computer Graphics**: 3D transformations and rendering
- **Quantum Mechanics**: State spaces of quantum systems
- **Signal Processing**: Function spaces for signals
- **Machine Learning**: Feature spaces and data representation

## Practice Problems

1. Verify that $\mathbb{R}^2$ with the operations defined above satisfies all vector space axioms.

2. Determine which of the following are subspaces of $\mathbb{R}^3$:
   - $\{(x, y, z) : x + y + z = 0\}$
   - $\{(x, y, z) : x + y + z = 1\}$
   - $\{(x, y, 0) : x, y \in \mathbb{R}\}$

3. Find the span of the vectors $(1, 2, 3)$ and $(2, 1, 0)$ in $\mathbb{R}^3$.

## Next Topics

In our next lesson, we'll explore:
- Linear independence and dependence
- Basis and dimension of vector spaces
- Coordinate systems

---

*This is part of the Mathematics course series focusing on Linear Algebra. Check out other mathematical topics in the course collection.*
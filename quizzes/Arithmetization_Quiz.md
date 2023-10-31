# Arithmetization Quiz

**Question 1**

How many gates are required in R1CS while proving that you know a solution to an equation of degree 3

**Solution:**

The number of gates is not dependent on the degree of the equation.

For example, equations $x^2 - 1$ and $x^2 - 5x - 1$ have the same degree but different number of gates

**Question 2**

How many gates are required in R1CS while proving that you know a solution to this equation

$$
3x^2 + x + 2 == 32
$$

**Solution:**

This equation requires 4 gates

1. $x*x = sym_1$
2. $3*sym_1 = sym_2$
3. $sym_2 + x = sym_3$
4. $sym_3 + 2 = out$

**Question 3**

While proving for the equation $x - 3 = 5$, which of the following are valid constraints for the below gate

$$
symbols \hspace{0.1cm} order = [\sim one, x, \sim out]
$$

$$
\sim out = x - 3
$$

**Solution:**

The correct set of constraints is:

$$
\vec{a} = [1, 0, 0] \newline
\vec{b} = [-3, 1, 0] \newline
\vec{c} = [0, 0, 1] \newline
$$

The gate can be written as $1 * (x - 3) = \sim out$

Hence $\vec{a}$ represents 1, $\vec{b}$ represents $(x-3)$ and $\vec{c}$ represents the symbol ~out

**Question 4**

If the number of gates is 4 and the number of symbols is 6, what is the total number of polynomials in QAP?

A) 6

B) 12

C) 18

D) Cannot be determined

**Solution:**

The number of columns in R1CS corresponds to symbols and the number of rows to gates. There are 3 such matrices each containing the collection of $\vec{a}$, $\vec{b}$ , and $\vec{c}$ vectors. In this case, for each matrix 6 polynomials are formed as each polynomial represents a column. Since there are 3 such matrices, 18 polynomials are formed in total.

**Question 5**

What is the degree of polynomials formed in QAP if the number of gates is 3?

A) 3

B) 2

C) 1

D) Cannot be determined

**Solution:**

If the number of gates is 3, 3 points go into forming a Lagrange polynomial. A unique polynomial that passes through these 3 points will be of degree `n-1` or 2.

**Question 6**

Consider two polynomials F(x) and P(x) defined on x that can only be a natural number between 1 and 100,000. Both F(x) and P(x) have a degree of 10. What is the upper bound of probability that if a random point is chosen, it satisfies both polynomials?

A) **0.0001**

B) 0.001

C) 0.2

D) 0.6

**Solution:**

Since F(x) and P(x) both have a degree of 10, the maximum number of points they can intersect at is 10. If a random point is chosen out of 100,000 available points, the probability that it is one of those 10 points is $10/100000$ = 0.0001
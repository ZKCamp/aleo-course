# Polynomials Quiz

**Question 1**

What is the value of polynomial $f(x) = x^3 + x^2 + 1$ at $x = 2$ ?

**Solution**

Plugging in the value of x = 2, we get $f(x) = 2^3 + 2^2 + 1 = 13$

**Question 2**

What is the degree of this polynomial?

$$
f(x) = 12x^8 + 17x^6 + 21x^3 + 11x^2 + 41x + 3
$$

**Solution:** The degree of a polynomial is the highest power of x it contains. In this case, the highest power of x is 8, hence the degree is 8.

**Question 3**

What are the roots of the given polynomial?

$$
f(x) = x^2 - 5x + 6
$$

**Solution**: The roots of polynomials are values of `x` where the value of the polynomial is 0, i.e., f(x) = 0. The following polynomial can be written as `(x-2)*(x-3) = 0`, which means it is zero at x = 2, 3.

**Question 4**

What is the value of **t** from the polynomial $x^2 -3x + t$, if one of the zeroes of the polynomial is **2**?

**Solution:** 

Given one of the zeroes of the polynomial is 2, we can say that f(2) = 0.

$\therefore 2^2 - 3*2 + t = 0$

$\therefore t = 2$

**Question 5**

What is the sum of polynomials $p_1 = 3x^3 - 5x^2 + 6x - 7$ and $p_2 = -4x^3 + 3x^2 + 2x$ ?

**Solution:** The sum of polynomials is equal to the sum of coefficients of each degree. In this case, the sum equals

$(3 - 4)x^3 + (-5 + 3)x^2 + (6 + 2)x - 7 = -x^3 - 2x^2 + 8x - 7$

**Question 6**

What is the product of polynomials $p_1 = 3x^3 - 5x^2 + 6x - 7$ and $p_2 = -4x^3 + 3x^2 + 2x$ ?

**Solution:** The product of two polynomials $p_1$ and $p_2$ is the multiplication of each term in the polynomial. The answer is $-12x^6 + 29x^5 - 33x^4 + 36x^3 - 9x^2 - 14x$

**Question 7**

What is the degree of product of polynomials $p_1 = -2x^6 - 10x^3 + 17x^2 + 6x - 7$ and

 $p_2 = 11x^{12} + 16x^{11} + 3x^{10} + 6x^9 - x^6 + 5x^4 + 4x^3 + 3x^2 + 2x$ ?

**Solution:**

The highest power in the product of these polynomials is going to come from the multiplication of the highest power terms in each of these polynomials which are $-2x^6$ and $11x^{12}$. The multiplication of these terms is going to give the power 18 of x, which is the degree of the resulting polynomial.

**Question 8**

Calculate the value of polynomial $p_1$

$$
p_1 = \dfrac{x^3 - 32x^2 + 141x - 162}{x - 27}
$$

**Solution:** Long division of polynomial $x^3 - 32x^2 + 141x - 162$ by $x - 27$ gives quotient $x^2 - 5x + 6$

**Question 9**

Find the polynomial of the least degree which should be subtracted from the polynomial

 $x^4 + 2x^3 - 4x^2 + 6x - 3$ so that it is exactly divisible by $x^2 - x + 1$

**Solution:** To find this polynomial, use the long division method to find the remainder. When subtracted from the polynomial, the remainder makes it completely divisible by the divisor. In this case, the remainder is `x - 1`

**Question 10**

An equation of line is a Lagrange polynomial passing through two points. Can you find the equation of a line which passes through points - (1, 4) and (2, 6)

**Solution**:

The equation of a line that passes through two points is $(x_1, y_1), (x_2, y_2)$ is

$y - y_1 = \frac{(y_2 - y_1) * (x - x_1)}{(x_2 - x_1)}$

Plugging in the values of two points, we get $y = 2x + 2$. This can also be solved using Lagrange polynomial equation.

**Question 11**

Find the Lagrange polynomial which passes through these points - (0, 1), (2, 4), and (6, 8)

**Solution:**

$L_1 = \frac{(x - 2) * (x - 6)}{(0 - 2) * (0 - 6)}$

$L_2 = \frac{(x - 0) * (x - 6)}{(2 - 0) * (2 - 6)}$

$L_3 = \frac{(x - 0) * (x - 2)}{(6 - 0) * (6 - 2)}$

$f(x) = 1 * L_1 + 4 * L_2 + 8 * L_3$

$\therefore f(x) =$  $\dfrac{-x^2}{12} + \dfrac{5x}{3} + 1$
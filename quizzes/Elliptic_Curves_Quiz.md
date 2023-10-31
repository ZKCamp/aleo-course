# Elliptic Curves Quiz

**Question 1**

Given the elliptic curve,

$Y^2 = X^3 + 497X + 1768, p=9739$

Can you find the point Q(x, y) such that given a point **P(8045,7175)**, **`P + Q = O`**?

**Solution:**

Q is the negation of point P. Negation of a point $(x_1, y_1)$ is calculated as $(x_1, -y_1)$. In this case, the point Q is (8045, 2564)

**Note: The code snippet that is used for the next questions is as below**

```python
from copy import deepcopy

class EllipticCurve:
    def __init__(self, a, b, p):
        self.a = a
        self.b = b
        self.p = p

class Point:
    def __init__(self, x=False, y=False):
        self.x = x
        self.y = y
        self.o = not (type(x) == int and type(y) == int)

    def __eq__(self, q):
        return (self.x == q.x and self.y == q.y) or (self.o and q.o)

    def __ne__(self, q):
        return not (self == q)

    def __str__(self):
        return (f"Point({self.x},{self.y})" if not self.o else "Point(O)")

    def __mul__(self, n):
        return self.scalar_mult(self, n)

    def __add__(self, q):
        return self.point_add(self, q)

    def inverse(self, val, p):
        return pow(val, p - 2, p)

    def scalar_mult(self, p, n, ec=EllipticCurve(497, 1768, 9739)):
        q = deepcopy(p)
        r = Point()
        while n > 0:
            if n % 2 == 1:
                r = r + q
            q = q + q
            n //= 2
        return r

    def point_add(self, p, q, ec=EllipticCurve(497, 1768, 9739)):
        # P + point at infinity = P
        if p.o:
            return q
        if q.o:
            return p

        # P + -P = point at infinity
        if p.x == q.x and p.y == -q.y:
            return Point()

        # Else, point add algorithm
        if p != q:
            x_inv = self.inverse(q.x - p.x, ec.p)
            l = ((q.y - p.y) * x_inv) % ec.p
        else:
            y_inv = self.inverse(2 * p.y, ec.p)
            l = (((3 * (p.x ** 2)) + ec.a) * y_inv) % ec.p
        res_x = ((l ** 2) - p.x - q.x) % ec.p
        res_y = ((l * (p.x - res_x)) - p.y) % ec.p
        return Point(res_x, res_y)
```

**Question 2**

Given an elliptic curve of type

$$
Y^2 = X^3 + aX + b
$$

Here is the algorithm for calculating the addition of two points P and Q:

(a) If P = O, then P + Q = Q

(b) Otherwise, if Q = O, then P + Q = P

(c) Otherwise, write P = $(x_1, y_1)$ and Q = $(x_2, y_2)$

(d) If $x_1 = x_2$ and $y_1 = -y_2$, then P + Q = O.

(e) Otherwise:

(e1) if P ≠ Q: $λ = \frac{(y_2 - y_1)}{x_2 - x_1}$

(e2) if P = Q: $λ = \frac{3x_1^2 + a}{2y_1}$

(f) $x_3 = λ^2 - x_1 - x_2$, $y_3 = λ(x_1 - x_3) - y_1$

(g) P + Q = $(x_3, y_3)$

Consider the elliptic curve,

$Y^2 = X^3 + 497X + 1768, p=9739$

Given points, P = (493, 5564), Q = (1539, 4742), R = (4403,5202), 

What is the value of **P + P + Q + R**?

**Solution:**

Execute the following code

```python
P = Point(493, 5564)
Q = Point(1539, 4742)
R = Point(4403, 5202)

print(P + P + Q + R)
```

The answer/output should be (4215,2162)

**Question 3**

Using the algorithm and elliptic curve from the previous question, find the value of **P - Q,** if the value of P is (493, 5564) and Q is (1539, 4742)

**Solution:**

Negation of Q is (1539, 4997). Execute the following code to get the answer

```python
P = Point(493, 5564)
Q = Point(1539, 4997)

print(P + Q)
```

The answer/output should be (6782,8152)

**Question 4**

In elliptic curves, scalar multiplication is defined as repeated additions: **3P = P + P + P**.

To calculate the scalar multiplication of point P by n , you can use the following algorithm called **Double and Add algorithm**

1. Set Q = P and R = O
2. Loop while n > 0
    1. If n ≡ 1 mod 2, set R = R + Q
    2. Set Q = 2Q and n = ⌊n/2⌋
    3. If n > 0, continue with loop at Step 2
3. Return the point R, which equals nP

Consider the elliptic curve,

$Y^2 = X^3 + 497X + 1768, p=9739$

Given P = (2339, 2213), find the point **Q(x, y) = 7863 P** by implementing the double and add algorithm

**Solution:**

Execute the following code to get the answer

```python
P = Point(2339, 2213)

print(P * 7863)
```

The answer/output should be (9467,2742)

**Question 5**

Given the following,

Elliptic curve

$Y^2 = X^3 + 497X + 1768, p=9739, G=(1804, 5368)$

Encrypted powers of “s”

$[s^0]$ = (1804, 5368)

$[s^1]$ = (4929,8240)

$[s^2]$ = (7909,7508)

$[s^3]$ = (5697,8702)

Polynomial f(x)

$f(x) = 72x^3 + 3x^2 + 32x + 4$

Paste the value of encrypted f(s) (also denoted as [f(s)]) in the form of “(x,y)” below.

**Solution:**

Execute the following code to get the answer

```python
S_0 = Point(1804, 5368)
S_1 = Point(4929, 8240)
S_2 = Point(7909, 7508)
S_3 = Point(5697, 8702)

print(S_3 * 72 + S_2 * 3 + S_1 * 32 + S_0 * 4)
```

The answer/output should be (959,1461)
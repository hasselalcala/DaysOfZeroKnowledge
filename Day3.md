Today we are going to learn about a bit complex topic Elliptic Curve Cryptography (ECC), to provide a simple overview of what ECC is and why it is considered secure. 

What is an elliptic curve? Mathematically, an ECC is the set of point described by the equation $y^2 = x^3 + ax + b$ where $4a^3 + 27b^2 \neq 0$ (this is require to exclude singular curves). The equation above is what is called Weierstrass normal form for elliptic curves. Depending on the value of 
$a$ and $b$, elliptic curves may assume different shapes on the plane. As it can be easily seen and verified, elliptic curves are symmetric about the 
x-axis.

![Elliptic Curve Cryptography](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/ECC_1.png)

We will also need a point at infinity (also known as ideal point) to be part of our curve and denote with the symbol 0 (zero).

What is a group for elliptic curves?

A group is defined following the next four properties:

- The elements of the group are the points of an elliptic curve.
- The identity element is the point at infinity 0, such that $a + 0 = 0 + a = a$;
- The inverse of a point $P$ is the one symmetric about the x-axis.
- Addition operation is given by the following rule: given three aligned, non-zero points $P, Q, R$, their sum is $P + Q + R = 0$.

![Elliptic Curve Cryptography](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/ECC_1.png)


# Reference
Corbellini, Andrea. Elliptic Curve Cryptography: a gentle introduction. 


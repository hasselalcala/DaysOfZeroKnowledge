Today we are going to learn about a bit complex topic Elliptic Curve Cryptography (ECC), to provide a simple overview of what ECC is and why it is considered secure. 

What is an elliptic curve? Mathematically, an ECC is the set of point described by the equation $y^2 = x^3 + ax + b$ where $4a^3 + 27b^2 \neq 0$ (this is require to exclude singular curves). The equation above is what is called Weierstrass normal form for elliptic curves. Depending on the value of 
$a$ and $b$, elliptic curves may assume different shapes on the plane. As it can be easily seen and verified, elliptic curves are symmetric about the 
x-axis.

We will also need a point at infinity (also known as ideal point) to be part of our curve and denote with the symbol 0 (zero).

![Elliptic Curve Cryptography](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/ECC_1.png)

In order for the set $G$ to be a group, an addition operation must satisfies Abelian Group Properties:

1. Closure: if $a$ and $b$ are members og $G$ then $a+b$ is also
2. Associativity: $( a + b ) + c = a + ( b + c ) $
3. Identity: $ a + 0 = 0 + a = a $
4. Inverse: for every $a$, there exists $b$ such that $a + b = 0$
5. Commutativity: $a + b = b + a$

What is a group for elliptic curves?

A group is defined following the next four properties:

- The elements of the group are the points of an elliptic curve.
- The identity element is the point at infinity 0, such that $a + 0 = 0 + a = a$;
- The inverse of a point $P$ is the one symmetric about the x-axis.
- Addition operation is given by the following rule: given three aligned, non-zero points $P, Q, R$, their sum is $P + Q + R = 0$. This means that, if 
$ P, Q, R$ are aligned, then $P+(Q+R)=Q+(P+R)=R+(P+Q) = ... =0$. This way, we proved that our $+$ operator is both associative and commutative, and we are in an abelian group.

![Sum of three aligned points](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/ECC_2.png)

If we want to perform point addition $P + Q + R = 0$, then $P + Q = -R$. The corner cases are when we have symmetric points and one zero point, we already know that $P + (-P) = 0$ and $P + 0 = 0 + P = P$. 

If we consider two non-zero, non-symmetric points $P = (x_P , y_P )$ and $Q= (x_Q , y_Q )$ and $P$ and $Q$ are distinct $(x_P \neq x_Q)$, the line through them has slope:

$m = \frac{y_P - y_Q}{x_P - x_Q}$

The intersection of this line with the elliptic curve is a third point $R = (x_{R}, y_{R})$: 

$x_R = m^2 - x_P - x_Q$ and 
$y_R = y_P + m (x_R - x_P) = y_Q + m (x_R - x_Q)$

The case $P = Q$ needs to be treated a bit differently: the equations for $x_R$ and $y_R$ are the same, but given that $x_P = x_Q$, we must use a different equation for the slope:
 $m = \frac{3x_P^2 + a}{2y_P}$

# Reference
Corbellini, Andrea. Elliptic Curve Cryptography: a gentle introduction. 


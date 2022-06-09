# #DaysOfZeroKnowledge. Day 7.

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
 
 
That's all for this thread. Thank you for reading! If you liked this thread, follow me @Hasseru and retweet.


# Reference
Corbellini, Andrea. Elliptic Curve Cryptography: a gentle introduction.

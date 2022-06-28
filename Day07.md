# #DaysOfZeroKnowledge. Day 7.

Today we are going to continue talking about ECC. Well, What is a group for elliptic curves?

A group is defined following the next four properties:

- The elements of the group are the points of an elliptic curve.
- The identity element is the point at infinity 0, such that $a + 0 = 0 + a = a$;
- The inverse of a point $P$ is the one symmetric about the x-axis.
- Addition operation is given by the following rule: given three aligned, non-zero points $P, Q, R$, their sum is $P + Q + R = 0$. This means that, if 
$ P, Q, R$ are aligned, then $P+(Q+R)=Q+(P+R)=R+(P+Q) = ... =0$. This way, we proved that our $+$ operator is both associative and commutative, and we are in an abelian group.

![Sum of three aligned points](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/ECC_2.png)

If we want to perform point addition $P + Q + R = 0$, then $P + Q = -R$. The corner cases are when we have symmetric points and one zero point, we already know that $P + (-P) = 0$ and $P + 0 = 0 + P = P$. 

![Example of sum](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/ECC_Example.png)
 
That's all for this thread. Thank you for reading! 
If you liked this thread, follow me @Hasseru and retweet.


# Reference
Corbellini, Andrea. Elliptic Curve Cryptography: a gentle introduction.

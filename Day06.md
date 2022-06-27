# #DaysOfZeroKnowledge. Day 6.

Today we are going to learn about a bit complex topic Elliptic Curve Cryptography (ECC), to provide a simple overview of what ECC is and why it is considered secure. 

![What is an elliptic curve?](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/ECC_0.png)

The equation above is what is called Weierstrass normal form for elliptic curves. Depending on the value of $a$ and $b$, elliptic curves may assume different shapes on the plane. As it can be easily seen and verified, elliptic curves are symmetric about the x-axis.

We will also need a point at infinity (also known as ideal point) to be part of our curve and denote with the symbol 0 (zero).

![Elliptic Curve Cryptography](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/ECC_1.png)

In order for the set $G$ to be a group, an addition operation must satisfies Abelian Group Properties:

1. Closure: if $a$ and $b$ are members of $G$ then $a+b$ is also
2. Associativity: $( a + b ) + c = a + ( b + c ) $
3. Identity: $ a + 0 = 0 + a = a $
4. Inverse: for every $a$, there exists $b$ such that $a + b = 0$
5. Commutativity: $a + b = b + a$
 
That's all for this thread. Thank you for reading! If you liked this thread, follow me @Hasseru and retweet.


# Reference
Corbellini, Andrea. Elliptic Curve Cryptography: a gentle introduction.




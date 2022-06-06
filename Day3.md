Today we are going to learn about a bit complex topic Elliptic Curve Cryptography (ECC), to provide a simple overview of what ECC is and why it is considered secure. 

What is an elliptic curve? Mathematically, an ECC is the set of point described by the equation $y^2 = x^3 + ax + b$ where $4a^3 + 27b^2 \neq 0$ (this is require to exclude singular curves). The equation above is what is called Weierstrass normal form for elliptic curves. Depending on the value of 
$a$ and $b$, elliptic curves may assume different shapes on the plane. As it can be easily seen and verified, elliptic curves are symmetric about the 
x-axis.

![Elliptic Curve Cryptography](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/ECC_1.png)


# Reference

Corbellini, Andrea. Elliptic Curve Cryptography: a gentle introduction. 


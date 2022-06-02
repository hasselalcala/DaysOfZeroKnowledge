# #DaysOfZeroKnowledge. Day 2.

ZKP is not a new concept and in order to understand ZKP there are a series of mathematics and cryptographic that need to be understood.

Modular math is a fundamental component of cryptographic. The idea is essentially very simple and is identical to the “clock arithmetic” you learn in school. More formally, Let n be a positive integer. We denote the set [0..n−1] by Zn.

We consider two integers x,y to be the same if x and y differ by a multiple of n, and we write this as x=y(mod n), and say that x and y are congruent modulo n. We may omit (mod n) when it is clear from context. Every integer x is congruent to some y in Zn. When we add or subtract multiples of n from an integer x to reach some y ∈ Zn, we say are reducing x modulo n, and y is the residue. For example:

![Modular arithmetic](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/modularMath.png)

The Diffie - Hellman Algorithm (DHA) is one of the first practical implementations of public-key cryptography. It was published in 1976 by Whitfield Diffie and Martin Hellman. It is a key - exchange protocol that enables two parties communicating over public channel to establish a mutual secret without it being transmitted over the Internet. DHA enables the two to use a public key to encrypt and decrypt their conversation or data using symmetric cryptography.

![Diffie - Hellman Algorithm](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/diffieHellman .png)

Now Alice and Bob know to encrypt/decrypt their messages using the shared secret key 10.

RSA encryption is a mathematical problem that makes the internet work today. This algorithm relies on a concept of public and private keys and the idea of factoring large numbers using prime numbers. Public key is used to encrypt the message and private key is uses to decrypt the message. 

To obtain the keys, we need to follow the next steps:

![RSA Key Generation](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/RSA_1.png)

![Message encryption/decryption](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/RSA_2.png)

One of the first interactive proof of knowledge algorithm is Fiat - Shamir, which is consider the "grandfather" of ZKPs because allows one to prove information about a number, without revealing the number. The algorithm work as follow:

![Message encryption/decryption](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/Fiat-shamir.png)

That's all for this thread. Thank you for reading! 

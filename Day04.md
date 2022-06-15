# #DaysOfZeroKnowledge. Day 4.

Today, we are going to talk about RSA encryption. It is a mathematical problem that makes the internet work today. This algorithm relies on a concept of public and private keys and the idea of factoring large numbers using prime numbers. Public key is used to encrypt the message and private key is uses to decrypt the message. 

To obtain the keys, we need to follow the next steps:

![RSA Key Generation](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/RSA_1.png)

The idea of RSA is based on the fact that it is difficult to factorize a large integer. The public key consists of two numbers where one number is multiplication of two large prime numbers. And private key is also derived from the same two prime numbers. So if somebody can factorize the large number, the private key is compromised. 

Therefore encryption strength totally lies on the key size and if we double or triple the key size, the strength of encryption increases exponentially. RSA keys can be typically 1024 or 2048 bits long, but experts believe that 1024 bit keys could be broken in the near future. But till now it seems to be an infeasible task.

To encrypt and decrypt a message, we consider the following: 

![Message encryption/decryption](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/RSA_2.png)

![Message encryption/decryption example](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/RSA_3.png)



That's all for this thread. Thank you for reading! If you liked this thread, follow me @Hasseru and retweet.







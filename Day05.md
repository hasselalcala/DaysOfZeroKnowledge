# #DaysOfZeroKnowledge. Day 5.

One of the first interactive proof of knowledge algorithm is Fiat - Shamir, which is consider the "grandfather" of ZKPs because allows one to prove information about a number, without revealing the number. The algorithm work as follow:

![Message encryption/decryption](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/fiatShamir.png)

For the method to work, the original interactive proof must have the property of being public-coin, i.e. verifier's random coins are made public throughout the proof protocol. 

The Fiat–Shamir Algorithm may also be viewed as converting a public-coin interactive proof of knowledge into a non-interactive proof of knowledge. If the interactive proof is used as an identification tool, then the non-interactive version can be used directly as a digital signature by using the message as part of the input to the random oracle.

A random oracle is an oracle (a theoretical black box) that responds to every unique query with a (truly) random response chosen uniformly from its output domain. If a query is repeated, it responds the same way every time that query is submitted.

That's all for this thread. Thank you for reading! If you liked this thread, follow me @Hasseru and retweet.

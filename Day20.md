# #DaysOfZeroKnowledge. Day 20.

In the following days, we’ll cover the various techniques to write circuits, and show you how to create and verify proofs off-chain and on-chain on ethereum. Today we are going to learn the pre-requisites to create and execute our first ZK proof using circom and snarkjs libraries.

First off, make sure you have a recent version of Node.js installed.

![Install Node.js](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/circom_09.png)

Now, to install circom and snarkjs run the following commands:

![Install circom and snarkjs](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/circom_10.png)

Once that we’ve installed circom and snarkjs, let’s build a circuit that we know two numbers (call them a and b) that multiply together to give c, without revealing a and b.

![What is a circuit?](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/circom_11.png)

Even though the verifier has zero knowledge about the private inputs to the circuit, the proof, the output, and the public inputs(s) will be enough to convince her that our statement is valid (hence the term zero-knowledge proof).

Now that we know what a circuit is and why it’s useful, tomorrow we are going to start by designing one. 

That's all for this thread. Thank you for reading! If you liked, follow me @Hasseru and retweet.

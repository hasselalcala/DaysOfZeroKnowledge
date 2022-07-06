# #DaysOfZeroKnowledge. Day 17.

As we notice, zk-SNARK permits proving computational statement, but they cannot be applied to the computational problem directly, the statement first needs to be converted into the right form, for example: a QAP. The nice thing about arithmetic circuits and QAP, is that although most ZK protocols have an inherent complexity that can be overwhelming, the design of arithmetic circuits is clear and neat.

Today we are going to talk about an "ingredient" that is used to build a ZK proof, which is a language for expressing the property you want to prove.

But, first let's remember some important ideas:

![Arithmetic Circuit Satisfiability](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/zksnark_27.png)

The language that we are going to use to express the arithmetic circuit is circom and to generate the proof and the verifier, we can use snarkjs, which is a JavaScript implementation of zk-SNARK developed by iden3.

![What is circom?](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/zksnark_28.png)

![circom in zk-proof](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/zksnark_29.png)

The next days, we are going to learn the basis about circom language, how to create and execute our first ZK proof using circom and snarkjs libraries. That's all for this thread. Thank you for reading! If you liked, follow me @Hasseru and retweet.

# #DaysOfZeroKnowledge. Day 11.

Today, we are going to talk a particular type of ZKP, which does not require interaction between a verifier and a prover, is a Non-Interactive Zero Knowledge Proof (NIZK). 

NIZK are very suitable for Ethereum blockchain applications because they allow a smart contract to act as a verifier. This way, anyone can generate a proof and send it as part of a transaction to the smart contract, which can perform some action depending on whether the proof is valid or not. Also, this protocol can verify one’s statement to a larger group of people. 

The most preferable NIZK is Zero-knowledge Succinct Non-Interactive Argument of Knowledge (zk-SNARK) proof.
  
This protocol adds the following:

![Features with zk-SNARK](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/zksnark_4.png)

These properties make zk-SNARK especially suitable for blockchains, where on-chain storage and computation can be expensive and senders often go offline after sending a transaction.

This protocol uses three algorithms:

![Key generator](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/zksnark_1.png)

![Prover function](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/zksnark_2.png)

![Verifier function](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/zksnark_3.png)

When zk-SNARKs are used in blockchains, both the key and proof generation are executed off-chain. Only the general verification algorithm is run inside a smart contract on chain.

That's all for this thread. Thank you for reading! If you liked this thread, follow me @Hasseru and retweet.

# References

[zk-SNARKs on Bitcoin](https://xiaohuiliu.medium.com/zk-snarks-on-bitcoin-239d96d182bd).



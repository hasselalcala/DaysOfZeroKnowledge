# #DaysOfZeroKnowledge. Day 1.

Today, I want to start this challenge with some background that will be useful to understand Zero-Knowledge Proof (ZKP). 

ZKP is a protocol that enables one party, called the prover, to convince another, the verifier, that a statement is true without revealing any information beyond the veracity of the statement. 

The main idea behind this concept is to prove possession of knowledge without revealing it. For example, Alice and Bob are racing to find Waldo. 

![Find Waldo Example](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/findWaldoExample.png)

Is ZKP == to privacy?

No, ZKP are not equal to privacy, they are equal to honest computation. I claim "I did some work, the result is this and I can give you a proof of this". For a bitcoin applicacion, I can claim "I done a computation for a entire blockchain and I can tell you everyone balance and give you a proof that this state is correct".

There are three properties that every ZKP must satisfy: completeness, soundness and zero-knowledge. 
- Completeness: If the statement is really true and both users follow the rules properly, then the verifier would be convinced without any artificial help. 
- Soundness: If the statement is false, the verifier would not be convinced in any scenario.  
- Zero-knowledge: the verifier in every case would not know any more information. 

This protocol was first introduced by Goldwasser, Micali and Rackoff in 1985. The trio were working on a problem related to a concept called an interactive proof system. In such a system, it is assumed that the prover cannot be trusted while the verifier can be. It is the goal of the system to be designed in such a way that: 

- The verifier can be convinced of a true statement by an untrusted prover, and 
- It is impossible for the prover to convince the verifier of an untrue statement.

They added an additional layer of complexity to the whole interaction. They asked (and answered) the question: how do we handle it if, none of two parties (prover and verifier) can trust each other. Whatever the issue is, suddenly the prover does not want the verifier to know the underlying information.

There are two forms of zero knowledge: interactive and non-interactive 

- Interactive: in this form, the prover, had to perform a serious of actions to convince the verifier of a certain fact. However, there is one drawback to this technique: The proof is limited and  transferability, this means that we have to repeat the entire process if we want to convince a new verifier. 
- Non - interactive. Allow you to deliver a proof that anyone can verify by themselves, i.e, ZK - SNARK (Succinct Non-interactive Arguments of Knowledge) is used by some cryptocurrencies to protect the privacy of their users.  

That's all for this thread. Thank you for reading! 
If you liked this thread, follow me @Hasseru and retweet.

References
- https://blog.goodaudience.com/understanding-zero-knowledge-proofs-through-simple-examples-df673f796d99
- https://app.gitbook.com/s/VDeE9GzY1GcrALvhLi0f/day-1

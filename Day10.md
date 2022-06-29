# #DaysOfZeroKnowledge. Day 10.

Today we are going to talk about some highlights of the evolution of the most popular ZKP. 

Let's remember that the development of these protocols begin with publication of “The Knowledge Complexity of Interactive Proof- Systems” by Goldwasser, Micali and Rackoff. It was the first paper on zero knowledge proofs. The document explains the mathematical basis of the proofs in an informal way. At the time, zero-knowledge proofs were “horribly inefficient” due to the size of the proofs and the needed interaction between prover and verifier.

In 1988, The first publication proposing Non-Interactive Zero-Knowledge (NIZK) by Blum, Feldman, and Micali. 

1992: “A note on efficient zero-knowledge proofs and argument”, by Joe Kilian, is the first publication on succinct (i.e. small, compact) zero-knowledge proofs.

1994: Goldreich and Oren published a paper where they proposed the first succinct non-interactive zero-knowledge proof.

2006: Groth proposed the first linear size proofs. Proof sizes started getting smaller.

2011: Publication of first paper on Succinct Non-Interactive Adaptive Argument of Knowledge (SNARK).

2016: Groth proposed an algorithm that reduces significantly computational complexity of Zero-Knowledge Succinct Non-Interactive Adaptive Argument of Knowledge (zkSNARK). The fastest and smallest known zk-SNARK to the time. Used in Zcash.

2017: The publication on Bulletproofs, “non-interactive zero-knowledge proof protocol with very short proofs and without a trusted setup”.

2018: Zero-Knowledge Scalable Transparent ARguments of Knowledge (zk- STARK) are proposed. zk-STARKs are Succinct Non-Interactive Adaptive Argument of Knowledges with a transparent setup, or in other words, without a trusted setup.

2019: Zero-Knowledge Succinct Non-interactive Oecumenical aRguments of Knowledge (zkSNORK) are proposed (e.g. Sonic, Plonk . . . ). Sonic supports a universal and updatable common reference string. Proofs are constant size. However, verification is expensive. Many of the newest constructs later that year were based on Sonic. Libra protocol was also proposed, which is a protocol that yields ZKPs with linear prover time and succint proof size and verification time. However it needs a trusted setup. Its follow-up, Virgo does not require a trusted setting.

ZKP have been a part of cryptography research for almost forty years. However, the implementations for actual applications have only recently bloomed. It is incredible the fast evolution of ZKP on the last ten years, as opposed as the first three previous decades.   

That's all for this thread. Thank you for reading! If you liked this thread, follow me @Hasseru and retweet.

Reference: https://essay.utwente.nl/83802/

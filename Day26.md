

# #DaysOfZeroKnowledge. Day 26.

Last friday we talk about Groth16 which is currently the gold standard of ZKPs. Let's remember that Groth16 are not universal, in other words, proofs are specific to a given program. Changing the program means starting over, throwing out the old parameters, and generating new ones. Also, zkSNARKs rely on a common reference string (CRS) so the information used to create the CRS, called ‘toxic waste’ needs to be destroyed as soon as the CRS is created. Otherwise, it can be used by adversaries to forge fraudulent proofs.

As we mention, SNARKs have a structured setup phase with a multiparty computation (MPC) for the setup, to reduce the trust assumptions. 

![Multiparty computation](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/circom_29.png)

![Multiparty computation](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/circom_30.png)

The first family of MPC protocols for ZKPs was proposed in "Secure Sampling of Public Parameters for Succinct Zero Knowledge Proofs" by Ben-Sasson and prove that the CRS generated with these protocols is secure as long as at least one contributing party is honest. Since then, the goal of setup ceremonies has been to maximize the number of honest and independent contributors. If there are many, independent participants, then intuitively the likelihood that all are dishonest is reduced to the point of negligibility.

In 2017, Bowe introduced a second family of MPC protocols in "Scalable Multi-party Computation for zk-SNARK Parameters in the Random Beacon Model" specifically for pairing-based zk-SNARKs like Groth16. This paper aimed to address some of the drawbacks of prior schemes. 

![Multiparty computation](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/circom_31.png)

![Multiparty computation](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/circom_32.png)

Since the original publication of the paper, Powers of Tau ceremonies have become the industry standard. However, since 2017, there's been an explosion in ZKP research to try to mitigate the trusted setup requirement while still competing with Groth16 on performance. Tomorrow we are going to talk about this protocols. 

That's all for this thread. Thank you for reading! If you liked, follow me @Hasseru and retweet.

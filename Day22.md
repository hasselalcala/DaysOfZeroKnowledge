# #DaysOfZeroKnowledge. Day 22.

Today we are going to talk about the first step in generating a zero-knowledge proof requires what we call a trusted setup.

The need for a trusted setup boils down to the fact that the balance between privacy for the prover, and assurance of not cheating for the verifier, is delicate. To maintain this delicate balance, zero-knowledge protocols require the use of some randomness.

Usually, this randomness is encoded in the challenge the verifier sends to the prover, and serves to prevent the prover from cheating. The randomness however can’t be made public, because it’s essentially a backdoor to generating fake proofs. This implies that a trusted entity should generate the randomness. Hence the term trusted setup.

Now that we have a better intuition for what we are doing, let’s go ahead and create a trusted setup for our circuit (in this case, we’ll also play the role of the trusted entity).

![Setup using snarkjs](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/circom_16.png)

Before creating the proof, we need to calculate all the signals that match the constraints of the circuit. This set of signals is called the witness.

![Why do we need a witness?](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/circom_17.png)

What do we need to calculate it? Let's remenber that when we compile the circuit, we obtain the wasm code to generate the witness. We need this along with a file – let’s call it input.json – containing the inputs to the circuit.

Once we have these two files we’ll use snarkjs’s calculatewitness command to calculate the witness for us.

![What do we need to calculate it?](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/circom_18.png)

That's all for this thread. Tomorrow we are going to see an example to calculate the witness. Thank you for reading! If you liked, follow me @Hasseru and retweet.

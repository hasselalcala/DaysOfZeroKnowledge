# #DaysOfZeroKnowledge. Day 24.

On previous days, we calculate the witness and we noted that there’s nothing preventing us from using a = 1 and b = c (or vice-versa) to satisify the constraints of the circuit, for any c. Today we are going to see how to fix this by adding some extra constraints to our circuit.

The trick here is to use the property that 0 has no inverse. This insight allows us to do the following:

![Adding extra constraints](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/circom_23.png)

As a final step, we’ll convert our proof into the right format, and publish it on-chain. To generate a solidity version of the proof, we can use snarkjs generateverifier to generate a Solidity smart contract that verifies the zero knowledge proof.

![Generate a solidity version of the proof](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/circom_24.png)

To publish the proof, we can upload verifier.sol directly into Remix. Remix is an open source tool that helps you write (and publish) Solidity contracts straight from the browser. If this is your first time using it, have a look through this tutorial before continuing: https://kauri.io/#communities/Getting%20started%20with%20dapp%20development/remix-ide-your-first-smart-contract/

If you take a look inside verifier.sol you should see that it contains two contracts: Pairings and Verifier. For our purposes, we just need to deploy the Verifier contract. The verifier contract deployed has a function called verifyProof. It takes as input four parameters and returns true if the proof and the inputs are valid.

![Verify the proof](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/circom_25.png)

![Verify the proof](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/circom26.png)

That's all for this thread. Thank you for reading! If you liked, follow me @Hasseru and retweet.

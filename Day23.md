# #DaysOfZeroKnowledge. Day 23.

Today we are going to see an example to calculate the witness. For example, imagine that we want to prove that we are able to factor 33. We need to prove that we know two numbers a and b that multiply to give 33:

![Example calculate witness](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/circom_19.png)

![Example calculate witness](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/circom_20.png)

Now that we’ve generated the witness, we’re ready to create the proof.

![Create the proof](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/circom_21.png)

At this stage we would hand over both the proof.json and public.json files to the verifier. With both the proof, and the public input and outputs, we can now prove to the verifier that we know one or more private signals that satisfy the constraints of the circuit, without revealing anything about those private signals.

From the verifier’s point of view, she can verify that we know the set of private signals contained in the witness – without ever having access to it. This is the core of the magic behind zk-proofs!

![Verify the proof](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/circom_22.png)

That's all for this thread. Thank you for reading! If you liked, follow me @Hasseru and retweet.

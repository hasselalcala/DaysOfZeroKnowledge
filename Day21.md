# #DaysOfZeroKnowledge. Day 21,

Today we are going to design a circuit usign circom and snarkjs. Create (and move into) a new directory called factor where we’ll put all the files that we want to use in this guide. 

Remember, the purpose of this circuit is to allow us to prove that we know two numbers ("in1" and "in2") that multiply together to give "out", without revealing "in1" and "in2".

![Design the circuit](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/circom_12.png)

We’re now ready to compile the circuit. To do this, run the following:

![Compile the circuit](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/circom_13.png)

Now that the circuit is compiled, we can use it in snarkjs to create a proof. But first, let’s have a look at some of the information circuit.r1cs gives us.

![Information about the circuit](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/circom_14.png)

This information fits with our mental map of the circuit we designed. Remember, we had two private inputs "in1" and "in2", and one output. And the one constraint we specified was that in1 * in2 = out.

![Information about the circuit constraints](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/circom15.png)

To see a list of all snarkjs commands, as well as descriptions about their inputs and outputs, run snarkjs --help from the command line.

That's all for this thread. Tomorrow we are going to see the steps to generate the zero-knowledge proof using snarkjs. 

Thank you for reading! If you liked, follow me @Hasseru and retweet.

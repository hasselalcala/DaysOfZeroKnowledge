# #DaysOfZeroKnowledge. Day 14.

Today we are going to continue talking about the steps of transformation for zk-SNARK. Once that we have the flattening of a function and the arithmetic circuit, our next step is to build what is called a Rank 1 Constraint System, or R1CS. 

![Whats is R1CS?](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/zksnark_11.png)

There is a natural way to transform the flattened version of our code to a R1CS. First we are going to have many constraints: one for each logic gate.We need to convert a logic gate into a (a,b,c) triple depending on what the operation is and whether the arguments are variables or numbers. Then, we define a vector, which will hold the state of our program, i.e. all variables which are used in the program. Each component of this vector will be one variable and the solution s will be an assignment to each variable.

Using the example from yesterday, we have:

![R1CS example](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/zksnark_12.png)

![First gate](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/zksnark_13.png)

![Second gate](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/zksnark_14.png)

![Third gate](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/zksnark_15.png)

![Fourth gate](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/zksnark_16.png)

![R1CS result](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/zksnark17.png)

That's all for this thread. Tomorrow we are going to analyze the next step: take this R1CS and converting it into Quadratic Arithmetic Program (QAP) form.

Thank you for reading! If you liked this thread, follow me @Hasseru and retweet.

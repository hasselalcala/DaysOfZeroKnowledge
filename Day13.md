# #DaysOfZeroKnowledge. Day 13. 

Let's continue talking about the steps of transformation for zk-SNARK. Today we are going to focus on the first step: turning a function into a mathematical representation is to break down the logical steps into the smallest possible oprations, creating an "arithmetic circuit". 

Any computation at it is core consists of elemental operations of the form: 

![Single operation](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/zksnark_7.png)

This step is know as "flattening" procedure, where we convert the original code, which may contain arbitrarily complex statements and expressions, into a sequence of statements that are represented as a single operation or x = y form. For example, consider the following computation and the result flattening:  

![Computation](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/zksnark_8.png)

![Flattening procedure](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/zksnark_9.png)

The arithmetic circuit is similar to a boolean circuit. Here is an example of what an arithmetic circuit looks like for computing the example above: 

![Arithmetic circuit](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/zksnark_10.png)


The next step is to convert the above to a R1CS. Tomorrow we are going to talk about this.

That's all for this thread. Thank you for reading! If you liked this thread, follow me @Hasseru and retweet.

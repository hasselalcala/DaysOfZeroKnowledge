# #DaysOfZeroKnowledge. Day 12.

Today we are going to continue talking about zk-SNARK. To apply zk-SNARK, a computation needs to be expressed in terms of algebraic circuit, converted to a constraint system called R1CS, and then finally a form called “quadratic arithmetic program” (QAP). Eran Tromer describe the steps of transformation for zk-SNARK as follows:

![Steps of tranformation for zk-SNARK](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/zksnark_5.png)

![Steps of tranformation for zk-SNARK](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/zksnark_6.png)

Transforming the code of a function into a QAP is itself highly nontrivial and is another process that can be run alongside so that if you have an input to the code you can create a corresponding solution (sometimes called “witness” to the QAP). After this, there is another fairly intricate process for creating the actual “zero knowledge proof” for this witness, and a separate process for verifying a proof that someone else passes along to you.

The next days we are going to digs deeper into the machinery behind the technology, and tries to explain as well as possible the first half of the pipeline.

That's all for this thread. 
Thank you for reading! If you liked this thread, follow me @Hasseru and retweet.

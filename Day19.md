# #DaysOfZeroKnowledge. Day 19.

Let's continue learning more about circom. Another important thing in circom is that we build circuits combining templates and creating components from other components. For example: 

![Subcomponents and variables](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/circom_07.png)

As we have said, a circom program has two representations: the constraints and the executable code. The compiler does not check whether they are related or not. If <-- is not used (or only in library templates) we are safe. Otherwise, it is the programmer’s responsibility to show that the code is safe: both express (exactly) the same relation between the signals of the circuit the computed witness must be the only solution to the constraints.

Circom also provides a library that contains the implementation of useful circuits that can be used as primitive templates. Such as:

![circomlib](https://raw.githubusercontent.com/hasselalcala/DaysOfZeroKnowledge/main/images/circom_08.png)


That's all for this thread, tomorrow we will continue learning more about circom. Thank you for reading! If you liked, follow me @Hasseru and retweet.

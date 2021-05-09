# SmartContractsStructures 01
----
![Supply Image](Images/ethereum_solidity.jpg)

### My First Contract

I am trying to simplify solidity and show how to build it step by step. 
I am using Dapp University and freeCodeCamp.org to build the building blocks step by step.(https://www.youtube.com/watch?v=ipwxYa-F1uY&t=2358s)

----
### How to find errors and how to solve them?

![Supply Image](Images/one.gif)

The above Gif Image shows once you compile the above simple, smart contract, you get errors in lines 7 and 8. Line 7 says 

#### " Did you intend to add "public" ? function get() 

This means we need to add "public." or if it is private we can add "private" after the get().

But its still give an error on line 8.

![image](https://user-images.githubusercontent.com/71329902/115631370-8a217f80-a2ba-11eb-832f-891210421384.png)

The error says,

![image](https://user-images.githubusercontent.com/71329902/115631491-c7860d00-a2ba-11eb-995f-6142467fef61.png)

The above error means there are many arguments, which means the solidity compiler didn't know the return value is a string, integer, etc.( VAR), So we need to change that public returns(string) as show below, but still it gives an warning.

![image](https://user-images.githubusercontent.com/71329902/115632272-36179a80-a2bc-11eb-8355-8aa7aedd5e53.png) 

and the warning says,

![image](https://user-images.githubusercontent.com/71329902/115632313-49c30100-a2bc-11eb-8af8-3d9399959d2f.png)

This simply means we cant view the string value after we deply it, so we add "view" before returns.

Finally we can compile it and depoly it as below.

![Supply Image](Images/two.gif)

### How to ADD set function ?

When you add "set" function, the argument of adding set fuction is to change value to another value, or set a value. 

You can see your value in your get function. the compiler and deployer looks like below. 

![Supply Image](Images/three.gif)

### Also, we can add optional fuction called " constructor "

https://www.tutorialspoint.com/solidity/solidity_constructors.htm

A contract can have only one constructor.

A constructor code is executed once when a contract is created and it is used to initialize contract state.

After a constructor code executed, the final code is deployed to blockchain. This code include public functions and code reachable through public functions. Constructor code or any internal method used only by constructor are not included in final code.

A constructor can be either public or internal.

A internal constructor marks the contract as abstract.

In case, no constructor is defined, a default constructor is present in the contract.

![Supply Image](Images/four.gif)

So thats it, this is the most simple smart contract.. To be continue see SmartContractsStructures Part II
https://github.com/dmkskasun/Smart_Contract_Structures_Part_2.git









# VotingContract
A smart contract in Solidity that uses the require(), assert(), and revert() statements.

License
This contract is using the MIT License.

Prerequisites
The pragma Solidity ^0.8.17.

Error Handling Control
This is a Solidity smart contract that demonstrates different error handling techniques using assert, revert, and require functions.

The ErrorHandling contract provides the following functions:
1.assert() function(uint number):
The assert() function checks if a condition is true and throws an error if it is not true.

2.revert() function:
The revert() function reverts all changes made to the state and stops execution of the contract.

3.require() function:
The require() function checks if a condition is true and throws an error if it is not true.

4.mult (uint a):
The mult() function takes an input parameter a and returns the product of a and the variable b. It first checks if a is greater than zero using the require statement.

If the condition fails, it reverts the transaction with a custom error message stating that the value of a should not be zero.

If the condition is met, it returns the result of the multiplication.

divide(uint numerator, uint denominator)
It takes an a parameter and performs multiplication with a predefined constant b.

It first checks if a is greater than zero using the require statement.

If the condition fails, it reverts the transaction with a custom error message stating that the value of a should not be zero. If the condition is met, it returns the result of the multiplication.

Usage
Make sure you have Solidity ^0.8.17 installed.

Compile and deploy the ErrorHandling contract to a supported Ethereum network.

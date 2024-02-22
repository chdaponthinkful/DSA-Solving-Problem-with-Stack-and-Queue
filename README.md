# 1.3.9  DSA-Solving-Problem-with-Stack-and-Queue

A simple algorithm may be outlined as follows:

Import the necessary modules: path and Stack.
Declare a constant named operator and assign an object with properties: +, -, *, and /, each corresponding to a function that takes two operands and returns the result of the corresponding operation.
Declare a function named evaluate that takes an expression as a parameter.
Create a new instance of the Stack class and assign it to a variable named stack.
Remove any whitespace from the input expression.
Iterate over each character in the expression and do the following:
If the character is one of the operators +, -, *, or /:
Pop the top two values from the stack (considered as right and left operands) and assign them to variables right and left.
Apply the corresponding operator function to the operands and push the result back onto the stack.
Otherwise (if the character is a number or operand):
Push the character onto the stack.
Convert the final result on the stack to a number and return it.
Export the evaluate function for use in other modules.
Implement your solution in the file named src/postfix.js.

Generate binary numbers
Given a number max, write an algorithm that generates all binary integers from 1 to max.

Examples:

Input: max = 2
Output: ["1", "10"]

Input: max = 5
Output: ["1", "10", "11", "100", "101"]
An algorithm that uses a queue to solve the problem is given below.

Initialize an empty queue.
Enqueue the string 1. This represents binary number 1.
Initialize an empty array named result.
Iterate from 1 to max and do the following:
Dequeue a value from the queue.
Push the value into result.
Append a 0 to the value and enqueue it.
Append a 1 to the value and enqueue it.
Return result.
Implement your solution in the file named src/binary.js.

Extend parentheses to other types of brackets
Recall the algorithm that was used to determine if a given expression contained matching parentheses. It is repeated in pseudocode below:

Initialize a new empty stack
Start a loop to iterate through each character in the expression
If the current character is (
Push it onto the stack
Else
If the current character is (
If the stack is not empty
Pop one item off the stack
Else
Return false
If the stack is empty
Return true
Else
Return false
Extend the algorithm to recognize 3 different types of brackets: (), [], and {}. These must be correctly nested; "([)]" is incorrect and should return false.

Implement your solution in the file named src/brackets.js.

# Dijkstra's Two Stack Algorithm

Goal: Evaluate infix expressions.

Algorithm:
* Loop from left to right
* If Value: push onto the valeu stack.
* If Operator: push onto the operator stack.
* Left parenthesis: ignore.
* Right parenthesis: pop operator and two values; push the result of applying that operator to those values onto the operand stack.

Example 

`( 1 + ( ( 2 + 3 ) * ( 4 * 5 ) ) )`

Outputs: 101.0

Context: Useful for interpreters, demonstrating fundamental value of Stacks.

## Java Implementation

![Alt text](./Dijkstras-Two-Stack-Java-Implementation.png)raw=true "Title")

# Java-Linked-List-Stack-Vs-Array

In Java you have 2 different implentations of a Stack, either using a Linked List or an Array.

The Stack is going to be slower on average but can guarantee constant time in the worst case. 

Using a resizing-array you'll get constant amortized time, getting very fast push and pops, but ocassionally using more time when the array needs to resize.

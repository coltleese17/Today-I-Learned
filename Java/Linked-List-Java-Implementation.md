# Linked-List-Java-Implementation

Tho a linked list can be constant time, the Java utils LinkedList.get() actually runs in linear time because the class extends the Iterable, which requires a linear iterator method.

If you want constant time, potentially implement your own constant time solution for your data type specifically.

In contrast, an Arraylist has constant time lookup, but linear lookup for inserts/deletes. LinkedList has constant deletes/insertion.


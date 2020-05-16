# The Ugly Cast

Java does not allow array creation of a generic type. For example:

```
public class GenericArray<Item>{

private Item[] s;

s = new Item[size];
```

Instead, you have to cast it after you make an array of Object type, like so:

```
s = (Item[]) new Object[size];
```

This is ugly and not ideal but required in Java. In general casting is not preferred.

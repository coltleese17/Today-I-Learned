# Linked Hash Table ( LRU Cache )

The basic structure of a LRU cache is a Hashmap which takes a key K, and a value which is a pointer to a node<k,v>.

This allows constant time lookup while also linking the items.

This concept allows us to keep track of the least recently used items.

The Linked List keeps track of head/tail.

You instantiate with the capacity size.

The basic functions are Read, Write, with add and remove as helper functions.

public V read(K key){

    //update the position since its been used most recently now
    removes the node from the current list
    add the node to the end

    returns the value of the node,
}

public void write(k key, v value){
    (if map.size == capacity) { remove(head.getKey())}
    add(key,value);
}

public add(K, V){
     Create new node with K V
     appendToLinkList(node);
     map.put(k, newNode)}

public remove(K) {
  if doesnt contain key, return null
  Node toRemove = map.get(key);
  removeFromLinkedList(toRemove);
  map.remove(key)
}


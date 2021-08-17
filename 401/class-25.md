#  Hash Tables

Terminology:

- Hash : Hashing is the process of transforming any given key or a string of characters into another value. That value could be used for either security or some other purpose.
- Buckets : A bucket is the container in the array of hashtable. Each index in hashtable is a buckets, and each bucket could contain multiple key/value pairs if a collision occurs.
- Collisions : A collision is when we have more than one key gets hashed to same index in hashtable.
- Hash Function : Hashing is the process of running data through a hash function. A hash function is a mapping between a set of input values and a set of integers, known as hash values.
- Separate Chaining : Separate chaining is a method for dealing with collisions. The hash table is an array of linked lists. Data elements that hash to the same value are stored in a linked list originating from the index equivalent of their hash value.
- Linear Probing : Linear probing is one method for dealing with collisions. If a data element hashes to a location in the table that is already occupied, the table is searched consecutively from that location until an open location is found.
- Linked List : A list data structure made up of nodes, each of which holds a pointer to the next list element.
# HashTables  

A data structure that is used to store information. The information in the hash table has two main components, a key and a value. 

A way to implement an associative array. 


#### Hash: A hash is the result of some algorithm taking an inomcin string and converting it into a value that could be used for either security or some other purpose. In the case of a hastable, it is used to determine the index of the array.

#### Buckets: A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.

#### Collisions: A collision is what happens when more than one key gets hashed into the same location of the hastable.

### Why do we use them 

1. Hold unique values
2. Dictionary
3. Libarary

### What are they 

Has tables are data stucture. that utilize key value pairs. This means every `Node` or `Bucket` has both a key, and a value.

`hash` is the ability to encode the key that will eventaully map to a specific location int he data stucture that we can look directly to retrieve tha vlaue. 

**Hash map  has `O(1) access`**

#### Hash Code Examples 

![preorder](/401-notes/assets/hash.png)  


### Methods

`set()` 

WHen adding a new key/value pair to a hashtable:

  1. send the key to the `hash()` method
  2. Once you determine the index of where it should be placed go to that index
  3. Check if something exists at that index already, if it doesn't, add it with the key/value pair
  4. If something does exist, add the new key/value pair to the data structure within that bucket


get()

The `get()` method takes in a key, gets the Hash, and goes to the index location specified. Once at the index location is found in the array, it is then the responsibility of the algorithm the iterate through the bucket and see if the key exists and return the value.

has()

The `has()` method will accept a key, and return a bool on if that key exists inside the hashtable. The best way to do this is to have the contains call the hash() method and check the hashtable if the key exists in the table given the index returned.

keys()

The `keys()` method returns a collection (array) of unique hash keys.

hash()

The `hash()` method will accept a key as a string, conduct the hash, and then return the index of the array where the key/value should be placed.
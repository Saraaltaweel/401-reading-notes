## Hash Tables

### Hash
*A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. it is used to determine the index of the array*

### Buckets
*A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs*

### Collisions
*A collision is what happens when more than one key gets hashed to the same location of the hashtable*

### Why do we use them?
- *Hold unique values*
- *Dictionary*
- *Library*

### Creating a Hash
- *Hashtable traditionally is created from an array*
- *After you've created your array, do some sort of logic to turn that "key" into a numeric number value (example: Add or multiply all the ASCII values together, Multiply it by a prime number such as 599, Use modulo to get the remainder of the result, when divided by the total size of the array, Insert into the array at that index)*
- *Each index of the array can hold many types of values*
- *Each index of the array contain “buckets”, and each of these “buckets” holds one key/value pair combination*
- *When there is no entry in a specific bucket, the buckets (each index of the array) all start null*
- *The hash table starts each bucket empty and overwrites their value once a key generates a hash code that corresponds with an index*

### Bucket Sizes
*Hash Maps can have any number of buckets. If a hash map has only a few buckets it will be densely full and have many collisions. If a hash map has more buckets it will be more sparsely populated, there will be less collisions, but there may be a lot of extra empty space*
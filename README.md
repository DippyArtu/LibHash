# LibHash

**LibHash is a dynamic hash table implementation with a generic string hashing algorithm for the C language.**

Collisions are handled using open addressing with double hashing.
The size of the table will automatically grow or shrink depending on the usage.

## Usage

 - Compile and use LibHash as a library.
 - **#include "hash_table.h"** in your code

## API
|Declaration|Description  |Return|
|--|--|--|
|`t_hash_table *ht_new(void);`  | Creates a new hash table |A pointer to the hash table created
  |`void ht_insert(t_hash_table *ht, const char *key, const char *value);` |Inserts a key-value pair in the table; If the *ht_insert* is called with an existing key, it's value will be updated | None |
  |`char *ht_search(t_hash_table *ht, const char *key);`|Searches for the key in the table|Returns the *value*, associated with the key or *NULL* if the key is not found |
  |`void ht_delete(t_hash_table *ht, const char *key);`|Deletes a key-value pair from the table|None|
  |`void ht_del_table(t_hash_table *ht);`|Deletes the hash table| None


Feel free to modify the code to suit your needs

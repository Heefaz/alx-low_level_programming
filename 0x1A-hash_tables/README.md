0x1A Hash Tables

In this project, I have learnt about hashing by implementing hash functions and hash tables in C.

## Tests :heavy_check_mark:

* [tests](./tests): Folder of test files.

## Header File :file_folder:

* [hash_tables.h](./hash_tables.h): Header file contains definitions and prototypes for all types and functions written for the project.

Data Structures:
```
typedef struct hash_node_s
{
	char *key;
	char *value;
	struct hash_node_s *next;
} hash_node_t;

typedef struct hash_table_s
{
	unsigned long int size;
	hash_node_t **array;
} hash_table_t;

typedef struct shash_node_s
{
	char *key;
	char *value;
	struct shash_node_s *next;
	struct shash_node_s *sprev;
	struct shash_node_s *snext;
} shash_node_t;

typedef struct shash_table_s
{
	unsigned long int size;
	shash_node_t **array;
	shash_node_t *shead;
	shash_node_t *stail;
} shash_table_t;
```

## Tasks :page_with_curl:

* **0. >>> ht = {}**
* **1. djb2**
* **2. key -> index**
* **3. >>> ht['betty'] = 'holberton'**
* **4. >>> ht['betty']**
* **5. >>> print(ht)**
* **6. >>> del ht**
* **7. $ht['Betty'] = 'Holberton'**

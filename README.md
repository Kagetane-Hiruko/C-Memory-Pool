# C-Memory-Pool
Utility library for C/C++ programming language, that provides functions for creating efficient memory pools.

## Functions

* create_memory_pool
```cpp

// Function for creating memory pool
// Params: size of some type, number of memory blocks	
	
memory_pool_t * mempool = create_memory_pool(sizeof(int), 4);


```
* allocate_memory_pool
```cpp

// This function will return next free memory address from created memory pool. If there are 0 free memory blocks it will return NULL.
// Params: existing memory pool
	
int * variable = (int *) allocate_memory_pool(mempool);


```
* deallocate_memory_pool
```cpp

// 	This function will deallocate given memory block from memory pool if it exeists there.
// Params: existing memory pool, memory block from pool
	
deallocate_memory_pool(mempool, variable);


```
* delete_memory_pool
```cpp

// This function will delete given memory pool if it exists.
// Params: existing memory pool
	
delete_memory_pool(mempool);


```




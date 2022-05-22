# Data Structures
## Linked Lists
Types:
- Single
- Double

### Single
- Grows dynamically
- Access to find something in the list is O(n)
- Add at head is O(1) as it is just an assignment
- Add at the end is O(n) since you have to follow all pointers to get to the end
- Only 1 pointer so less memory

### Double
- Access is O(n)
- 2 nodes so more memory
- Good for LRU

## Binary Trees
- Has 1 root node
- Has a left and right node
- Access is O(log(n)) but could be O(n) if structure is like linked list

## Hash Table
- Key/Value lookup
- Uses a hash function to place a value into an index
- If there are collisions, then chaining (linked list) could be used
- Runtime and lookup is O(1) but could be O(n)

## Graphs
- Nodes connected with other nodes connected by edges
- Useful for social networks
- Access is O(V+E)

# Algorithms
## Linear Search
- Start at the beginning and search to the end one by one
- O(n)

## Binary Search
- Sort array/list
- Split array in two
- O(log(n))

## Sorting Algorithm
- Insertion sort
	- search through until found then insert
	- O(n) to O(n^2)
- Merge sort
	- ![[Pasted image 20220522135349.png]]
- Quicksort
	- Find a pivot, have left and right pointer, compare pointer, rearrange
	- O(log(n)) to O(n^2)
 


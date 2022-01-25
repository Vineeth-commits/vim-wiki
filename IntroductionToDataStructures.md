## Introduction to data Structures
---
* Data structures is a collection of data items so that they can utilize operations on data effectively.
* The effective operations on data items are done inside the main memory.
* Data base is the arrangement of data like a relational model in the HDD storage.
* Data warehouse contains large amount of legacy data (historical data) stored.
* Storing and utilizing the abundent data to study is big data.

## Stack vs Heap memory
---
* The main memory is divided into smaller parts called segments.
* The main memory contains linear addresses.
* The main memory is divided into - Heap, stack and code section
* The variables defined in a function is stored in the stack and the portion of this memory given to the function is called as activation record of the function. This is static memory allocation.
* Since the amount of bytes required to store is decided during the compile time, it is called static memory allocation.
* Check out why stack memory is called "stack"?
* Heap memory is an unorganised memory while the stack memory is organised.
* Heap memory is treated like a resource. It should be accessed and then deleted after the task is finished.
* Code cant access heap memory directly
* Example(heap memory allocation)
    ```C
    void main()
    {
        int *p;
        p =(int *)malloc(sizeof(int)*5); /* or p = new int[5] in C++ */
        delete []p; /* Deletes the memory allocated */
        p = NULL; /* Doesnt point to the heap memory */
    }
    ```
## Physical vs Logical Data structures
---
* Physical Data structures - The following is called physical because of how the memory is organised and allocated
    * Array - Homogeneous and fixed memory. It is created in stack and heap. They are stored in consecutive memory locations.
    * Linked list - variable length(dynamic memory). It is created in heap.
* Logical Data structures - Logical Data structures are implemented by the physical data structures.
    * Stack(linear) - Last in First Out
    * Queues(linear) - First in First out
    * Trees(non-linear) - data structure which consists of a collection of nodes arranged in a hierarchical order. One of the nodes is designated as the root node, and the remaining nodes can be partitioned into disjoint sets such that each set is a sub-tree of the root.
    * Graph(non-linear) - data structure which is a collection of vertices (also called nodes) and edges that connect these vertices. A graph is often viewed as a generalization of the tree structure, where instead of a purely parent-to-child relationship between tree nodes, any kind of complex relationships between the nodes can exist.
    * Hash table(tabular)

## Abstract DataType (ADT)
---
* An abstract data type (ADT) is the way we look at a data structure, focusing on what it does and ignoring how it does its job.
* Data type is defined on two terms - representation of data and operations on data
* Representation on data is done by - 
    * space for storing element
    * capacity
    * size
* Operations that can be performed - 
    * add() / insertion()
    * remove() / deletion()
    * search()
    * traversing()
    * sorting()
    * merging()
## Time and Space complexity
---
* Time complexity is done by taking the highest degree of a polynomial
    * order of n or O(n)
    * O(n^2)
    * If the elements of being divided into half(1/2) every time, it is O(log2(n))
    * When processing all the elements in a matrice, it is O(n^2)
    * For swapping, it is O(1)
* The Time taken by the function1 which in turn is calling a function2 will be the time taken by the function.
* The time complexity of an algorithm is basically the running time of the program as a function of the input size.
* The space complexity of an algorithm is the amount of computer memory required during the program execution as a function of the input size.
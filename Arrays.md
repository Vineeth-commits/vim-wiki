# Arrays
---
* Array is a collection of similar data elements grouped under one name which are contiguous.
* Static array -
    int a[] = {1,2,3};*/
* Dynamic array -
    int *p;
    p = (int *)malloc(3*sizeof(int))
    p[0] = 1;
    p[1] = 5;
    p[2] = 32;
    free(p); // deleting memory
* Different ways of accessing the memory - A[2] or 2[A] or *(A+2)
* The size of the array can be increased or decreased only in the heap and not in stack.
* The size of the array can be increased or decreased only by creating a new array and transferring all the data to the newly created array.
* The size of the array cant be altered as they are stored in contiguous in the memory. Since the immediate next memory location may be occupied by other objects.
* Example to increase the size of a dynamic array
    int *p = (int *)malloc(2*sizeof(int));
    p[0] = 5;
    p[1] = 3;
    int *q = (int *)malloc(4*sizeof(int));
    for(int i = 0;i<2;i++)
    {
        q[i] = p[i];
    }
    free(p);
    p = q;
    q = NULL;
* In memory, 2D arrays are stored like a single dimension array.
* Declaration of dynamic 2D arrays
    Method 1:
        // array of pointers in the stack while actual values in the heap
        int *A[3]; //array of integer pointers
        A[0] = (int *)malloc(3*sizeof(int));
        A[1] = (int *)malloc(4*sizeof(int));
        A[2] = (int *)malloc(2*sizeof(int));
        A[1][2] = 4; //accessing
    Method 2:
        // double pointer in the stack
        int **A;
        A = (int **)malloc(2*sizeof(int));
        A[0] = (int *)malloc(3*sizeof(int));
        A[1] = (int *)malloc(4*sizeof(int));
* Address(A[i]) = L + i * w
    where L is the base Address, i is the index and w is the size of the datatype
* The reason why array begins from 0 and not 1 is to increase the performance. An extra operation (i-1) is done when an array begins from 1 while this can be neglected if it begins from 0.
* Row major, Address(A[i][j]) = L + [i*n + j] * w, where n is the number of columns
* Column major, Address(A[i][j]) = L + [j * m + i]*w, where m is the number of rows
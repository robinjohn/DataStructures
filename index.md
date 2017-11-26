Source Code for Data Structures and Algorithm Analysis in C++ (Second Edition)

Source Code for Data Structures and Algorithm Analysis in C++ (Second Edition)
==============================================================================

Here is the source code for *Data Structures and Algorithm Analysis in C++ (Second Edition),* by Mark Allen Weiss. **The materials here are copyrighted.**

**I have successfully compiled and tested the programs under Borland 5.0, Visual C++ 5.0 and 6.0, CodeWarrior Pro Release 2 (Windows), g++ 2.7.2 and 2.8.1, and SunPro 4.1. Greg Ozbirn from U.T. Dallas has rewritten the code using ANSI C++. This mostly involves fixing the header files. [Click here to obtain the ANSI C++ conversion](ansi)**

Known Bugs
----------

-   `TestCursorList.cpp` does not compile under g++ 2.7.2. I think it is a problem with static template members, which g++ does not understand until g++ 2.8.1.
-   Metrowerks insists on compiling the STL, which causes conflicts for `swap` and `merge` in `Sort.h`. Also, it does not understand default template parameters, making its `vector` and `string` incompatible with some of the code. The easy fix is to add preprocessor macros as follows: in `vector.h`, `#define vector Vector`; similarly for `string.h` and in `Sort.h`. This works as long as `iostream.h` is **included prior to the other header files**, as is done in the online code.

Compilation Instructions
------------------------

Here are compilation instructions for [g++](g++.txt), [SunPro](compileSun.txt), [Borland 5.0](compileBorland.bat), and [Visual 5.0](compileVisual.bat). (How to setup Windows for Visual [command line compilation](visualsetup.txt).) You can use this to guide you on how to generate project files for Visual C++. Throughout I am assuming 32-bit ints. All template classes have the header file include the .cpp file, even though this defeats the purpose of separate compilation. There are ways around this, but I'd rather keep everything simple for now. Jeffrey Walton has supplied some [common workarounds for C++ compilers](http://www.cs.fiu.edu/~weiss/Deltoid/workaround.html). Finally, here is a [zip file that contains CodeWarrior projects](CodeWarriorProjects.zip). You'll have to get everything in the correct directories. (Does not include some late additions from Chapter 1; check back later).

Complete Bundle
---------------

-   [Unix tar | gzip](CodeUnix.tar.gz)
-   [Unix tar](CodeUnix.tar)
-   Note to Macintosh users: There is a utility to read zip files. Click [here to download](http://www.javaworld.com/javaworld/ftp/mactools/macgzip.hqx).

Individual Files
----------------

[**mystring.h**: If you don't have a string type](mystring.h)

[**string.cpp**: If you don't have a string type](string.cpp)

[**vector.h**: If you don't have a vector type](vector.h)

[**vector.cpp**: If you don't have a vector type](vector.cpp)

[**matrix.h**: Simple matrix class](matrix.h)

[**dsexceptions.h**: Simple exception classes](dsexceptions.h)

[**Fig01\_02.cpp**: A simple recursive routine with a test program](Fig01_02.cpp)

[**Fig01\_03.cpp**: An example of infinite recursion](Fig01_03.cpp)

[**Fig01\_04.cpp**: Recursive routine to print numbers, with a test program](Fig01_04.cpp)

[**Fig01\_05.cpp**: Simplest IntCell class, with a test program](Fig01_05.cpp)

[**Fig01\_06.cpp**: IntCell class with a few extras, with a test program](Fig01_06.cpp)

[**IntCell.h**: IntCell class interface (Fig 1.7)](IntCell.h)

[**IntCell.cpp**: IntCell class implementation (Fig 1.8)](IntCell.cpp)

[**TestIntCell.cpp**: IntCell test program (Fig 1.9)](TestIntCell.cpp)

[**Fig01\_10.cpp**: Illustration of using the vector class](Fig01_10.cpp)

[**Fig01\_11.cpp**: Dynamically allocating an IntCell object (lame)](Fig01_11.cpp)

[**BuggyIntCell.cpp**: Buggy IntCell class implementation (Figs 1.14 and 1.15)](BuggyIntCell.cpp)

[**Fig01\_16.cpp**: IntCell class with pointers and Big Three](Fig01_16.cpp)

[**FindMax.cpp**: Function template FindMax (Figs 1.17 and 1.18)](FindMax.cpp)

[**Fig01\_19.cpp**: MemoryCell class template without separation](Fig01_19.cpp)

[**MemoryCell.h**: MemoryCell class interface (Fig 1.20)](MemoryCell.h)

[**MemoryCell.cpp**: MemoryCell class implementation (Fig 1.21)](MemoryCell.cpp)

[**TestMemoryCell.cpp**: MemoryCell test program (Fig 1.22)](TestMemoryCell.cpp)

[**Fig01\_23.cpp**: Using Comparable templates: Employee class example](Fig01_23.cpp)

[**MaxSumTest.cpp**: Various maximum subsequence sum algorithms](MaxSumTest.cpp)

[**Fig02\_09.cpp**: Test program for binary search](Fig02_09.cpp)

[**Fig02\_10.cpp**: Euclid's algorithm, with a test program](Fig02_10.cpp)

[**Fig02\_11.cpp**: Recursive exponentiation algorithm, with a test program](Fig02_11.cpp)

[**LinkedList.h**: Header file for linked list](LinkedList.h)

[**LinkedList.cpp**: Implementation for linked list](LinkedList.cpp)

[**TestLinkedList.cpp**: Test program for linked list package](TestLinkedList.cpp)

[**Polynomial.cpp**: Polynomials](Polynomial.cpp)

[**CursorList.h**: Header file for cursor linked list](CursorList.h)

[**CursorList.cpp**: Implementation for cursor linked list](CursorList.cpp)

[**TestCursorList.cpp**: Test program for cursor implementation of linked lists](TestCursorList.cpp)

[**StackAr.h**: Header file for stack: array version](StackAr.h)

[**StackAr.cpp**: Implementation for stack: array version](StackAr.cpp)

[**TestStackAr.cpp**: Test program for (array-based) stacks](TestStackAr.cpp)

[**StackLi.h**: Header file for stack: list version](StackLi.h)

[**StackLi.cpp**: Implementation for stack: list version](StackLi.cpp)

[**TestStackLi.cpp**: Test program for (list-based) stacks](TestStackLi.cpp)

[**QueueAr.h**: Header file for queue: array version](QueueAr.h)

[**QueueAr.cpp**: Implementation for queue: array version](QueueAr.cpp)

[**TestQueueAr.cpp**: Test program for queues](TestQueueAr.cpp)

[**BinarySearchTree.h**: Header file for binary search tree](BinarySearchTree.h)

[**BinarySearchTree.cpp**: Implementation for binary search tree](BinarySearchTree.cpp)

[**TestBinarySearchTree.cpp**: Test program for binary search tree](TestBinarySearchTree.cpp)

[**AvlTree.h**: Header file for AVL tree](AvlTree.h)

[**AvlTree.cpp**: Implementation for AVL tree](AvlTree.cpp)

[**TestAvlTree.cpp**: Test program for AVL trees](TestAvlTree.cpp)

[**SeparateChaining.h**: Header file for separate chaining](SeparateChaining.h)

[**SeparateChaining.cpp**: Implementation for separate chaining](SeparateChaining.cpp)

[**TestSeparateChaining.cpp**: Test program for separate chaining hash tables](TestSeparateChaining.cpp)

[**QuadraticProbing.h**: Header file for quadratic probing hash table](QuadraticProbing.h)

[**QuadraticProbing.cpp**: Implementation for quadratic probing hash table](QuadraticProbing.cpp)

[**TestQuadraticProbing.cpp**: Test program for quadratic probing hash tables](TestQuadraticProbing.cpp)

[**BinaryHeap.h**: Header file for binary heap](BinaryHeap.h)

[**BinaryHeap.cpp**: Implementation for binary heap](BinaryHeap.cpp)

[**TestBinaryHeap.cpp**: Test program for binary heaps](TestBinaryHeap.cpp)

[**LeftistHeap.h**: Header file for leftist heap](LeftistHeap.h)

[**LeftistHeap.cpp**: Implementation for leftist heap](LeftistHeap.cpp)

[**TestLeftistHeap.cpp**: Test program for leftist heaps](TestLeftistHeap.cpp)

[**BinomialQueue.h**: Header file for binomial queue](BinomialQueue.h)

[**BinomialQueue.cpp**: Implementation for binomial queue](BinomialQueue.cpp)

[**TestBinomialQueue.cpp**: Test program for binomial queues](TestBinomialQueue.cpp)

[**Sort.h**: A collection of sorting and selection routines](Sort.h)

[**TestSort.cpp**: Test program for sorting and selection routines](TestSort.cpp)

[**DisjSets.h**: Header file for disjoint sets algorithms](DisjSets.h)

[**DisjSets.cpp**: Efficient implementation of disjoint sets algorithm](DisjSets.cpp)

[**TestFastDisjSets.cpp**: Test program for disjoint sets algorithm](TestFastDisjSets.cpp)

[**Fig10\_38.cpp**: Simple matrix multiplication algorithm with a test program](Fig10_38.cpp)

[**Fig10\_40.cpp**: Algorithms to compute Fibonacci numbers](Fig10_40.cpp)

[**Fig10\_43.cpp**: Inefficient recursive algorithm (see text)](Fig10_43.cpp)

[**Fig10\_45.cpp**: Better algorithm to replace fig10\_43.c (see text)](Fig10_45.cpp)

[**Fig10\_46.cpp**: Dynamic programming algorithm for optimal chain matrix multiplication, with a test program](Fig10_46.cpp)

[**Fig10\_53.cpp**: All-pairs algorithm, with a test program](Fig10_53.cpp)

[**Random.h**: Header file for random number class](Random.h)

[**Random.cpp**: Implementation for random number class](Random.cpp)

[**TestRandom.cpp**: Test program for random number class](TestRandom.cpp)

[**Fig10\_62.cpp**: Randomized primality testing algorithm, with a test program](Fig10_62.cpp)

[**SplayTree.h**: Header file for top-down splay tree](SplayTree.h)

[**SplayTree.cpp**: Implementation for top-down splay tree](SplayTree.cpp)

[**TestSplayTree.cpp**: Test program for splay trees](TestSplayTree.cpp)

[**DSL.h**: Header file for deterministic skip list](DSL.h)

[**DSL.cpp**: Implementation for deterministic skip list](DSL.cpp)

[**TestDSL.cpp**: Test program for determinstic skip lists](TestDSL.cpp)

[**RedBlackTree.h**: Header file for top-down red black tree](RedBlackTree.h)

[**RedBlackTree.cpp**: Implementation for top-down red black tree](RedBlackTree.cpp)

[**TestRedBlackTree.cpp**: Test program for red black trees](TestRedBlackTree.cpp)

[**Treap.h**: Header file for treap](Treap.h)

[**Treap.cpp**: Implementation for treap](Treap.cpp)

[**TestTreap.cpp**: Test program for treap](TestTreap.cpp)

[**AATree.h**: Header file for AA-tree](AATree.h)

[**AATree.cpp**: Implementation for AA-tree](AATree.cpp)

[**TestAATree.cpp**: Test program for AA-trees](TestAATree.cpp)

[**KdTree.cpp**: Implementation and test program for k-d trees](KdTree.cpp)

[**PairingHeap.h**: Header file for pairing heap](PairingHeap.h)

[**PairingHeap.cpp**: Implementation for pairing heap](PairingHeap.cpp)

[**TestPairingHeap.cpp**: Test program for pairing heaps](TestPairingHeap.cpp)

[**FigA\_04.cpp**: Example of push\_back with vectors](FigA_04.cpp)

[**FigA\_05.cpp**: Queue implemented with STL list](FigA_05.cpp)

[**FigA\_06.cpp**: Example of set with reverse order](FigA_06.cpp)

[**Concordance1.cpp**: Concordance program using STL](Concordance1.cpp)

[**Concordance2.cpp**: Concordance program not using STL](Concordance2.cpp)

[**Graph1.cpp**: Shortest path program using STL](Graph1.cpp)

[**Graph2.cpp**: Shortest path program not using STL](Graph2.cpp)

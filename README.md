Download link :https://programming.engineering/product/homework-3-binary-search-tree/

# Homework-3-Binary-Search-Tree
Homework 3: Binary Search Tree
You are to code a binary search tree, BST, which is a collection of nodes, each having a data item and a reference pointing to a left and a right child nodes. The BST must follow the order property: for any given node, its left child’s data and all of its children’s data must be less than the current node while its right child’s data and all of its children’s data must be greater than the current node. In order to compare the data, all elements added to the tree must implement Java’s generic Comparable interface.

It will have two constructors: a no-argument constructor (which should initialize an empty tree), and a constructor that takes in a collection of data to be added to the tree, and initializes the tree with this collection of data.

You may import Java’s LinkedList/ArrayList classes for the 4 traversal methods, but only use them in these methods.

Recursion

Since trees are naturally recursive structures, all methods that are not O(1) must be implemented recursively, except for level order traversal. You’ll also notice that a lot of the public method stubs we’ve provided do not contain the parameters necessary for recursion to work, so these public methods act as “wrapper methods” for the user to use. You will have to write private recursive helper methods and call them in these wrapper methods. All of these helper methods must be private. To reiterate, do not change the method headers for the provided methods.

For methods that change the structure of the tree in some way, we highly recommend you use a technique taught in class called pointer reinforcement. It is not required, but it will make the homework cleaner, and it’ll also help greatly when we get to a later homework.

Nodes

The binary search tree consists of nodes. A class BSTNode is provided to you. BSTNode has getter and setter methods to access and mutate the structure of the nodes.

Methods

You will implement all standard methods for a Java data structure (add, remove, etc.) in addition to a few other methods (such as traversals). You must follow the requirements stated in the javadocs of each method you implement.

Traversals

You will implement 4 different ways of traversing a tree: pre-order traversal, in-order traversal, post-order traversal, and level-order traversal. The first 3 MUST be implemented recursively; level-order is best implemented iteratively. For a level-order traversal, you may use Java’s Queue interface (and an implementing class for it such as LinkedList).

Height

You will implement a method to calculate the height of the tree. The height of the tree is defined as the height of its root. The height of any given node is max(left node’s height, right node’s height)

1. When doing this calculation, a leaf node has a height of 0 and a null node has a height of -1.

Homework 3: BST Due: See Canvas

Comparable

As stated, the data in the BST must implement the Comparable interface. As you’ll see in the files, the generic typing of the BST and BSTNode classes will enforce this Comparable data requirement. You use the interface by making a method call like data1.compareTo(data2). This will return an int, and the value tells you how data1 and data2 are in relation to each other

If the int is positive, then data1 is larger than data2.

If the int is negative, then data1 is smaller than data2.

If the int is zero, then data1 equals data2.

Note that the returned value can be any integer in Java’s int range, not just -1, 0, 1.

Homework 3: BST Due: See Canvas

Grading

Here is the grading breakdown for the assignment. There are various deductions not listed that are incurred when breaking the rules listed in this PDF and in other various circumstances.

Methods:

constructor

4pts

add

14pts

remove

20pts

get

5pts

contains

5pts

preorder

3pts

inorder

3pts

postorder

3pts

levelorder

3pts

height

3pts

clear

2pts

pruneGreaterThan

10pts

Other:

Checkstyle

10pts

Efficiency

15pts

Total:

100pts

Provided

The following file(s) have been provided to you. There are several, but we’ve noted the ones to edit.

BST.java

This is the class in which you will implement the BST. Feel free to add private helper methods but do not add any new public methods, inner/nested classes, instance variables, or static variables.

BSTNode.java

This class represents a single node in the tree. It encapsulates the data, and the left and right references. Do not alter this file.

BSTStudentTest.java

This is the test class that contains a set of tests covering the basic operations on the BST class. It is not intended to be exhaustive and does not guarantee any type of grade. Write your own tests to ensure you cover all edge cases.

Deliverables

You must submit all of the following file(s) to the course Gradescope. Make sure all file(s) listed below are in each submission, as only the last submission will be graded. Make sure the filename(s) matches the filename(s) below, and thatonly the following file(s) are present. DoNOT submit BSTNode.java for this homework; if you do, your homework will not compile on Gradescope. If you resubmit, be sure only one copy of each file is present in the submission. If there are multiple files, do not zip up the files before submitting; submit them all as separate files.

Homework 3: BST Due: See Canvas

Once submitted, double check that it has uploaded properly on Gradescope. To do this, download your uploaded file(s) to a new folder, copy over the support file(s), recompile, and run. It is your sole responsibility to re-test your submission and discover editing oddities, upload issues, etc.

BST.java

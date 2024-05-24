# Binary Search Tree Sort

This C program implements a binary search tree (BST) to sort and print random numbers in increasing order. It reads integers from standard input, inserts them into the BST, and then prints the sorted numbers.

## Table of Contents
- [Description](#description)
- [Usage](#usage)
- [Functions](#functions)
  - [add_value_to_tree](#add_value_to_tree)
  - [is_right_most_node](#is_right_most_node)
  - [get_right_most_node](#get_right_most_node)
  - [get_left_most_node](#get_left_most_node)
  - [print_tree_increasing_order](#print_tree_increasing_order)
  - [print_in_order](#print_in_order)
- [Compiling and Running](#compiling-and-running)
- [Example](#example)
- [License](#license)

## Description
This program creates a binary search tree (BST) where each node contains an integer value. It reads integers from the standard input, inserts them into the BST, and prints the values in increasing order. The BST ensures that for each node, values in the left subtree are less than the node's value, and values in the right subtree are greater than or equal to the node's value.

## Usage
To use this program, provide a series of integers as input. The program will read these integers, insert them into the BST, and print the sorted sequence.

## Functions

### add_value_to_tree
```c
void add_value_to_tree(NODE ** addr_of_root, int character);
```
Inserts a new value into the BST. It creates a new node with the given value and places it in the correct position in the tree.

### is_right_most_node
```c
int is_right_most_node(NODE * node);
```
Determines if the given node is the rightmost node in the BST. Returns 1 if it is, otherwise returns 0.

### get_right_most_node
```c
NODE * get_right_most_node(NODE * root);
```
Finds and returns the rightmost node (node with the maximum value) in the BST.

### get_left_most_node
```c
NODE * get_left_most_node(NODE * root);
```
Finds and returns the leftmost node (node with the minimum value) in the BST.

### print_tree_increasing_order
```c
void print_tree_increasing_order (NODE * root);
```
Prints the values of the BST nodes in increasing order.

### print_in_order
```c
void print_in_order (NODE * node);
```
Performs an in-order traversal of the BST and prints the values of the nodes.

## Compiling and Running
To compile and run the program, use the following commands:

```sh
# make to compile
make
# execute by typing
./bst_sort
```

You can provide input through standard input, for example by using a file:

```sh
./bst_sort < test.txt
```

## Example
Given the input:
```
1091238 12381 123 13 12415 56765 758 8978 345 3543 5345
```

The program will output:
```
13 123 345 758 3543 5345 8978 12381 12415 56765 1091238
```
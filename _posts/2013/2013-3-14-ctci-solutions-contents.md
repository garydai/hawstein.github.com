---
layout: post
category: Programming
title: Cracking the coding interview--问题与解答
---

## 前言

《Cracking the coding interview》是一本被许多人极力推荐的程序员面试书籍，
详情可见：<http://www.careercup.com/book>。
里面有150道程序员面试题目及相应的解答。书中大部分是编程题目，
并且配有相应的java程序(有些地方有错误或是有更优的方案)。我把书中的题目做了一遍，
并且记录下来，包含自己对问题的一些思路及看法，许多问题给出了两种以上的解答方案。
由于个人平时使用较多的是C++，所以程序是用C++编写，所有的代码都托管在Github上：

<https://github.com/Hawstein/cracking-the-coding-interview>

记录下来的主要目的是加深自己对问题的理解，如果此外还能对一两个人起到帮助作用，
那真真是再好不过了。:P

## 目录

Chapter 1 | Arrays and Strings

1.1
[Implement an algorithm to determine if a string has all unique 
characters. What if you can not use additional data structures?
](/posts/1.1.html)

1.2
[Write code to reverse a C-Style String. (C-String means that “abcd” 
is represented as five characters, including the null character.)
](/posts/1.2.html)

1.3
[Design an algorithm and write code to remove the duplicate characters in a string
without using any additional buffer. NOTE: One or two additional variables are fine.
An extra copy of the array is not.
FOLLOW UP
Write the test cases for this method.
](/posts/1.3.html)

1.4
[Write a method to decide if two strings are anagrams or not.
](/posts/1.4.html)

1.5
[Write a method to replace all spaces in a string with ‘%20’.
](/posts/1.5.html)

1.6
[Given an image represented by an NxN matrix, where each pixel in the image is 4
bytes, write a method to rotate the image by 90 degrees. Can you do this in place?
](/posts/1.6.html)

1.7
[Write an algorithm such that if an element in an MxN matrix is 0, its entire row and
column is set to 0.
](/posts/1.7.html)

1.8
[Assume you have a method isSubstring which checks if one word is a substring of
another. Given two strings, s1 and s2, write code to check if s2 is a rotation of s1 using
only one call to isSubstring (i.e., “waterbottle” is a rotation of “erbottlewat”).
](/posts/1.8.html)

Chapter 2 | Linked Lists

2.1
[Write code to remove duplicates from an unsorted linked list.
FOLLOW UP
How would you solve this problem if a temporary buffer is not allowed?
](/posts/2.1.html)

2.2
[Implement an algorithm to find the nth to last element of a singly linked list.
](/posts/2.2.html)

2.3
[Implement an algorithm to delete a node in the middle of a single linked list, given
only access to that node.
EXAMPLE
Input: the node ‘c’ from the linked list a->b->c->d->e
Result: nothing is returned, but the new linked list looks like a->b->d->e
](/posts/2.3.html)

2.4
[You have two numbers represented by a linked list, where each node contains a single 
digit. The digits are stored in reverse order, such that the 1’s digit is at the head of
the list. Write a function that adds the two numbers and returns the sum as a linked
list.
EXAMPLE
Input: (3 -> 1 -> 5) + (5 -> 9 -> 2)
Output: 8 -> 0 -> 8
](/posts/2.4.html)

2.5
[Given a circular linked list, implement an algorithm which returns node at the beginning of the loop.
DEFINITION
Circular linked list: A (corrupt) linked list in which a node’s next pointer points to an
earlier node, so as to make a loop in the linked list.
EXAMPLE
input: A -> B -> C -> D -> E -> C (the same C as earlier)
output: C
](/posts/2.5.html)

Chapter 3 | Stacks and Queues

3.1
[Describe how you could use a single array to implement three stacks.
](/posts/3.1.html)

3.2
[How would you design a stack which, in addition to push and pop, also has a function
min which returns the minimum element? Push, pop and min should all operate in
O(1) time.
](/posts/3.2.html)

3.3
[Imagine a (literal) stack of plates. If the stack gets too high, it might topple. 
Therefore, in real life, we would likely start a new stack when the previous stack exceeds
some threshold. Implement a data structure SetOfStacks that mimics this. 
SetOfStacks should be composed of several stacks, and should create a new stack once
the previous one exceeds capacity. SetOfStacks.push() and SetOfStacks.pop() should
behave identically to a single stack (that is, pop() should return the same values as it
would if there were just a single stack).
FOLLOW UP
Implement a function popAt(int index) which performs a pop operation on a specific
sub-stack.
](/posts/3.3.html)

3.4
[In the classic problem of the Towers of Hanoi, you have 3 rods and N disks of different
sizes which can slide onto any tower. The puzzle starts with disks sorted in ascending
order of size from top to bottom (e.g., each disk sits on top of an even larger one). You
have the following constraints:	
(A) Only one disk can be moved at a time.
(B) A disk is slid off the top of one rod onto the next rod.
(C) A disk can only be placed on top of a larger disk.
Write a program to move the disks from the first rod to the last using Stacks.
](/posts/3.4.html)

3.5
[Implement a MyQueue class which implements a queue using two stacks.
](/posts/3.5.html)

3.6
[Write a program to sort a stack in ascending order. You should not make any assump-
tions about how the stack is implemented. The following are the only functions that
should be used to write this program: push | pop | peek | isEmpty.
](/posts/3.6.html)

Chapter 4 | Trees and Graphs

4.1
[Implement a function to check if a tree is balanced. For the purposes of this question,
a balanced tree is defined to be a tree such that no two leaf nodes differ in distance
from the root by more than one.
](/posts/4.1.html)

4.2
[Given a directed graph, design an algorithm to find out whether there is a route between two nodes.
](/posts/4.2.html)

4.3
[Given a sorted (increasing order) array, write an algorithm to create a binary tree with
minimal height.
](/posts/4.3.html)

4.4
[Given a binary search tree, design an algorithm which creates a linked list of all the
nodes at each depth (i.e., if you have a tree with depth D, you’ll have D linked lists).
](/posts/4.4.html)

4.5
[Write an algorithm to find the ‘next’ node (i.e., in-order successor) of a given node in
a binary search tree where each node has a link to its parent.
](/posts/4.5.html)

4.6
[Design an algorithm and write code to find the first common ancestor of two nodes
in a binary tree. Avoid storing additional nodes in a data structure. NOTE: This is not
necessarily a binary search tree.
](/posts/4.6.html)

4.7
[You have two very large binary trees: T1, with millions of nodes, and T2, with hun-
dreds of nodes. Create an algorithm to decide if T2 is a subtree of T1.
](/posts/4.7.html)

4.8
[You are given a binary tree in which each node contains a value. Design an algorithm
to print all paths which sum up to that value. Note that it can be any path in the tree
- it does not have to start at the root.
](/posts/4.8.html)

Chapter 5 | Bit Manipulation

5.1
[You are given two 32-bit numbers, N and M, and two bit positions, i and j. Write a
method to set all bits between i and j in N equal to M (e.g., M becomes a substring of
N located at i and starting at j).
EXAMPLE:
Input: N = 10000000000, M = 10101, i = 2, j = 6
Output: N = 10001010100
](/posts/5.1.html)

5.2
[Given a (decimal - e.g. 3.72) number that is passed in as a string, print the binary 
representation. If the number can not be represented accurately in binary, print “ERROR”
](/posts/5.2.html)

5.3
[Given an integer, print the next smallest and next largest number that have the same
number of 1 bits in their binary representation.
](/posts/5.3.html)

5.4
[Explain what the following code does: ((n & (n-1)) == 0).
](/posts/5.4.html)

5.5
[Write a function to determine the number of bits required to convert integer A to
integer B. Input: 31, 14 Output: 2
](/posts/5.5.html)

5.6
[Write a program to swap odd and even bits in an integer with as few instructions as
possible (e.g., bit 0 and bit 1 are swapped, bit 2 and bit 3 are swapped, etc).
](/posts/5.6.html)

5.7
[An array A[1...n] contains all the integers from 0 to n except for one number 
which is missing. In this problem, we cannot access an entire integer in A with 
a single operation. The elements of A are represented in binary, and the only 
operation we can use to access them is “fetch the jth bit of A[i]”, which
takes constant time. 
Write code to find the missing integer. Can you do it in O(n) time?
](/posts/5.7.html)

Chapter 6 | Brain Teasers

[Cracking the coding interview--Q6.1~Q6.6](/posts/brain-teasers.html)

Chapter 7 | Object Oriented Design

XDDDDDD

Chapter 8 | Recursion

8.1
[Write a method to generate the nth Fibonacci number.
](/posts/8.1.html)

8.2
[Imagine a robot sitting on the upper left hand corner of an NxN 
grid. The robot can only move in two directions: right and down. How 
many possible paths are there for the robot?
FOLLOW UP
Imagine certain squares are “off limits”, such that the robot can 
not step on them.
Design an algorithm to get all possible paths for the robot.
](/posts/8.2.html)

8.3
[Write a method that returns all subsets of a set.
](/posts/8.3.html)

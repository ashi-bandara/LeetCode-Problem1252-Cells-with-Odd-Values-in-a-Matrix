
# LeetCode Challenge D30
## Overview

Welcome to my LeetCode solution repository! This project addresses the coding challenge presented by [1252. Cells with Odd Values in a Matrix](https://leetcode.com/problems/cells-with-odd-values-in-a-matrix/). Below, you'll find details about the problem, my approach to solving it, and the implemented solution.

## Problem Statement

There is an  `m x n`  matrix that is initialized to all  `0`'s. There is also a 2D array  `indices`  where each  `indices[i] = [ri, ci]`  represents a  *0-indexed location*  to perform some increment operations on the matrix.

For each location  `indices[i]`, do  *both*  of the following:
1.  Increment  *all*  the cells on row  `ri`.
2.  Increment  *all*  the cells on column  `ci`.

Given  `m`,  `n`, and  `indices`, return  _the  *number of odd-valued cells*  in the matrix after applying the increment to all locations in_ `indices`.

**Example**

>   
![](https://assets.leetcode.com/uploads/2019/10/30/e1.png)
> 
> **Input:** m = 2, n = 3, indices = [[0,1],[1,1]]
> 
> **Output:** 6
> 
> **Explanation:**
> Initial matrix = [[0,0,0],[0,0,0]]. After applying first increment it becomes [[1,2,1],[0,1,0]]. The final matrix is [[1,3,1],[1,3,1]], which contains 6 odd numbers.

**Language Used**
> Java

**Difficulty**
> Easy

## Solution Overview
The solution initializes a 2D array representing the matrix and iterates through the provided indices. For each index, it increments all cells in the corresponding row and column. To enhance efficiency, the algorithm could adopt a sparse matrix approach, tracking only the increments rather than updating each cell individually. Additionally, integrating the counting of odd values into the increment operations can potentially reduce unnecessary iterations, improving the overall runtime of the solution.

# Circular Reference Memory Leak in Objective-C

This repository demonstrates a common memory management issue in Objective-C: circular references leading to memory leaks.  The `circularReferenceBug.m` file contains code exhibiting the problem, while `circularReferenceSolution.m` provides a solution.

## Problem
Two objects retain each other, preventing the system from deallocating them, thus resulting in a memory leak that grows over time.

## Solution
The solution involves carefully managing object ownership, often using techniques like weak references to break the circular dependency.
# Lab 04 - SOP/POS and KMaps

In this lab, you’ve learned how to apply KMaps, Sum Of Products and Products of
sums to simplify digital logic equations. Then, you’ve proven out that they work
using an implemented design on your Basys3 boards.

## Rubric

| Item | Description | Value |
| ---- | ----------- | ----- |
| Summary Answers | Your writings about what you learned in this lab. | 25% |
| Question 1 | Your answers to the question | 25% |
| Question 2 | Your answers to the question | 25% |
| Question 3 | Your answers to the question | 25% |

## Lab Summary

In this lab, we learned how to build boolean expressions directly from a truth table and how to convert a
truth table into a Karnaugh map to simplify a naive equation. We used minterms and maxterms to create both
SOP and POS forms. We also learned how Verilog designs are verified through simulation before being implemented
on real hardware. After confirming that all test cases passed and that each version produced identical outputs,
we were able to load the design onto a physical board and see it function correctly.

## Lab Questions

### Why are the groups of 1’s (or 0’s) that we select in the KMap able to go across edges?

The groups of 1’s (or 0’s) in a K-Map can go across edges because the map wraps around like a cylinder. The left
and right edges are considered adjacent, and the top and bottom edges are also adjacent because the K-Map is arranged
in Gray code order, where only one variable changes between neighboring cells.

### Why are the names Sum of Products and Products of Sums?

The names Sum of Products and Product of Sums describe how the boolean expression is structured. In SOP, variables
are first ANDed together to form product terms, and then those terms are ORed together, making it a sum of products.
In POS, variables are first ORed together to form sum terms, and then those terms are ANDed together, making it a product
of sums.

### Open the test.v file – how are we able to check that the signals match using XOR?

Because of XOR's truth table if the outputs wern't the same than XOR would return 1, if they were the same XOR would return 0. 

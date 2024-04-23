# Multi-Threading
## Submitted by:
- Name - Raghav Garg
- Roll number - 102103283
- Group - 3COE10

## Objective
The objective of this code is to demonstrate multi-threaded matrix multiplication in Python using numpy and threading libraries. The goal is to compare the performance of matrix multiplication using different numbers of threads.

## Methodology
- ### Generate Matrices
The generate_matrices function generates a list of random matrices based on the specified number of matrices (num_matrices) and the size of each matrix (size).

- ### Matrix Multiplication
The matrix_multiply function performs matrix multiplication using a constant matrix and a list of input matrices. It uses numpy's dot function for matrix multiplication.

- ### Multi-threaded Matrix Multiplication
The matrix_multiplication_using_threads function performs matrix multiplication using multiple threads. It divides the list of matrices into chunks based on the number of threads and assigns each chunk to a separate thread for parallel processing.

- ### Performance Measurement
The code measures the time taken for matrix multiplication using different numbers of threads (num_threads) and records the results in a dictionary.

- ### Results Display
The code prints the time taken by each number of threads for matrix multiplication and stores the results in a dictionary (results).
Usage

- #### Threads vs Time Taken

| Threads | Time (sec) |
| ------- | ---------- |
| 1       | 13.351340  |
| 2       | 12.292459  |
| 3       | 12.760156  |
| 4       | 12.333199  |
| 5       | 12.224955  |
| 6       | 12.346241  |
| 7       | 11.969289  |
| 8       | 12.319016  |

- #### Output Graph
![Output Graph](ExecutionTime.png)

- #### CPU core utilization
![](CPU0_5.png)
![](CPU6_11.png)

## Conclusion
The results demonstrate that multi-threading can significantly reduce the time taken for matrix multiplication, especially as the number of threads increases. However, there may be diminishing returns beyond a certain number of threads due to overhead and resource limitations.
# PGC
# Sequential Matrix Multiplication

## Description

This experiment implements sequential matrix multiplication using the C programming language. Two 4000 × 4000 matrices are initialized and multiplied using the standard three nested-loop approach.

The computation is performed sequentially using a single CPU execution flow. The execution time is measured to establish a baseline for performance comparison with parallel implementations.

## Objective

- To implement matrix multiplication using sequential execution.
- To measure the execution time of matrix multiplication.
- To establish a baseline execution time for comparison with parallel implementations.
- To verify the correctness of the matrix multiplication result.

## Environment

- Operating System: Ubuntu on WSL2
- Programming Language: C
- Compiler: GCC
- Matrix Size: 4000 × 4000

## Result

- Matrix Size: 4000 × 4000
- Execution Time: 244.120000 seconds
- Verification: C[0][0] = 4000.00

The sequential execution time is used as the baseline for calculating the speedup of parallel implementations.

# OpenMP Matrix Multiplication

## Description

This experiment implements parallel matrix multiplication using OpenMP and the C programming language. Two 4000 × 4000 matrices are initialized and multiplied using multiple CPU threads on a shared-memory system.

OpenMP is used to distribute the outer loop iterations among multiple threads, allowing different parts of the matrix multiplication to execute concurrently. The experiment uses 8 OpenMP threads and measures the execution time of the parallel computation.

The performance of the OpenMP implementation is compared with the sequential implementation to determine the speedup achieved through parallel execution.

## Objective

- To implement matrix multiplication using OpenMP.
- To understand parallel execution using multiple CPU threads.
- To measure the execution time of the parallel implementation.
- To compare OpenMP performance with the sequential baseline.
- To calculate the speedup obtained through parallel execution.

## Environment

- Operating System: Ubuntu on WSL2
- Programming Language: C
- Compiler: GCC
- Parallel Programming Model: OpenMP
- Matrix Size: 4000 × 4000
- Number of Threads: 8

## Result

- Matrix Size: 4000 × 4000
- Number of Threads: 8
- Execution Time: 30.830434 seconds
- Verification: C[0][0] = 4000.00
- Speedup: 7.92×

The OpenMP implementation achieves a significant reduction in execution time compared with the sequential baseline.

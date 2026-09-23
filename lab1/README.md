## Experiment 1 – Parallel Merge Sort

### Aim

Write an OpenMP program to sort an array of `n` elements using both sequential and parallel merge sort using the `sections` directive. Record and print the difference in execution time between the two methods.

### Description

In this program, an array of `100000` random elements is generated and copied into two arrays. The first array is sorted using **Sequential Merge Sort**, while the second array is sorted using **Parallel Merge Sort**. The parallel version uses the OpenMP `parallel sections` directive to divide the sorting of the two halves between different threads. The execution time of both methods is measured using `omp_get_wtime()`, and the difference between the sequential and parallel execution times is displayed.

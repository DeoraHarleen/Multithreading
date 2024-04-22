# Multithreading using Python
Multiply 100 random matrices of size 1k x 1k with a constant matrix of size 1k x 1k and generate the result table and graph.
# Methodology used in assignment:
## Matrix Multiplication Function: 
The code defines a function matrix_multiply to perform matrix multiplication using NumPy's dot function. This function takes two matrices as input and returns their product.
## Batch Matrix Multiplication Function: 
Another function matrix_multiply_batch is defined to perform matrix multiplication in batches. This function takes a constant matrix A, a batch of matrices matrices_batch, a list results to store the results, and a start_index to indicate where in the results list to store the results of the current batch.
## Threaded Execution Function:
The function run_with_threads orchestrates the threaded execution of matrix multiplication. It divides the list of matrices into chunks based on the number of threads specified. Each thread is assigned a chunk of matrices to multiply concurrently. Once all threads finish their computation, their results are combined.
## Benchmarking: 
The code then benchmarks the performance of matrix multiplication with varying numbers of threads. It initializes a constant matrix A, generates a list of random matrices matrices, and defines a list num_threads indicating the number of threads to use for benchmarking.
## Execution and Measurement: 
For each number of threads specified, the code runs the matrix multiplication with threaded execution and measures the time taken for each execution.
## Result Presentation:
Finally, the code presents the results in tabular and graphical formats.
## Observation
As the number of threads increases, there's an initial reduction in computation time, indicating improved efficiency through parallel processing. However, beyond a certain point, the benefits plateau or even decline due to overhead from thread management and synchronization. This underscores the critical need for judiciously selecting the number of threads based on hardware capabilities and task characteristics to achieve optimal performance.
## Results
![image](https://github.com/DeoraHarleen/Multithreading/assets/100436671/28bfe3aa-7a65-47ed-a6ed-2f0465670a03)
![image](https://github.com/DeoraHarleen/Multithreading/blob/main/cpu1.jpg)


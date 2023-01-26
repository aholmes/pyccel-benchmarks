### Performance Comparison (as of 1.7.1)
## Compilation time
Algorithm                 | python                    | pythran                   | numba                     | pyccel                    | pyccel_c                 
------------------------- | ------------------------- | ------------------------- | ------------------------- | ------------------------- | -------------------------
Ackermann                 | -                         | 2.26                      | 0.34                      | 1.71                      | 1.52                     
Bellman Ford              | -                         | 2.82                      | 0.97                      | 2.40                      | 2.32                     
Dijkstra                  | -                         | 2.86                      | 1.29                      | 2.48                      | 2.35                     
Euler                     | -                         | 3.34                      | 1.30                      | 2.34                      | 2.35                     
Midpoint Explicit         | -                         | 3.88                      | 2.04                      | 2.77                      | 2.67                     
Midpoint Fixed            | -                         | 4.43                      | 2.35                      | 2.79                      | 2.81                     
RK4                       | -                         | 4.82                      | 2.43                      | 3.30                      | 3.26                     
FD - L Convection         | -                         | 2.62                      | 0.33                      | 2.31                      | 2.33                     
FD - NL Convection        | -                         | 2.56                      | 0.32                      | 2.36                      | 2.32                     
FD - Poisson              | -                         | 7.46                      | 0.77                      | 2.40                      | 2.37                     
FD - Laplace              | -                         | 11.00                     | 1.77                      | 3.01                      | -                        
M-D                       | -                         | -                         | 5.33                      | 3.48                      | 3.18                     

## Execution time
Algorithm                 | python                    | pythran                   | numba                     | pyccel                    | pyccel_c                 
------------------------- | ------------------------- | ------------------------- | ------------------------- | ------------------------- | -------------------------
Ackermann (ms)            | 406.00 $\pm$ 2.00         | 7.92 $\pm$ 0.07           | 30.70 $\pm$ 0.30          | 3.28 $\pm$ 0.01           | 3.19 $\pm$ 0.00          
Bellman Ford (ns)         | 59700.00 $\pm$ 1000.00    | 369.00 $\pm$ 5.00         | 530.00 $\pm$ 11.00        | 219.00 $\pm$ 1.00         | 480.00 $\pm$ 6.00        
Dijkstra (ns)             | 29400.00 $\pm$ 200.00     | 316.00 $\pm$ 1.00         | 371.00 $\pm$ 5.00         | 263.00 $\pm$ 3.00         | 459.00 $\pm$ 6.00        
Euler (ms)                | 44.90 $\pm$ 0.70          | 0.69 $\pm$ 0.00           | 1.13 $\pm$ 0.01           | 0.13 $\pm$ 0.00           | 2.95 $\pm$ 0.02          
Midpoint Explicit (ms)    | 92.30 $\pm$ 1.40          | 1.53 $\pm$ 0.00           | 2.89 $\pm$ 0.04           | 0.23 $\pm$ 0.01           | 5.28 $\pm$ 0.02          
Midpoint Fixed (ms)       | 450.00 $\pm$ 4.00         | 9.34 $\pm$ 0.12           | 15.90 $\pm$ 0.10          | 0.95 $\pm$ 0.04           | 23.50 $\pm$ 0.20         
RK4 (ms)                  | 228.00 $\pm$ 3.00         | 1.91 $\pm$ 0.00           | 5.76 $\pm$ 0.10           | 0.27 $\pm$ 0.01           | 6.34 $\pm$ 0.05          
FD - L Convection (ms)    | 2160.00 $\pm$ 40.00       | 1.65 $\pm$ 0.10           | 9.38 $\pm$ 0.07           | 1.68 $\pm$ 0.04           | 1.61 $\pm$ 0.09          
FD - NL Convection (ms)   | 2700.00 $\pm$ 30.00       | 1.90 $\pm$ 0.02           | 9.22 $\pm$ 0.04           | 1.72 $\pm$ 0.05           | 1.78 $\pm$ 0.07          
FD - Poisson (ms)         | 4260.00 $\pm$ 40.00       | 2.03 $\pm$ 0.00           | 10.50 $\pm$ 0.10          | 3.88 $\pm$ 0.00           | 1.75 $\pm$ 0.00          
FD - Laplace (\textmu s)  | 53.00 $\pm$ 0.70          | 2.46 $\pm$ 0.04           | 8.72 $\pm$ 0.08           | 1.96 $\pm$ 0.05           | -                        
M-D (ms)                  | 46200.00 $\pm$ 1000.00    | -                         | 223.00 $\pm$ 2.00         | 269.00 $\pm$ 0.00         | 274.00 $\pm$ 0.00        
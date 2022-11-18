### Performance Comparison (as of 1.6.1)
## Compilation time
Algorithm                 | python                    | pythran                   | numba                     | pyccel                    | pyccel_c                 
------------------------- | ------------------------- | ------------------------- | ------------------------- | ------------------------- | -------------------------
Ackermann                 | -                         | 2.42                      | 0.33                      | 1.24                      | 1.13                     
Bellman Ford              | -                         | 2.75                      | 0.95                      | 1.78                      | 1.70                     
Dijkstra                  | -                         | 2.76                      | 1.25                      | 1.89                      | -                        
Euler                     | -                         | 3.29                      | 1.30                      | 1.83                      | 1.73                     
Midpoint Explicit         | -                         | 4.14                      | 2.01                      | 2.17                      | 2.08                     
Midpoint Fixed            | -                         | 4.96                      | 2.31                      | 2.22                      | 2.16                     
RK4                       | -                         | 4.95                      | 2.36                      | 2.57                      | -                        
FD - L Convection         | -                         | 2.39                      | 0.32                      | 1.68                      | 1.67                     
FD - NL Convection        | -                         | 2.39                      | 0.31                      | 1.68                      | 1.69                     
FD - Poisson              | -                         | 7.81                      | 0.74                      | 1.80                      | 1.75                     
FD - Laplace              | -                         | 12.86                     | 1.71                      | 2.26                      | -                        
M-D                       | -                         | -                         | 5.27                      | -                         | -                        

## Execution time
Algorithm                 | python                    | pythran                   | numba                     | pyccel                    | pyccel_c                 
------------------------- | ------------------------- | ------------------------- | ------------------------- | ------------------------- | -------------------------
Ackermann (ms)            | 472.00 $\pm$ 3.00         | 22.00 $\pm$ 0.20          | 32.40 $\pm$ 0.30          | 13.20 $\pm$ 0.00          | 14.30 $\pm$ 0.00         
Bellman Ford (ns)         | 58900.00 $\pm$ 700.00     | 367.00 $\pm$ 5.00         | 541.00 $\pm$ 4.00         | 232.00 $\pm$ 4.00         | 472.00 $\pm$ 4.00        
Dijkstra (ns)             | 30000.00 $\pm$ 100.00     | 356.00 $\pm$ 5.00         | 356.00 $\pm$ 4.00         | 245.00 $\pm$ 3.00         | -                        
Euler (ms)                | 48.40 $\pm$ 0.80          | 0.49 $\pm$ 0.01           | 1.27 $\pm$ 0.01           | 0.14 $\pm$ 0.01           | 2.70 $\pm$ 0.03          
Midpoint Explicit (ms)    | 98.80 $\pm$ 1.50          | 1.18 $\pm$ 0.02           | 3.13 $\pm$ 0.05           | 0.18 $\pm$ 0.00           | 4.85 $\pm$ 0.02          
Midpoint Fixed (ms)       | 501.00 $\pm$ 10.00        | 7.28 $\pm$ 0.06           | 17.50 $\pm$ 0.20          | 0.61 $\pm$ 0.03           | 21.50 $\pm$ 0.60         
RK4 (ms)                  | 253.00 $\pm$ 7.00         | 1.89 $\pm$ 0.02           | 6.37 $\pm$ 0.09           | 0.65 $\pm$ 0.03           | -                        
FD - L Convection (ms)    | 2210.00 $\pm$ 10.00       | 1.89 $\pm$ 0.00           | 9.13 $\pm$ 0.13           | 1.75 $\pm$ 0.04           | 1.69 $\pm$ 0.16          
FD - NL Convection (ms)   | 2780.00 $\pm$ 20.00       | 2.00 $\pm$ 0.04           | 9.44 $\pm$ 0.24           | 1.79 $\pm$ 0.01           | 1.94 $\pm$ 0.00          
FD - Poisson (ms)         | 4490.00 $\pm$ 90.00       | 2.29 $\pm$ 0.01           | 11.00 $\pm$ 0.10          | 3.87 $\pm$ 0.00           | 2.01 $\pm$ 0.01          
FD - Laplace (\textmu s)  | 54.80 $\pm$ 0.70          | 2.42 $\pm$ 0.06           | 8.93 $\pm$ 0.09           | 2.19 $\pm$ 0.01           | -                        
M-D (s)                   | 53.00 $\pm$ 1.90          | -                         | 0.23 $\pm$ 0.00           | -                         | -                        
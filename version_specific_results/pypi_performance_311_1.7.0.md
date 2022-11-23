### Performance Comparison (as of 1.7.0)
## Compilation time
Algorithm                 | python                    | pythran                   | pyccel                    | pyccel_c                 
------------------------- | ------------------------- | ------------------------- | ------------------------- | -------------------------
Ackermann                 | -                         | 3.12                      | 1.66                      | 1.50                     
Bellman Ford              | -                         | 3.50                      | 2.26                      | 2.14                     
Dijkstra                  | -                         | 3.51                      | 2.38                      | 2.24                     
Euler                     | -                         | 4.16                      | 2.30                      | 2.24                     
Midpoint Explicit         | -                         | 5.15                      | 2.65                      | 2.59                     
Midpoint Fixed            | -                         | 6.07                      | 2.74                      | 2.70                     
RK4                       | -                         | 5.93                      | 3.24                      | 3.19                     
FD - L Convection         | -                         | 3.18                      | 2.13                      | 2.12                     
FD - NL Convection        | -                         | 3.19                      | 2.17                      | 2.23                     
FD - Poisson              | -                         | 9.88                      | 2.30                      | 2.23                     
FD - Laplace              | -                         | 16.29                     | 3.09                      | -                        
M-D                       | -                         | -                         | 3.49                      | 3.17                     

## Execution time
Algorithm                 | python                    | pythran                   | pyccel                    | pyccel_c                 
------------------------- | ------------------------- | ------------------------- | ------------------------- | -------------------------
Ackermann (ms)            | 500.00 $\pm$ 5.00         | 13.50 $\pm$ 0.20          | 4.02 $\pm$ 0.04           | 3.34 $\pm$ 0.08          
Bellman Ford (ns)         | 70500.00 $\pm$ 2200.00    | 449.00 $\pm$ 31.00        | 277.00 $\pm$ 4.00         | 582.00 $\pm$ 14.00       
Dijkstra (ns)             | 32800.00 $\pm$ 300.00     | 415.00 $\pm$ 4.00         | 342.00 $\pm$ 1.00         | 560.00 $\pm$ 5.00        
Euler (\textmu s)         | 56400.00 $\pm$ 1700.00    | 666.00 $\pm$ 4.00         | 166.00 $\pm$ 9.00         | 3590.00 $\pm$ 50.00      
Midpoint Explicit (ms)    | 112.00 $\pm$ 2.00         | 1.52 $\pm$ 0.02           | 0.20 $\pm$ 0.00           | 6.39 $\pm$ 0.09          
Midpoint Fixed (ms)       | 534.00 $\pm$ 9.00         | 9.47 $\pm$ 0.07           | 0.82 $\pm$ 0.03           | 28.70 $\pm$ 0.60         
RK4 (ms)                  | 272.00 $\pm$ 5.00         | 2.17 $\pm$ 0.02           | 0.30 $\pm$ 0.01           | 7.74 $\pm$ 0.14          
FD - L Convection (ms)    | 2410.00 $\pm$ 40.00       | 2.00 $\pm$ 0.02           | 1.89 $\pm$ 0.04           | 1.89 $\pm$ 0.03          
FD - NL Convection (ms)   | 3100.00 $\pm$ 40.00       | 2.26 $\pm$ 0.02           | 1.83 $\pm$ 0.04           | 1.98 $\pm$ 0.03          
FD - Poisson (ms)         | 5080.00 $\pm$ 50.00       | 2.45 $\pm$ 0.01           | 4.68 $\pm$ 0.05           | 2.12 $\pm$ 0.01          
FD - Laplace (\textmu s)  | 63.70 $\pm$ 0.80          | 2.82 $\pm$ 0.03           | 2.55 $\pm$ 0.15           | -                        
M-D (ms)                  | 54400.00 $\pm$ 600.00     | -                         | 209.00 $\pm$ 1.00         | 216.00 $\pm$ 1.00        
# LMTR
LMTR suite for unconstrained optimization. This package contains limited memory trust-region and line-search algorithms implemented in MATLAB. This package contains limited memory trust-region and line-search algorithms implemented in MATLAB. 
The algorithms are described in "On Efficiently Combining Limited Memory and Trust-Region Techniques", Mathematical Programming Computation (2017) Vol. 9, no 1, pp. 101-134, [https://doi.org/10.1007/s12532-016-0109-7](https://doi.org/10.1007/s12532-016-0109-7).

## ALGORITHMS
For more information on each algorithm, type "help ALGORITHMNAME.m"
- LMTR_EIG_inf_2.m - limited memory trust-region algorithm EIG(&infin;; 2) based on
the eigenvalue-based norm &Vert;x&Vert;<sub>&infin;,2</sub>, with the exact solution to the TR subproblem in closed form;
- LMTR_EIG_MS_2_2.m - limited memory trust-region algorithm EIG-MS(2,2) based
on the eigenvalue-based norm &Vert;x&Vert;<sub>2,2</sub>, with the Moré-Sorenson approach for solving a low-dimensional TR subproblem;
- LMTR_EIG_MS.m - limited memory trust-region algorithm EIG-MS, applies the
Moré-Sorenson approach for solving the TR subproblem de ned in the Euclidean
norm using the eigenvalue decomposition of the Hessian approximation;
- LMTR_BWX_MS.m - limited memory trust-region algorithm BWX-MS, applies the
Moré-Sorenson approach for solving the TR subproblem de ned in the Euclidean
norm. It is a modified version of the algorithm by Burke et al;
- LMTR_DDOGL.m - limited memory trust-region algorithm DDOGL, applies the
double dogleg approach for solving the TR subproblem de ned in the Euclidean
norm.
- LBFGS_MT.m - limited memory line-search algorithm based on the Moré-Thuente
line search;
- LBFGS_MTBT.m - limited memory line-search algorithm based on the Moré-Thuente
line search, takes initial step using backtrack;
- LBFGS_TR.m - limited memory line-search algorithm, takes a trial step along the
quasi-Newton direction inside the trust region.

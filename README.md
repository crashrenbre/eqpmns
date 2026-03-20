# Equality tests in the Polynomial Modular Number System

This folder contains the code used to measure cycle counts in the relevant tables in the "Equality tests in the Polynomial Modular Number System" paper. You will need GCC and GnuMP to compile the codes. For the performances to be accurate on intel processors the Turbo Boost® needs to be disabled. For linux we provide the script "disableturboboost.sh" to disable the turbo boost. To run it:
> chmod +x disableturboboost.sh && sudo ./disableturboboost.sh

## Benchmarks
To perform the benchmarks for all four algorithms for the inequality case:
> make inequalitybench

Similarly, to run the benchmark in the equality case:
> make equalitybench

## Code generation
We also provide a code generation script to generate a header file for any PMNS. This is done through the codegen.py file. Simply edit the line which sets the parameters (p,n,gamma,lam,rho,M) as needed. Support for values of phi different from 2^64 is not done yet. The code generation needs the SageMath library to be installed in order to be run. This can be obtained from the address http://www.sagemath.org/

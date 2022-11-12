# Complexity

[TOC]

## Polynomial / Exponential Time

The complexity class of all problems that can be solved in **polynomial** time on a **deterministic** RAM.

In the case of **deterministic RAM**, the algorithm can take **polynomial** (P) or **exponential**  (EXPTIME) time to find solution.



## Non Determinism In Algorithm

**Non determinstic algorithm** is an algorithm that, even for **same input**, can provide **different outputs on different runs**.

In the case of **non-deterministic RAM**, the algorithm can take **polynomial** (NP) or **exponential** (NEXPTIME).

## NP Problems

The complexity class of all problems that can be solved in **polynomial** time on a **non-deterministic** RAM.

* NP-Complete
* NP-Hard



## How to Solve NP-Complete or NP-Hard Problems?

We may not be able to find the **optimal** solution. But the objective is to find out the **near-optimal** solution.

Typically, the hard problems take **exponential** time (for ex: $$2^n$$, n being input size), which is not acceptable. By different techniques, if we can change  the *base* of the exponent for the run time, may yield better results (for ex: $$1.7^n$$).

For the **harder** problems, the size of input (*n*) is not the only the problem. The structure of the *input* (*k*) matters as well. 

Following are some of approaches to solving NP-Complete or NP-Hard problems.

- With Performace Guarantee

  1. **Optimized Search Trees and pre-processing.**

     Avoid the exhaustive search space by optimizing the tree. 

     The **pre-processing** here is to trim the input (aka clean the input space), that would result in reduced search space. Also, note that the *pre-processing* should be in *polynomial* time and that should not affect the *solution*.

  2. **Approximation Algorithms**

     They provide a mathematical proof certfying the quality of the returned solution in worst case.

     The objective is to find the **near-optimal** solution.

     - Constant Factor Approximation

     - Polynomial Time Approximation Scheme (PTAS)

  3. **Randomized Algorithms**

     Uses **random** number in the algorithm. It employs some degree of *randomness* as part of its logic or procedure. It usually uses *pseudo random number generator*, which is a **deterministic** 

      * Las Vegas algorithm

      * Monte Carlo algorithm

        

- No Performace Guarantees.

  - Heuristics Algorithm : They resonably find good solution on some inputs but provide no clear indication at the outset why they succeed or fail.
    - Genetic Algorithm
    - Simulated Annealing
    - Local Search
  - Metaheuristic

## Resources


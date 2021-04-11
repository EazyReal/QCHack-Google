# QC Hack 2021 (Google Quantum AI Challenge)
> [name=Maxwill Lin] [time=2021, April 11] 

![](https://i.imgur.com/YlvmR8x.png)

## Problem
- https://github.com/quantumlib/qchack-2021-challenge
- Maybe the restriction of ability to be run on `google.Sycamore` may be reach with 
    - implementing CNOT gate with the gate set given 
    - use consecutive SWAP/CNOTs to link disjoint paths on the grid

## Resources
SOTA results
- https://arxiv.org/pdf/quant-ph/0404089.pdf
    - Quantum circuits for general multi-qubit gates, 2004
    - $4^n-2^{n+1}$ CNOTs
    - and the first proposal of $F_m^k$ implementation
- https://arxiv.org/pdf/2101.02993.pdf
    - Efficient decomposition of unitary matrices in quantum circuit compilers
    - QSD, 2021
    - $\frac 3 4 \cdot4^n-2^{n+1}$ CNOTs
    - Optimal In some sense
- https://www.nature.com/articles/s41598-018-23764-x
    - Efficient Contolled Rn with one ancillary
- https://arxiv.org/pdf/quant-ph/0406176.pdf
    - Synthesis of Quantum Logic Circuits (2006)
        - propsal of QSD
- https://www.researchgate.net/publication/2189906_Smaller_Circuits_for_Arbitrary_n-qubit_Diagonal_Computations
    - complicated, technical part for decomposing diagonal

## Resources (Not SOTA)
Outdated
- https://core.ac.uk/download/pdf/193939351.pdf
    - survey paper @2006
    - CSD
- https://arxiv.org/pdf/quant-ph/9902062.pdf
    - A Rudimentary Quantum Compiler (2cnd Ed.)
    - CSD original, 199x
- https://arxiv.org/pdf/1210.7366.pdf
    - Decomposition of unitary matrices and quantum gates, 2013
    - good explanations
- https://arxiv.org/pdf/quant-ph/0312218.pdf
    - Efficient decomposition of quantum gates, 2004
    - $11\cdot4^n$
- https://arxiv.org/pdf/1904.01072.pdf
    - a compiler paper
- https://arxiv.org/pdf/1501.06911.pdf
    - Quantum Circuits for Isometries, detailed 2016


## Repos for Other compiler
- https://github.com/Q-Compiler/UniversalQCompiler
- https://github.com/openql-org
- https://github.com/prince-ph0en1x/QSD/blob/master/QSD_matlab/QSD_Main.m
- https://github.com/QE-Lab/OpenQL/tree/develop/src
- https://github.com/qosf/awesome-quantum-software#quantum-compilers

## Cirq Functions that May be Useful
- https://quantumai.google/reference/python/cirq/optimizers/decompose_multi_controlled_rotation

---

## Some Situations
- My teams chose to leave during the QC hack.
- I continue to study the research papers, but cannot implement the alone in time :(.
- Some results are in `./try.ipynb`
    - I tried to implement Quantum Shannon Decomposition

## Final Strategy
- Try to pass trivial testcases :(
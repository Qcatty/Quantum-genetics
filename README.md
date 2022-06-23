# Quantum-genetics

## Team Name:
QSchrodinger

Project Description:
genetic quantum algorithm (GQA). GQA is based on the concept and principles of quantum computing such as qubits and superposition of states. Instead of binary, numeric, or symbolic representation, by adopting qubit chromosome as a representation GQA can represent a linear superposition of solutions due to its probabilistic representation. As genetic operators, quantum gates are employed for the search of the best solution. Rapid convergence and good global search capability characterize the performance of GQA. The effectiveness and the applicability of GQA are demonstrated by experimental results on the knapsack problem, The results show that GQA is superior to other genetic algorithms using penalty functions, repair methods, and decoders.
a quantum genetic algorithm consist on:
1- First step, the algorithm begins preparing a superposition of all individuals, i.e., N, or chromosomes of population Q(t), Therefore, all individuals are represented by only one individual quantum register. That is, the entire population is represented by a single chromosome in a superposition state, One of the key steps of RQGA is the correlation between the individual quantum register |x>i and a fitness quantum register | f itness>i.
2- In a second step the algorithm searches for the maximum fitness. Once the operator F is applied, RQGA searches for the maximum fitness value based on the Grover’s search algorithm.
3- Finally, making a measure in the chromosome with maximum fitness is obtained.
Reference material:

[1] https://www.mdpi.com/2073-431X/5/4/24/pdf
[2] https://arxiv.org/pdf/cs/0403003.pdf
[3] https://www.researchgate.net/publication/2573070_Genetic_Quantum_Algorithm_and_its_Application_to_Combinatorial_Optimization_Problem
[4] https://iopscience.iop.org/article/10.1088/1742-6596/1719/1/012102/pdf

## Source code:
https://github.com/echchallaouy/Quantum-genetics

## Resource Estimate:
A 1-2 paragraph written Resource Estimate, indicating how you expect to use the IBM 16-qubit QPU, if awarded, to finish your Open Hackathon project.

We are going to use the IBM 16-qubit QPU, if awarded to simulate a large number of the population's chromosomes.
### 1- In the first place, Genes are the qubits.
### 2- Second, preparing the superposition of all individuals, or chromosomes of the population.
### 3- In third place, the oracle O marks the maximum fitness of |ψ>i, such that when the oracle is applied we obtain the superposition, this step is repeated a given number of iterations. The Grover’s maximum number of iterations is calculated as pi *sqrt(2**n)/4 where n is the number of qubits or length of the quantum chromosome.
### 4- In fourth and last place the Grover’s diffusion operator G finds the chromosome with a marked state.
### 5- Finally, making a measure, we get the state that points to chromosome with maximum fitness

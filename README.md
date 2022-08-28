## TASK

Implement a genetic algorithm for determining the maximum of a positive function over a domain
given (function will be fixed in code)
## Input:

- population size
- the scope of the function
- parameters for the function to be maximized (coefficients of the degree 2 polynomial)
- the precision with which one works (with which the interval is discretized)
- the probability of recombination (crossover)
- the probability of mutation
- the number of stages of the algorithm

## Output:
- A suggestive file highlighting the operations of the **first stage** of the algorithm, (de
example of the file Evolution.txt (obtained for the function –x^2 +x+2, domain [-1, 2],
population size 20, precision 6, probability of recombination 0.25, probability of
mutation 0.01 and 50 stages))

## FORMATATION
 - the initial population in the form
i: chromosome representation x = the value corresponding to the chromosome in the definition domain
of the function f = the value corresponding to the chromosome (f(X​i​))
  - selection probabilities for each chromosome
  - the cumulative probabilities that give the ranges for selection
  - highlighting the selection process, which consists in generating a uniform random number u on
[0,1) and determining the interval [q​i​, q​i+1​) to belong to this number; value of this
interval, chromosome i+1 will be selected. The process is repeated until the desired number of is selected
chromosomes. **Requirement:** the search of the interval set to u will be binary
searched.
  - highlighting the chromosomes that participate in recombination
  - for recombinations that take place, the pairs participating in the recombination are highlighted,
the randomly generated breakpoint as well as the chromosomes resulting from recombination (or,
if applicable, the type of crossing chosen is highlighted)
  - the resulting population after recombination
  - the resulting population after mutations
  - for the rest of the generations (populations from the next stages) only the value will be displayed
maximum and average performance value.

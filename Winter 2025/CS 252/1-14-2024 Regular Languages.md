Computational Model
- Mathematical object (defined on paper) that enables us to reason about computation and to study properties and limitations of computation
**Finite Automata** is the simplest model
- Good model for computers with an extremely limited amount of memory 
- Useful tools when attempting to recognize patterns
# Snack Machine Example
### Assumptions
- Every item costs 75 cents
- This machine takes
	- Quarters (q)
	- Fifty Cent coins (f)
	- One dollar coins (d)

- After 75 cents are deposited, the user can push the button "item" (b) and the machines resets
- Machine does not give back change


The state of the machine is the amount of change deposited, since the last time the machine reset

Total Function: Every element in the domain can be mapped to an image in the range
Partial Function:  Only some elements in the domain can be mapped to an image in the range

Finite Automaton 
- Is a model for computers with an extremely **limited amount of memory**
- Good for emulating **simple/few** instructions
- useful to recognize **patterns**

A 5 tuple ($Q,\sum,\delta, q_{0},F$) where
- $Q$ is a finite set called the **states**
- $\sum$ is a finite set called the **alphabet**
- $\delta: Q\times \sum \rightarrow Q$ is the **transition function** ($q_{i}, a$) $\rightarrow q_{j}$
- $q_{0}\in Q$ is the **start state**
- $F \subset Q$ is the set of **accept states**


Q = {0, 0.25, 0.50, 0.75}
$\sum$ = {q, f, d, b}
$\delta$  = 
$q_{0}$ = 0
$F$ = {0.75} 

# The Language of a FA
$x \in L(M)$ then M accepts x or x is a member of the language recognized by $M$ 

If $A$ is the set of all strings a machine $M$ accepts, the $A$ is the **language** of the machine 
- $L(M) = A$ 

A machine may accept several strings, but recognizes only one language
If the machine accepts no strings, it still recognizes one language 
- empty language
# Complementing Languages
- By swapping final states and non-final states of $M_{1}$,  we get a new finite automaton $M_{2}$, such that $L(M_{2}) = \complement{L(M_{1})}$ 


5 10 15 20 25 30 35



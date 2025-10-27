#Sets #SetOperations #CartesianProducts #SetBuilderNotation




|       Term       | Definition                                                                          |
| :--------------: | ----------------------------------------------------------------------------------- |
|      $\in$       | is an element of                                                                    |
|     $\notin$     | is not an element of                                                                |
|        \|        | such that                                                                           |
|   $\subseteq$    | is a subset of                                                                      |
|   $\supseteq$    | is a superset of                                                                    |
|   Cardinality    | The size of finite set                                                              |
|      \|A\|       | the cardinality of a finite set                                                     |
| $\emptyset$, {}  | empty set; \|$\emptyset$\| = 0                                                      |
|  {$\emptyset$}   | A set with only one element                                                         |
| $\wp (S)$, $2^S$ | Power set; the set of all subsets of set $S$                                        |
|     $\land$      | and                                                                                 |
|      $\lor$      | or                                                                                  |
|    $\forall$     | for all                                                                             |
|    $\implies$    | implies                                                                             |
|    $\exists$     | there exists                                                                        |
|     $\times$     | Cartesian Product; The set of all ordered pairs of two sets                         |
|      $\cup$      | Union; The set of all unique elements in two sets                                   |
|  $\setminus$, -  | Difference; The set of unique elements that is present in one set but not the other |
|    $\bar{A}$     | The complement of $A$ with respects to $U$                                          |


> [!Info]+ Set
> An unordered collection of distinct objects (elements)

$a \in A$ means that a is an element of set A
$a \notin A$ means that a is not an element of set A


> [!faq] Example 1
> $V = \{a, e, i, o, u\}$ 
> set V is the set of all vowels
> Listing all the elements in a set is called the **roster method**

> [!faq] Example 2
> Give the set of all positive integers less than 10
> $O = \{1,3,5,7,9\}$

> [!faq] Example  3
> $\{a, 2, Fred\}$
> Elements in a set don't necessarily need to be related to eachother

# Set Builder Notation


> [!info]+ Set Builder Notation
> $\left\{x\mid P\left(x\right) \right\}$ = the set of all x such that x has the property of P
> 
> | can be read as "such that"


> [!faq] Example 1
> $O = \{\:x\:|\:$ x is an odd positive integer less than 10 $\}$
> $O = \{1,3,5,7,9\}$

$\mathbb{N} = \{0,1,2,3,\dots\}$ the set all natural numbers
$\mathbb{Z} = \{\dots,-2,-1,0,1,2,\dots\}$ the set of all integers
$\mathbb{Z^{+}} = \{1, 2, 3,\dots\}$ the set of all positive integers
$\mathbb{Q} = \{\frac{p}{q}\mid \ p \in \mathbb{Z} \text{ and } q \in \mathbb{Z} \}$  
$\mathbb{R} =$ the set of all real numbers
$\mathbb{R^{+}} =$ the set of all positive real numbers 
# Empty Sets
Null Set $= \emptyset , \{\}$ 
$\{\emptyset\} =$ a singleton set where it only has 1 element
# Subsets
A is a subset of B if every element of A is in B 
$$
A \subseteq B
$$
B is a superset of A if A is a subset of B
$$
B \supseteq A
$$
Therefore
$$
A \subseteq B = B \supseteq A
$$

> [!faq] Example
> set of all odd positive integers less than 10 is a subset of all positive integers less than 10

# Size of a Set

> [!info]+ Finite Set
> Suppose we have set S
> If there are exactly n distinct elements where $n \geq 0$, then S is a finite set
> The Cardinality of S is denoted as $|S|=n$

> [!faq] Example
> Let A be the set of odd positive integers less then 10. What is the cardinality of A?
> $A=\{1,3,5,7,9\}$
> $|A|=5$

> [!faq] Example
> Let S be the set of all letters in the English alphabet. What is the cardinality of S?
> $|S|=26$

> [!faq] Example
> What is the cardinality of a null set?
> $|\emptyset|=0$ 

> [!info] Infinite Set
> If a set is not finite, it is considered infinite

> [!faq] Example
> The set of all positive integers is infinite
# Power Sets

> [!info]+ Power Set
> The Power Set of S is the set of all subsets of the set S
> $\wp(S)$ or $2^S$

if a set has n elements, its power set will have $2^n$ elements
# Cartesian Products

> [!info]+ Ordered n-tuples
> $\{a_1,a_2,a_3\dots,a_n\}$ is an ordered collection where $a_1$ is the first element, $a_2$ is the second element, and $a_n$ is the nth element
>
> $\{a_1,a_2,\dots,a_{n\}}=\{b_1,b_2,\dots,b_n\}$ 
> if $a_i=b_i$  
> where  $i=1,2,\dots,n$

> [!info]+ Cartesian Product
> $A\times B$ is the set of all ordered pairs
> 
> $(a,b)$ 
> where $a \in A$ and $b \in B$
>
$$
A \times B = \{(a,b) \mid {a \in A} \land {b\in B}\}
$$
# Set Operations

> [!info]+ Union of Sets
> The Union of a set is the set of all elements in set A and set B
$$
A \cup B = \{x\mid x\in A \lor x\in B\}
$$

> [!info]+ Intersection of Sets
> The Intersection of set A and B is the difference of A and B.
$$
A - B = \{x \mid x \in A \land x \notin B\} 
$$

$A - B$ is also called the complement of B with respect to A


> [!info]+ Complements of Sets
> Let U be the universal set. The complement of set A is $\bar{A}$
> $\bar{A}$ is the complement of A with respect to U
$$
\bar{A} = U - A = \{x \in U \mid x \notin A\}
$$


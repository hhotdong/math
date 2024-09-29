## Definitions

<details><summary>Proposition</summary>
  
  - A sentence or statement which has a definite truth value.[^truth_value_def]
  
  - ex. 1 = 2 (false), 1 = 1(true)
    
</details>

<details><summary>Formula</summary>

  - A statement which possibliy involves some variables, which is either true or false whenever we assign particular values to each of the variables.
    
  - ex. Given a formula $`x^2 + y = 5`$, which is true when (x, y) = (1, 4), (2, 1)⋯, but false when (2, 2), (4, 1)⋯.

</details>

<details><summary>Negation</summary>

  - If P is a formula, then “not P” is another formula, which we write symbolically as ¬P.

| P   | $\neg$ P |
| :-: | :-:      |
| T   | F        |
| F   | T        |

</details>

<details><summary>Conjunction</summary>
  
  - Suppose that P and Q are formulas. Then “P and Q” is a formula written symbolically as P $\land$ Q, called the conjunction of P and Q.
    </br>For P $\land$ Q to be true both P and Q must be true, otherwise it is false.
  
  - $\land$, 'and', '곱연산'

| P   | Q   | P $\land$ Q  |
| :-: | :-: | :-:          |
| T   | T   | T            |
| T   | F   | F            |
| F   | T   | F            |
| F   | F   | F            |

</details>

<details><summary>Disjunction</summary>

  - Given two formulas P and Q, disjunction is a operation which makes new formula whose truth value is false only when both P, Q are false.

  - $\lor$, 'or', '합연산'

| P   | Q   | P $\lor$ Q |
| :-: | :-: | :-:        |
| T   | T   | T          |
| T   | F   | T          |
| F   | T   | T          |
| F   | F   | F          |

</details>

<details><summary>Condition</summary>

  - If P and Q are formulas, then “if P then Q” or “P implies Q” is written P $\Rightarrow$ Q, using the conditional symbol, $\Rightarrow$.

| P   | Q   | P $\Rightarrow$ Q |
| :-: | :-: | :-:               |
| T   | T   | T                 |
| T   | F   | F                 |
| F   | T   | T                 |
| F   | F   | T                 |

</details>

<details><summary>Bicondition</summary>

  - Given two propositions P and Q. If P implies Q and Q implies P, written $\Leftrightarrow$, corresponds to the phrase “if and only if” or “iff” for short. So P $\Leftrightarrow$ Q is true when both P and Q have the same truth value, otherwise it is false.

| P   | Q   | P $\Leftrightarrow$ Q |
| :-: | :-: | :-:                   |
| T   | T   | T                     |
| T   | F   | F                     |
| F   | T   | F                     |
| F   | F   | T                     |

</details>

<details><summary>Tautology</summary>

- A logical expression that always evaluates to T, that is, the last column of its truth table consists of nothing but T’s.

- ex. (P $\land$ Q) $\lor$ P $\Leftrightarrow$ P is tautology.

| P   | Q   | P $\land$ Q | (P $\land$ Q) $\lor$ P | (P $\land$ Q) $\lor$ P $\Leftrightarrow$ P |
| :-: | :-: | :-:         | :-:                    | :-:                                        |
| T   | T   | T           | T                      | T                                          |
| T   | F   | F           | T                      | T                                          |
| F   | T   | F           | F                      | T                                          |
| F   | F   | F           | F                      | T                                          |

</details>

### Reference

- [수학의 즐거움](https://www.youtube.com/@enjoyingmath9346/featured)
- Patrick Keef, David Guichard, \<An Introduction to Higher Mathematics\>

[^truth_value_def]: In logic and mathematics, a truth value, sometimes called a logical value, is a value indicating the relation of a proposition to truth, which in classical logic has only two possible values (true or false). - [Wikipedia](https://en.wikipedia.org/wiki/Truth_value)

## Definitions

<details><summary>Proposition</summary>
  
  - A sentence or statement which has a definite truth value.[^truth_value_def]
  
  - ex. 1 = 2 (false), 1 = 1(true)
    
</details>

<details><summary>Formula</summary>

  - A statement which possibliy involves some variables, which is either true or false whenever we assign particular values to each of the variables.
    
    - ex. Given a formula $`x^2 + y = 5`$, which is true when (x, y) = (1, 4), (2, 1)⋯, but false when (2, 2), (4, 1)⋯.
   
  - A formula that contains variables is not simply true or false unless each of these variables is bound by a quantifier. If a variable is not bound the truth of the formula is contingent on the value assigned to the variable from the universe of discourse.

</details>

<details><summary>Negation</summary>

  - If P is a formula, then “not P” is another formula, which we write symbolically as $\neg$ P.

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

  - Given two formulas P and Q, disjunction is an operation which constructs new formula whose truth value is false only when both P and Q are false.

  - $\lor$, 'or', '합연산'

| P   | Q   | P $\lor$ Q |
| :-: | :-: | :-:        |
| T   | T   | T          |
| T   | F   | T          |
| F   | T   | T          |
| F   | F   | F          |

</details>

<details><summary>Conditional</summary>

  - If P and Q are formulas, then “if P, then Q” or “P implies Q” is written P $\Rightarrow$ Q, using the conditional symbol, $\Rightarrow$.

| P   | Q   | P $\Rightarrow$ Q |
| :-: | :-: | :-:               |
| T   | T   | T                 |
| T   | F   | F                 |
| F   | T   | T                 |
| F   | F   | T                 |

</details>

<details><summary>Biconditional</summary>

  - It is written $\Leftrightarrow$, corresponds to the phrase “if and only if” or “iff” for short. So P $\Leftrightarrow$ Q is true when both P and Q have the same truth value, otherwise it is false.

| P   | Q   | P $\Leftrightarrow$ Q |
| :-: | :-: | :-:                   |
| T   | T   | T                     |
| T   | F   | F                     |
| F   | T   | F                     |
| F   | F   | T                     |

</details>

<details><summary>Tautology</summary>

  - A logical expression that always evaluates to T, that is, the last column of its truth table consists of nothing but T’s. A tautology is sometimes said to be valid; although “valid” is used in other contexts as well, this should cause no confusion.

  - ex. (P $\land$ Q) $\lor$ P $\Leftrightarrow$ P is tautology.

| P   | Q   | P $\land$ Q | (P $\land$ Q) $\lor$ P | (P $\land$ Q) $\lor$ P $\Leftrightarrow$ P |
| :-: | :-: | :-:         | :-:                    | :-:                                        |
| T   | T   | T           | T                      | T                                          |
| T   | F   | F           | T                      | T                                          |
| F   | T   | F           | F                      | T                                          |
| F   | F   | F           | F                      | T                                          |

  - A few important tautologies.

    - P ⇔ ¬¬P
    - P ∨ Q ⇔ Q ∨ P
    - P ∧ Q ⇔ Q ∧ P
    - (P ∧ Q) ∧ R ⇔ P ∧ (Q ∧ R)
    - (P ∨ Q) ∨ R ⇔ P ∨ (Q ∨ R)
    - P ∧ (Q ∨ R) ⇔ (P ∧ Q) ∨ (P ∧ R)
    - P ∨ (Q ∧ R) ⇔ (P ∨ Q) ∧ (P ∨ R)
    - (P ⇒ Q) ⇔ (¬P ∨ Q)
    - P ⇒ (P ∨ Q)
    - P ∧ Q ⇒ Q
    - (P ⇔ Q) ⇔ ((P ⇒ Q) ∧ (Q ⇒ P))
    - (P ⇒ Q) ⇔ (¬Q ⇒ ¬P)

</details>

<details><summary>Equivalent</summary>

  - If two formulas always take on the same truth value no matter what elements from the universe of discourse we substitute for the various variables, then we say they are equivalent. The value of equivalent formulas is that they say the same thing. It is always a valid step in a proof to replace some formula by an equivalent one. In addition, many tautologies contain important ideas for constructing proofs.

</details>

<details><summary>Quantifier</summary>

  - Universal quantifier: A sentence $`\forall xP(x)`$ is true if and only if $`P(x)`$ is true no matter what value (from the universe of discourse) is substituted for x.
  - ex. $`\forall x (P(x) \Rightarrow Q(x))`$ may be read, "All x satisfying P(x) also satisfy Q(x)."
  - ex. $`\forall x P(x) \Rightarrow Q(x)`$ may be read, "If P(x) is true for all x, Q(x) is true."[^quantifier_note_0]
  - ex. $`\forall x (P(x) \Rightarrow Q(x)) \neq \forall x P(x) \Rightarrow \forall xQ(x)`$[^quantifier_note_1]
  - ex. If S is a set, the sentence “every x in S satisfies P(x)” is written formally as $`\forall x ((x \in S) \Rightarrow P(x))`$[^quantifier_note_2]

</details>

### Reference

- Patrick Keef, David Guichard, \<An Introduction to Higher Mathematics\>
- [수학의 즐거움](https://www.youtube.com/@enjoyingmath9346/featured)

[^truth_value_def]: In logic and mathematics, a truth value, sometimes called a logical value, is a value indicating the relation of a proposition to truth, which in classical logic has only two possible values (true or false). - [Wikipedia](https://en.wikipedia.org/wiki/Truth_value)
[^quantifier_note_0]: The x in P(x) is bound by the universal quantifier, but the x in Q(x) is not. The formula (∀xP(x)) ⇒ Q(x) has the same meaning as (∀xP(x)) ⇒ Q(y), and its truth depends on the value assigned to the variable in Q(·). Q(·) is not proposition until the variable is bound or assigned.
[^quantifier_note_1]: (∀xP(x)) ⇒ Q(x) might also be written as ∀x P(x) ⇒ Q(x), which is to say that the universal quantifier has higher precedence than the conditional.
[^quantifier_note_2]: For clarity and brevity, this is usually written ∀x ∈ S (P (x)). To understand and manipulate the formula ∀x∈S(P(x)) properly, you will sometimes need to “unabbreviate” it, rewriting it as ∀x ((x ∈ S) ⇒ P(x)).

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

  - If P is a formula, then “not P” i.e., "denial of P" is another formula, which we write symbolically as $\neg$ P.

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

  - A logical expression that always evaluates to T, that is, the last column of its truth table consists of nothing but T’s. A tautology is sometimes said to be valid; although “valid” is used in other contexts as well, this should cause no confusion. Many tautologies contain important ideas for constructing proofs.

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

  - If two formulas always take on the same truth value no matter what elements from the universe of discourse we substitute for the various variables, then we say they are equivalent. The value of equivalent formulas is that they say the same thing. It is always a valid step in a proof to replace some formula by an equivalent one.

</details>

<details><summary>Quantifier</summary>
  
  #### Universal quantifier
  - A sentence $`\forall x P(x)`$ is true if and only if P(x) is true no matter what value (from the universe of discourse) is substituted for x.
    - ex. $`\forall x (x^2 ≥ 0)`$, i.e., “The square of any number is not negative.”
    - ex. $`\forall a \forall b (a < b \Rightarrow f(a) < f(b))`$, i.e., "A function f is increasing."
    - ex. $`\forall x \forall y (x + y = y + x)`$, i.e., the commutative law of addition.
    - ex. $`\forall x \forall y \forall z((x + y) + z = x + (y + z))`$, i.e., the associative law of addition.
    - ex. $`\forall x`$ (x is a square $\Rightarrow$ x is a rectangle), i.e., “All squares are rectangles.”
    - ex. $`\forall x`$ (x lives in Walla Walla $\Rightarrow$ x lives in Washington), i.e., “Every person who lives in
  Walla Walla lives in Washington.”
    - ex. “If x is negative, so is its cube", i.e., “Every negative x has a negative cube.”, i.e., $`\forall x ((x < 0) \Rightarrow (x^3 < 0))`$
    - ex. “If two numbers have the same square, then they have the same absolute value”, i.e., $`\forall x \forall y ((x^2 = y^2) \Rightarrow (|x| = |y|))`$.
    - ex. “If x = y, then x + z = y + z”, i.e., $`\forall x \forall y \forall z ((x = y) \Rightarrow (x + z = y + z))`$.
    - ex. If S is a set, the sentence “Every x in S satisfies P(x)” is written formally as $`\forall x ((x \in S) \Rightarrow P(x))`$.[^quantifier_note_0]
    - ex. $`\forall x \in [0,1](\sqrt{x} \geq x)`$, i.e., $`\forall x(x \in [0,1] \Rightarrow \sqrt{x} \geq x)`$.
    - ex. $`\forall x < 0(|x| = −x)`$, i.e., $`\forall x(x < 0 \Rightarrow |x| = −x)`$.
    - ex. $`\forall x (P(x) \Rightarrow Q(x))`$, i.e., "All x satisfying P(x) also satisfy Q(x)."
    - ex. $`\forall x P(x) \Rightarrow Q(x)`$, i.e., "If P(x) is true for all x, Q(x) is true."[^quantifier_note_1]
    - ex. $`\forall x (P(x) \Rightarrow Q(x)) \neq \forall x P(x) \Rightarrow \forall x Q(x)`$.
    - ex. $`\forall x \forall y(P(x) \Rightarrow Q(y)) \neq \forall x(P(x)) \Rightarrow \forall y(Q(y))`$
  
  #### Existential quantifier
  - A sentence $`\exists x P(x)`$ is true if and only if there is at least one value of x (from the universe of discourse) that makes P(x) true.
    - ex. $`\exists x (x \geq x^2)`$ is true since x = 0 is one of many solutions.
    - ex. $`\exists x \exists y (x^2+y^2 =2xy)`$ is true since x = y = 1 is one of many solutions.
    - ex. $`\exists x (P(x) \land Q(x))`$, i.e., “Some x satisfying P(x) also satisfies Q(x).”
    - ex. “Some x satisfying P(x) satisfies Q(x)” should not be translated as $`\exists x (P(x) \Rightarrow Q(x))`$.[^quantifier_note_2]
    - ex. “No democrats are republicans,”, i.e., $`\forall x`$(x is a democrat $\Rightarrow$ x is not a republican).[^quantifier_note_3]
    - ex. “No triangles are rectangles,”, i.e., $`\forall x`$(x is a triangle $\Rightarrow$ x is not a rectangle).
    - ex. $`\exists x < 0(x^2 = 1)`$, i.e., $`\exists x ((x < 0) ∧ (x^2 = 1))`$
    - ex. $`\exists x \in [0,1](2x^2 + x = 1)`$, i.e., $`$\exists x((x \in [0,1]) ∧ (2x^2 + x = 1))`$
    - ex. $`\exists x \exists y (P(x) \land Q(y)) \Leftrightarrow \exists x(P(x)) \land \exists y(Q(y))`$ 

  #### Mixed quantifiers
  - The order of the quantifiers is extremely important.
    - ex. For x, y $\in\mathbb{R}$, $`\forall x, \exists y, x + y = 0 \neq \exists y, \forall x, x + y = 0`$.[^quantifier_note_4]
    - ex. $`\exists x \forall y(x + y = y), \quad\forall y \exists x(x + y = 0)`$[^quantifier_note_5]
    - ex. $`\forall x \exists y(y^3 = x), \quad\exists y \forall x (xy^3 = −x)`$[^quantifier_note_6]
    - ex. $`\forall x \exists y(x < y), \quad\exists y \forall x(x < y)`$[^quantifier_note_7]
    - ex. $`\forall x \forall y \exists z ((x < y) \Rightarrow (x < z < y))`$[^quantifier_note_8]
    - ex. For x, y, z $\in\mathbb{Z}$, $`\forall x \exists y \exists z (x = 7y + 5z), \quad\forall x \exists y \forall z (z > x \Rightarrow z ≥ y).`$[^quantifier_note_9]

</details>

<details><summary>De Morgan's Laws</summary>

- $`\neg(P \lor Q) \Leftrightarrow (\neg P \land \neg Q)`$

- $`\neg(P \land Q) \Leftrightarrow (\neg P \lor \neg Q)`$

- $`\neg \forall xP(x) \Leftrightarrow \exists x\neg P(x)`$

- $`\neg\exists xP(x) \Leftrightarrow \forall x\neg P(x)`$

- Examples

  - ex. A denial of “For every x, $x^2$ is positive” is “There is an x such that $x^2$ fails to be positive.”
  - ex. A denial of “There is an x such that $x^2$ = −1” is “For every x, $x^2 \neq −1$.”
  - ex. A denial of “All people are tall” is **not** "No people are tall."[^de_morgan_note_0]
  - ex. $`\neg\forall x (P(x) \Rightarrow Q(x)) \Leftrightarrow \exists x (P(x) \land \neg Q(x))`$
  - ex. $`\neg\exists x (P(x) \land Q(x)) \Leftrightarrow \forall x (P(x) \Rightarrow \neg Q(x))`$
  - ex. $`\neg(P \Rightarrow Q)`$ </br>
        $`\quad\Leftrightarrow \neg(\neg P \lor Q)`$ </br>
        $`\quad\Leftrightarrow (\neg \neg P ) \land (\neg Q)`$ </br>
        $`\quad\Leftrightarrow P \land \neg Q`$[^de_morgan_note_1]
  - ex. $`\neg\forall x (P(x) \lor \neg Q(x))`$ </br>
        $`\quad\Leftrightarrow \exists x \neg(P(x) \lor \neg Q(x))`$ </br>
        $`\quad\Leftrightarrow \exists x (\neg P(x) \land \neg\neg Q(x))`$ </br>
        $`\quad\Leftrightarrow \exists x (\neg P(x) \land Q(x))`$[^de_morgan_note_1]
  - ex. $`\forall x P(x) \Leftrightarrow \displaystyle\bigwedge_{x\in U} P(x)`$[^de_morgan_note_2]

  - ex. $`\exists x P(x) \Leftrightarrow \displaystyle\bigvee_{x\in U} P(x)`$[^de_morgan_note_2]

  - ex. $`\neg \displaystyle\bigwedge_{x\in U} P(x) \,\Leftrightarrow\, \displaystyle\bigvee_{x\in U} \neg P(x)`$

</details>

## Exercises

- <details><summary>Observe that $P \lor Q \Leftrightarrow \neg\neg(P \lor Q) \Leftrightarrow \neg(\neg P \land \neg Q)$, so $\lor$ can be expressed in terms of $\land$ and $\neg$.</summary>

  - a) Show how to express $\Rightarrow$ in terms of $\land$ and $\neg$. </br>
    $`\quad\; P \Rightarrow Q`$ </br>
    $`\Leftrightarrow \neg\neg(P \Rightarrow Q)`$ </br>
    $`\Leftrightarrow \neg\neg(\neg P \lor Q)`$ </br>
    $`\Leftrightarrow \neg(P \land \neg Q)`$ </br>
    
  - b) Show how to express $\land$ in terms of $\neg$ and $\lor$. </br>
    $`\quad\; P \land Q`$ </br>
    $`\Leftrightarrow \neg\neg(P \land Q)`$ </br>
    $`\Leftrightarrow \neg(\neg P \lor \neg Q)`$ </br>
    
  - c) Show how to express $\lor$ in terms of $\neg$ and $\Rightarrow$. </br>
    $`\quad\; P \lor Q`$ </br>
    $`\Leftrightarrow (\neg\neg P \lor Q)`$ </br>
    $`\Leftrightarrow (\neg P \Rightarrow Q)`$ </br>


</details>

### References

- Patrick Keef, David Guichard, \<An Introduction to Higher Mathematics\>
- [수학의 즐거움, \[증명기초 스터디\] 1. 진리표와 명제의 참거짓](https://youtu.be/zbWQTYOHft0?feature=shared)
- [수학의 즐거움, \[증명기초 스터디\] 2. 어떤 경우가 하나 존재하는 것과 모든 경우에 대한 논리를 구분하는 양화사](https://youtu.be/1MjvdWbkkow?feature=shared)
- [수학의 즐거움, \[역시 함께읽어야죠 수학책은\] 한정사, 합집합과 교집합, 공허참, 귀납법의 이해](https://youtu.be/EHUspq2TT_A?feature=shared)

[^truth_value_def]: In logic and mathematics, a truth value, sometimes called a logical value, is a value indicating the relation of a proposition to truth, which in classical logic has only two possible values (true or false). - [Wikipedia](https://en.wikipedia.org/wiki/Truth_value)
[^quantifier_note_0]: For clarity and brevity, this is usually written ∀x ∈ S (P (x)). To understand and manipulate the formula ∀x ∈ S(P(x)) properly, you will sometimes need to “unabbreviate” it, rewriting it as ∀x ((x ∈ S) ⇒ P(x)).
[^quantifier_note_1]: (∀xP(x)) ⇒ Q(x) might also be written as ∀x P(x) ⇒ Q(x), which is to say that the universal quantifier has higher precedence than the conditional. The x in P(x) is bound by the universal quantifier, but the x in Q(x) is not. The formula (∀xP(x)) ⇒ Q(x) has the same meaning as (∀xP(x)) ⇒ Q(y), and its truth depends on the value assigned to the variable in Q(·). Q(·) is not proposition until the variable is bound or assigned.
[^quantifier_note_2]: Suppose P(x) = “x is an apple” and Q(x) = “x is an orange.” The sentence “some apples are oranges” is certainly false, but
∃x(P(x) ⇒ Q(x)) is true. To see this suppose x0 is some particular orange. Then P(x0) ⇒ Q(x0) evaluates to F ⇒ T, which is T, and the existential quantifier is satisfied.
[^quantifier_note_3]: In general, the statement “no x satisfying P(x) satisfies Q(x)” can be written ∀x (P(x) ⇒ ¬Q(x)). It is also equivalent to ¬∃x(P(x) ∧ Q(x)).
[^quantifier_note_4]: ∀x,∃y(x + y = 0) ⟺ ∀x(∃y(x + y = 0)) ⟺ "For all x, there exists y which satisfies x + y = 0". ∃y∀x(x + y = 0) ⟺ ∃y(∀x(x + y = 0)) ⟺ "There exists y which satisfies that for all x, x + y = 0".
[^quantifier_note_5]: In the first we require that x be a fixed value that satisfies the equation regardless of the value of y; clearly x = 0 will do. In the second formula, however, x depends on y; if y = 3, x = −3, if y = 0, x = 0.
[^quantifier_note_6]: The first is valid because given any x we can set y equal to the cube root of x. So as x varies, y also varies, that is, y depends upon x. The second is valid because there is a single fixed value y = −1 which makes the equation xy^3 = −x valid, regardless of the value of x.
[^quantifier_note_7]: The first sentence is true and states that given any number there is a strictly larger number, that is, there is no largest number. The second sentence is false; it says that there is a single number that is strictly larger than all real numbers. In general, if you compare ∃y∀xP(x,y) with ∀x∃yP(x,y) it is clear that the first statement implies the second. If there is a fixed value y0 which makes P(x,y) true for all x, then no matter what x we are given, we can find a y (the fixed value y0) which makes P(x,y) true. So the first is a stronger statement. As in this example, it is usually the case that this implication cannot be reversed.
[^quantifier_note_8]: Observe that z depends in an essential way on both variables “to its left,” namely, x and y. The sentence is true if U = ℝ, but neither of these is true for ℝ: ∀x∃z∀y((x < y) ⇒ (x < z < y)), ∃z ∀x ∀y ((x < y) ⇒ (x < z < y)).
[^quantifier_note_9]: Consider the first sentence. If we know the value of x, we can choose y = −2x and z = 3x, so 7y+5z = −14x+15x = x. Notice that y and z depend on x in an essential way. Turning to the second, if we know x, we can choose y to be the next integer, x + 1. Any z is strictly larger than x if and only if it is at least as large as y.
[^de_morgan_note_0]: This might be called the opposite of the original sentence—it says more than simply “ ‘All people are tall’ is untrue.” The correct denial of this sentence is “there is someone who is not tall,” which is a considerably weaker statement.
[^de_morgan_note_1]: We can use De Morgan’s laws to simplify the denial of a formula. Denials can also be a helpful study device. When you read a theorem or a definition in mathematics it is frequently helpful to form the denial of that sentence to see what it means for the condition to fail. The more ways you think about a concept in mathematics, the clearer it should become.
[^de_morgan_note_2]: This is not really a “statement” in our official mathematical logic, because we don’t allow infinitely long formulas.

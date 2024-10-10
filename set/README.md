## Definitions

<details><summary>Set</summary>

  - A collection of definable objects, i.e., it should be possible to tell clearly whether a certain object is in the set or not.
  
  - Element is an object which is in the set.
    - ex. A = { 1, 2 }. 1 $\in$ A, 3 $\notin$ A.
    - ex. B = { x | P(x) }

</details>

<details><summary>Subset</summary>

  - Given two sets A and B, if all elements of A are also in B, we can say "A is a subset of B", which is written symbolically as "$`A \subseteq B`$".

  - $`A \subseteq A \Leftrightarrow \text{Given a set A, A is a subset of itself.}`$

  - $`A \subseteq B := \forall x(x \in A \Rightarrow x \in B)`$
    - ex. A = { a, b }, B = { a, b, c }. $`A \subset B`$

</details>

<details><summary>Empty set</summary>

  - A set which has no elements, which is written symbolically as "$`\emptyset`$".
  
  - $`\emptyset \subseteq A`$ $\Leftrightarrow$ For any set A, the empty set is a subset of A.
    - The only subset of the empty set is the empty set itself.
    - The power set of the empty set is the set containing only the empty set.

</details>

<details><summary>Power set</summary>

  - Given a set A, power set of A is a set which has all subsets of A as element.

  - $`P(A) := \{ B | B \subseteq A \}`$
    - ex. A = { 1, 2 }. P(A) = { $\emptyset$, { 1 }, { 2 }, { 1, 2 } }

</details>

<details><summary>Product set</summary>

  - Given two sets A and B, product set of A and B, i.e. cartesian product of A and B, is a set which has all possible pairs of (a, b) as an element, where a is one of A's elements and b is one of B's elements.

  - $`A \times B := \{ (a, b) | a \in A \land b \in B \}`$
    - ex. $`A = \{ a, b \}, B = \{ c, d \}. A \times B = \{ (a, c), (a, d), (b, c), (b, d) \}`$

</details>

<details><summary>Union</summary>

  - $`\text{Let A, B $\subseteq$ U.} A \cup B := \{ x | x \in A \,or\, x \in B \}`$

</details>

<details><summary>Intersection</summary>

  - $`\text{Let A, B $\subseteq$ U.} A \cap B := \{ x | x \in A \,and\, x \in B \}`$

</details>

<details><summary>Complement</summary>

  - $`A^{\complement} := \{ x | x \notin A \}`$

</details>

<details><summary>Equality</summary>
</br>
  
$`\begin{flalign}
\text{Let A, B $\subseteq$ U.} &&\\
\quad\;\; A = B &&\\
\Leftrightarrow A \subseteq B \,\land\, B \subseteq A &&\\
\Leftrightarrow \forall x(x \in A \Rightarrow x \in B) \,\land\, \forall x(x \in B \Rightarrow x \in A) &&\\
\end{flalign}`$

</details>

## Exercises

<details><summary>Show that $\sqrt{2}(x^2 = 2, x > 0)$ is not the rational number.</summary>
  
$`\begin{flalign}
\text{Proof.} &&\\
\quad\text{Suppose } \sqrt{2} \in \mathbb{Q}. &&\\
\Leftrightarrow \sqrt{2} = \frac{q}{p}(p \neq 0 \in \mathbb{N},q \in \mathbb{N}, p \perp q) &&\\
\Leftrightarrow 2 = (\frac{q}{p})^2 &&\\
\Leftrightarrow 2p^2 = q^2 &&\\
\Leftrightarrow q = 2k(k \in \mathbb{N}) &&\\
\Leftrightarrow p^2 = 2k^2 &&\\
\Leftrightarrow q = 2k^{\prime}(k^{\prime} \in \mathbb{N}) \text{ Contradiction! a and b are coprime by the assumption.} &&\\
\therefore \sqrt{2} \notin \mathbb{Q} &&\\
\end{flalign}`$

</details>

<details><summary>Let A, B, C $\subseteq$ U. Show that ...</summary>
  
- <details><summary>A $\cap$ (B $\cup$ C) = (A $\cap$ B) $\cup$ (A $\cap$ C)</summary>

  $`\begin{flalign}
  \text{Need to show. } &&\\
  \quad A \cap (B \cup C) \subseteq (A \cap B) \cup (A \cap C) \quad and \quad (A \cap B) \cup (A \cap C) \subseteq A \cap (B \cup C) &&\\
  \text{Proof.} &&\\
  \quad A \cap (B \cup C) &&\\
  = \{ x | x \in A \:and\: (x \in B \:or\: x \in C) \} &&\\
  = \{ x | (x \in A \:and\: x \in B) \:or\: (x \in A \:and\: x \in C) \} &&\\
  = \{ x | x \in A \cap B \:or\: x \in A \cap C \} &&\\
  = (A \cap B) \cup (A \cap C) &&\\
  \end{flalign}`$

  </details>

- <details><summary>A $\cup$ (B $\cap$ C) = (A $\cup$ B) $\cap$ (A $\cup$ C)</summary>

  $`\begin{flalign}
  \text{Need to show. } &&\\
  \quad A \cup (B \cap C) \subseteq (A \cup B) \cap (A \cup C) \quad and \quad (A \cup B) \cap (A \cup C) \subseteq A \cup (B \cap C) &&\\
  \text{Proof.} &&\\
  \quad A \cup (B \cap C) &&\\
  = \{ x | x \in A \:or\: (x \in B \:and\: x \in C) \} &&\\
  = \{ x | (x \in A \:or\: x \in B) \:and\: (x \in A \:or\: x \in C) \} &&\\
  = \{ x | x \in A \cup B \:and\: x \in A \cup C \} &&\\
  = (A \cup B) \cap (A \cup C) &&\\
  \end{flalign}`$

  </details>

- <details><summary>$(A \cup B)^{\complement} = A^{\complement} \cap B^{\complement}$</summary>

  $`\begin{flalign}
  \text{Need to show. } &&\\
  \quad (A \cup B)^{\complement} \subseteq A^{\complement} \cap B^{\complement} \quad and\quad  A^{\complement} \cap B^{\complement} \subseteq (A \cup B)^{\complement} &&\\
  \text{Proof.} &&\\
  \quad (A \cup B)^{\complement} &&\\
  = \{ x | x \notin (A \cup B) \} &&\\
  = \{ x | \neg(x \in (A \cup B)) \} &&\\
  = \{ x | \neg(x \in A \:or\: x \in B) \} &&\\
  = \{ x | \neg(x \in A) \:and\: \neg(x \in B) \} &&\\
  = \{ x | x \notin A \:and\: x \notin B) \} &&\\
  = \{ x | x \in A^{\complement} \:and\: x \in B^{\complement}) \} &&\\
  = A^{\complement} \cap B^{\complement}
  \end{flalign}`$
  
  </details>

- <details><summary>$(A \cap B)^{\complement} = A^{\complement} \cup B^{\complement}$</summary>

  $`\begin{flalign}
  \text{Need to show. } &&\\
  \quad (A \cap B)^{\complement} \subseteq A^{\complement} \cup B^{\complement} \quad and \quad A^{\complement} \cup B^{\complement} \subseteq (A \cap B)^{\complement} &&\\
  \text{Proof.} &&\\
  \quad (A \cap B)^{\complement} &&\\
  = \{ x | x \notin (A \cap B) \} &&\\
  = \{ x | \neg(x \in (A \cap B)) \} &&\\
  = \{ x | \neg(x \in A \:and\: x \in B) \} &&\\
  = \{ x | \neg(x \in A) \:or\: \neg(x \in B) \} &&\\
  = \{ x | x \notin A \:or\: x \notin B) \} &&\\
  = \{ x | x \in A^{\complement} \:or\: x \in B^{\complement}) \} &&\\
  = A^{\complement} \cup B^{\complement}
  \end{flalign}`$
  
  </details>

</details>

<details><summary>If A has n elements, then show that P(A) has $2^{n}$ elements.</summary>
  
$`\begin{flalign}
\text{Proof.} &&\\
\quad Let\: Q_{x} \:be\: \forall x \in Z, x \geq 0(n(A) = x \Rightarrow n(P(A)) = 2^{x}). &&\\
\quad Let A_{k+1} = \{ a_{1}, a_{2}, \dots , a_{k+1} \} \: (k \in \mathbb{Z}, \: k + 1 > 0), A_{0} = \emptyset. &&\\
\quad \text{Let } \otimes \text{ an operation which is defined as } \{ A^{\prime} \cup B^{\prime} | A^{\prime} \subseteq A \;and\; B^{\prime} \subseteq B \} \text{, so that } n(A \otimes B) = n(A \times B) = n(A) \times n(B). &&\\
\quad A_{0} \text{has 0 element so that } P(A) = \{ \emptyset \}. \; \therefore \, Q_{0} \text{ is true} &&\\
\quad \text{If we assume that } Q_{k} \text{ is true, } P(A_{k+1}) = P(A_{k}) \otimes P(\{ a_{k+1} \}). &&\\
\quad n(P(A_{k+1})) &&\\
= n(P(A_{k}) \otimes P(\{ a_{k+1} \})) &&\\
= n(P(A_{k})) \times n(P(\{ a_{k+1} \})) &&\\
= 2^{k} \times 2 = 2^{k+1} \; \therefore \, Q_{k+1} \text{ is true.} &&\\
\end{flalign}`$

</details>

## TODO

- 공집합의 필요성. 모든 집합의 부분집합으로서 공집합이 포함되는 이유.

### References

- [수학의 즐거움, 기초부터 대학원 수학까지, 1. 집합론 기초 (a)](https://youtu.be/9HUk8zays2E?feature=shared)
- [수학의 즐거움, \[기초부터 대학원 수학까지 시리즈 스터디 3기\] 첫시간, 집합론 기초 1강](https://youtu.be/PZXafFesmHI?feature=shared)
- [Wikipedia, 'Empty set'](https://en.wikipedia.org/wiki/Empty_set)

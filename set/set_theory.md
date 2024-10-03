## Definition

<details><summary>Set</summary>

  - A collection of definable objects, i.e., it should be possible to tell clearly whether a certain object is in the set or not.
  
  - Element is an object which is in the set.
    - ex. A = { 1, 2 }. 1 $\in$ A, 3 $\notin$ A.
    - ex. B = { x | P(x) }

</details>

<details><summary>Subset</summary>

  - Given two sets A, B, if all elements of A are also in B, we can say "A is a subset of B", which is written symbolically as "$`A \subseteq B`$".
    - ex. A = { a, b }, B = { a, b, c }. $`A \subset B`$

</details>

<details><summary>Empty set</summary>

  - A set which has no elements, which is written symbolically as "$`\emptyset`$".
  
  - $`\emptyset \subset A`$ $\Leftrightarrow$ For any set A, the empty set is a subset of A.
    - The only subset of the empty set is the empty set itself.

</details>

<details><summary>Power set</summary>

  - Given a set A, power set of A is a set which has all subsets of A as element.
    - ex. C = { 1, 2 }. P(C) = { $\emptyset$, { 1 }, { 2 }, { 1, 2 } }

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
A = B &&\\
\Leftrightarrow A \subseteq B \,and\, B \subseteq A &&\\
\Leftrightarrow \text{If} x \in A, \,\text{then}\, x \in B \,and\, \text{if} y \in B, \,\text{then}\, y \in A.
\end{flalign}`$

</details>

## Exercise

<details><summary>Show that $\sqrt{2}(x^2 = 2, x > 0)$ is not the rational number.</summary>
</br>
  
$`\begin{flalign}
\text{Proof.} &&\\
\text{Suppose } \sqrt{2} \in \mathbb{Q}. &&\\
\Leftrightarrow \sqrt{2} = \frac{q}{p}(p \neq 0 \in \mathbb{N},q \in \mathbb{N}, p \perp q) &&\\
\Leftrightarrow 2 = (\frac{q}{p})^2 &&\\
\Leftrightarrow 2p^2 = q^2 &&\\
\Leftrightarrow q = 2k(k \in \mathbb{N}) &&\\
\Leftrightarrow p^2 = 2k^2 &&\\
\Leftrightarrow q = 2k^{\prime}(k^{\prime} \in \mathbb{N}) \text{ Contradiction! a and b are coprime by the assumption.} &&\\
\therefore \sqrt{2} \notin \mathbb{Q} &&\\
\end{flalign}`$

</details>

<details><summary>Let A, B, C $\subset$ U. A $\cap$ (B $\cup$ C) = (A $\cap$ B) $\cup$ (A $\cap$ C) </summary>
</br>

$`\begin{flalign}
\text{Need to show. } 
\text{Proof.} &&\\
\text{Suppose } \sqrt{2} \in \mathbb{Q}. &&\\
\Leftrightarrow \sqrt{2} = \frac{q}{p}(p \neq 0 \in \mathbb{N},q \in \mathbb{N}, p \perp q) &&\\
\Leftrightarrow 2 = (\frac{q}{p})^2 &&\\
\Leftrightarrow 2p^2 = q^2 &&\\
\Leftrightarrow q = 2k(k \in \mathbb{N}) &&\\
\Leftrightarrow p^2 = 2k^2 &&\\
\Leftrightarrow q = 2k^{\prime}(k^{\prime} \in \mathbb{N}) \text{ Contradiction! a and b are coprime by the assumption.} &&\\
\therefore \sqrt{2} \notin \mathbb{Q} &&\\
\end{flalign}`$

</details>

## TODO

- 공집합의 필요성. 모든 집합의 부분집합으로서 공집합이 포함되는 이유.

### Reference

- [수학의 즐거움, 기초부터 대학원 수학까지, 1. 집합론 기초 (a)](https://youtu.be/9HUk8zays2E?feature=shared)
- [수학의 즐거움, \[기초부터 대학원 수학까지 시리즈 스터디 3기\] 첫시간, 집합론 기초 1강](https://youtu.be/PZXafFesmHI?feature=shared)
- [Wikipedia](https://en.wikipedia.org/wiki/Empty_set)

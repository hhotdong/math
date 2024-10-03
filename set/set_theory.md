## Definitions

<details><summary>Set</summary>

  - A collection of definable objects, i.e., it should be possible to tell clearly whether a certain object is contained in the set or not.
    - ex. Given a set A = { 1, 2 }. 1 $\in$ A, 3 $\notin$ A.
    - ex. B = { x | P(x) }
    - ex. Given a set C = { 1, 2 }. Power set of C is P(C) = { $\emptyset$, { 1 }, { 2 }, { 1, 2 } }

</details>

## Exercise

<details><summary>Show that $\sqrt{2}(x^2 = 2, x > 0)$ is not the rational number.</summary>
</br>
  
$`\begin{flalign}
\text{Suppose }\sqrt{2} \in \mathbb{Q}. &&\\
\Leftrightarrow \sqrt{2} = \frac{q}{p}(p,q \in \mathbb{Z}, p \neq 0) &&\\
\Leftrightarrow 2 = (\frac{q}{p})^2 &&\\
\Leftrightarrow 2p^2 = q^2\text{(p가 짝수이고, q가 홀수인 경우 모순)} &&\\
\therefore \sqrt{2} \notin \mathbb{Q} &&\\
\end{flalign}`$

</details>

## TODO

- 집합 A에서 B로의 사상이 정의되기 위해서는 domain A의 모든 원소가 codomain의 원소와 연결돼야 하는데, 그 이유는 무엇인가?

- $A \cup (B \cap C)$ 

&emsp; $\Leftrightarrow$ $\\{\\,  x | x \in A \lor (x \in B \land x \in C)  \\,\\}$

&emsp; $\Leftrightarrow$ $\\{\\,  x | (x \in A \lor x \in B) \land (x \in A \lor x \in C)  \\,\\}$

&emsp; 에서 전개되는 방식은 논리합, 논리곱의 분배법칙에 따른 것인지? 아니면 직관적인 이해가 가능할지?

- 공집합의 필요성? 모든 집합의 부분집합으로서 공집합이 포함되는 이유는?

### References

- [수학의 즐거움, <기초부터 대학원 수학까지, 1. 집합론 기초 (a)>](https://youtu.be/9HUk8zays2E?feature=shared)

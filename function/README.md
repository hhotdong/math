## Definitions

<details><summary>Function</summary>

  -  Given two sets A, B, we call $`f : A \rightarrow B`$ is a function, so we have $`S_f \subseteq A \times B \text{ satisfying for each } a \in A, \text{ there exists } b \in B \text{ uniquely such that } (a, b) \in S_f`$.

![image](images/function_diagram.jpg)

  - The domain of $`f`$ is $`Dom(f)=A`$.

  - The codomain of $`f`$ is $`Cdm(f)=B`$.

  - The image$`_{range}`$ of $`f`$ is the set, which is defined as $`Img(f) = f[A] := \{ b = f(a) | a \in A \}`$.

  - The inverse$`_{pre}`$ image of $`B_1\subset B`$ under f is the set, which is defined as $`Img^{-1}(f) = f^{-1}[B_1] := \{ x \in A | f(x) \in B_1 \}`$.

</details>

## Exercises

<details><summary>Given f: A $\rightarrow$ B a function, let A₁, A₂ ⊆ A, show that ...</summary>

  - <details><summary>f(A₁ ∪ A₂) := {f(x)|x ∈ (A₁ ∪ A₂)} = f(A₁) ∪ f(A₂)</summary>

    $`\begin{flalign}
    \text{Need to show. } &&\\
    \quad (A \cup B)^{\complement} \subseteq A^{\complement} \cap B^{\complement} \:and\: A^{\complement} \cap B^{\complement} \subseteq (A \cup B)^{\complement} &&\\
    \text{Proof.} &&\\
    \quad (A \cup B)^{\complement} &&\\
    \Leftrightarrow \{ x | x \notin (A \cup B) \} &&\\
    \Leftrightarrow \{ x | \neg(x \in (A \cup B)) \} &&\\
    \Leftrightarrow \{ x | \neg(x \in A \:or\: x \in B) \} &&\\
    \Leftrightarrow \{ x | \neg(x \in A) \:and\: \neg(x \in B) \} &&\\
    \Leftrightarrow \{ x | x \notin A \:and\: x \notin B) \} &&\\
    \Leftrightarrow \{ x | x \in A^{\complement} \:and\: x \in B^{\complement}) \} &&\\
    \Leftrightarrow A^{\complement} \cap B^{\complement}
    \end{flalign}`$

    </details>

  - <details><summary>f(A₁ ∩ A₂) ⊆ f(A₁) ∩ f(A₂)</summary>
    
    </details>

</details>

### References

- [수학의 즐거움, \[수학 공부, 기초부터 대학원 수학까지, 1. 집합론 기초 (a)\]](https://youtu.be/9HUk8zays2E?feature=shared)
- [수학의 즐거움, \[기초부터 대학원 수학까지 시리즈 스터디 3기\] 2. 집합론 기초 2강](https://youtu.be/PPYhmRwbEno?feature=shared)

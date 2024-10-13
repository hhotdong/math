## Definitions

<details><summary>Function</summary>

  -  Given two sets A, B, we call $`f : A \rightarrow B`$ is a function, where $`S_f \subseteq A \times B \text{ satisfying for each } a \in A, \text{ there exists } b \in B \text{ uniquely s.t. } (a, b) \in S_f`$. That is, every element of A relates to exactly one element of B.

![image](images/function_diagram.jpg)

  - The domain of $`f`$ is $`Dom(f)=A`$.

  - The codomain of $`f`$ is $`Cdm(f)=B`$.

  - The image$`_{range}`$ of $`f`$ is the set, which is defined as $`Img(f) = f[A] := \{ b = f(a) | a \in A \} \Leftrightarrow \{ b \in B | \exists a \in A(b = f(a))\} \subseteq B`$.

  - The inverse$`_{pre}`$ image of $`B_1\subset B`$ under f is the set, which is defined as $`Img^{-1}(f) = f^{-1}[B_1] := \{ a \in A | f(a) \in B_1 \} \subseteq A`$.

</details>

## Exercises

<details><summary>Given f: A $\rightarrow$ B a function, let A₁, A₂ ⊆ A, show that ...</summary>

  - <details><summary>f(A₁ ∪ A₂) = f(A₁) ∪ f(A₂)</summary>

    $`\begin{flalign}
    \text{Need to show.} &&\\
    f(A_1 \cup A_2) \subseteq f(A_1) \cup f(A_2) \;\; and \;\; f(A_1) \cup f(A_2) \subseteq f(A_1 \cup A_2) &&\\
    &&\\
    \text{Proof.} &&\\
    \text{Recall that } b \in f(A) \Leftrightarrow \exists a \in A(f(a) = b). &&\\
    (\subseteq) &&\\
    \text{Let } b \in f(A_1 \cup A_2). &&\\
    \Leftrightarrow \exists a \in A_1 \cup A_2(f(a) = b) &&\\
    \Leftrightarrow \exists a((a \in A_1 \cup A_2) \land (f(a) = b)) &&\\
    \Leftrightarrow \exists a((a \in A_1 \lor a \in A_2) \land (f(a) = b)) &&\\
    \Leftrightarrow \exists a((a \in A_1 \land (f(a) = b)) \lor (a \in A_2 \land (f(a) = b))) &&\\
    \Rightarrow f(a) \in f(A_1) \lor f(a) \in f(A_2) &&\\
    \Leftrightarrow b \in f(A_1) \cup f(A_2) &&\\
    (\supseteq) &&\\
    \text{Let } b \in f(A_1) \cup f(A_2). &&\\
    \Leftrightarrow b \in f(A_1) \lor b \in f(A_2) &&\\
    \text{(Case 1) } b \in f(A_1) \Rightarrow \exists a_1 \in A_1(f(a_1) = b) &&\\
    \text{(Case 2) } b \in f(A_2) \Rightarrow \exists a_2 \in A_2(f(a_2) = b) &&\\
    \text{That is, } \exists a \in A_1 \cup A_2(f(a) = b). &&\\
    \Leftrightarrow \exists a((a \in A_1 \cup A_2) \land (f(a) = b)) &&\\
    \Rightarrow b \in f(A_1 \cup A_2) &&\\
    \end{flalign}`$

    </details>

  - <details><summary>f(A₁ ∩ A₂) ⊆ f(A₁) ∩ f(A₂)</summary>

    $`\begin{flalign}
    \text{Need to show.} &&\\
    f(A_1 \cap A_2) \subseteq f(A_1) \cap f(A_2) \;\; and \;\; f(A_1) \cap f(A_2) \nsubseteq f(A_1 \cap A_2) &&\\
    &&\\
    \text{Proof 1.} &&\\
    \text{Recall that } b \in f(A) \Leftrightarrow \exists a \in A(f(a) = b). &&\\
    (\subseteq) &&\\
    \text{Let } b \in f(A_1 \cap A_2). &&\\
    \Leftrightarrow \exists a \in A_1 \cap A_2(f(a) = b) &&\\
    \Leftrightarrow \exists a((a \in A_1 \cap A_2) \land (f(a) = b)) &&\\
    \Leftrightarrow \exists a((a \in A_1 \land a \in A_2) \land (f(a) = b)) &&\\
    \Leftrightarrow \exists a((a \in A_1 \land (f(a) = b)) \land (a \in A_2 \land (f(a) = b))) &&\\
    \Rightarrow f(a) \in f(A_1) \land f(a) \in f(A_2) &&\\
    \Rightarrow b \in f(A_1) \cap f(A_2) &&\\
    (\nsupseteq) &&\\
    \text{Counter example. Let } A_1 = \{ 1, 2 \}, A_2 = \{ 2, 3 \}, B = \{ 4, 5 \}, S_f = \{ (1, 4), (2, 5), (3, 4) \}. &&\\
    f(A_1) \cap f(A_2) = \{ 4, 5 \} &&\\
    f(A_1 \cap A_2) = \{ 5 \} &&\\
    &&\\
    \text{Proof 2.} &&\\
    \text{If b ∈ B is in f(A₁ ∩ A₂), then b = f(a) for some a ∈ A₁ ∩ A₂.} &&\\
    \text{Since a ∈ A₁ ∩ A₂, a is in both A₁ and A₂.} &&\\
    \text{Therefore, b = f(a) is in both f(A₁) and f(A₂), that is, b ∈ f(A₁) ∩ f(A₂).} &&\\
    \end{flalign}`$

    </details>

</details>

<details><summary>Given f: A $\rightarrow$ B a function, let B₁, B₂ ⊆ B, show that ...</summary>

  - <details><summary>$f^{-1}$(B₁ ∪ B₂) = $f^{-1}$(B₁) ∪ $f^{-1}$(B₂)</summary>

    $`\begin{flalign}
    \text{Need to show.} &&\\
    f^{-1}(B_1 \cup B_2) \subseteq f^{-1}(B_1) \cup f^{-1}(B_2) \;\; and \;\; f^{-1}(B_1) \cup f^{-1}(B_2) \subseteq f^{-1}(B_1 \cup B_2) &&\\
    &&\\
    \text{Proof.} &&\\
    \text{Recall that } a \in f^{-1}(B) \Leftrightarrow f(a) \in B. &&\\
    (\subseteq, \supseteq) &&\\
    \text{Let } a \in f^{-1}(B_1 \cup B_2). &&\\
    \Leftrightarrow f(a) \in B_1 \cup B_2 &&\\
    \Leftrightarrow f(a) \in B_1 \lor f(a) \in B_2 &&\\
    \Leftrightarrow a \in f^{-1}(B_1) \lor a \in f^{-1}(B_2) &&\\
    \Leftrightarrow a \in f^{-1}(B_1) \cup f^{-1}(B_2) &&\\
    \end{flalign}`$

    </details>

  - <details><summary>$f^{-1}$(B₁ ∩ B₂) = $f^{-1}$(B₁) ∩ $f^{-1}$(B₂)</summary>

    $`\begin{flalign}
    \text{Need to show.} &&\\
    f^{-1}(B_1 \cap B_2) \subseteq f^{-1}(B_1) \cap f^{-1}(B_2) \;\; and \;\; f^{-1}(B_1) \cap f^{-1}(B_2) \subseteq f^{-1}(B_1 \cap B_2) &&\\
    \text{Proof.} &&\\
    \text{Recall that } a \in f^{-1}(B) \Leftrightarrow f(a) \in B. &&\\
    (\subseteq, \supseteq) &&\\
    \text{Let } a \in f^{-1}(B_1 \cap B_2). &&\\
    \Leftrightarrow f(a) \in B_1 \cap B_2 &&\\
    \Leftrightarrow f(a) \in B_1 \land f(a) \in B_2 &&\\
    \Leftrightarrow a \in f^{-1}(B_1) \land a \in f^{-1}(B_2) &&\\
    \Leftrightarrow a \in f^{-1}(B_1) \cap f^{-1}(B_2) &&\\
    \end{flalign}`$

    </details>

  - <details><summary>$f^{-1}$(B₁ $^{\complement}$) = $f^{-1}$(B₁) $^{\complement}$</summary>

    $`\begin{flalign}
    \text{Need to show.} &&\\
    f^{-1}(B_1^{\complement}) \subseteq f^{-1}(B_1)^{\complement} \;\; and \;\; f^{-1}(B_1)^{\complement} \subseteq f^{-1}(B_1^{\complement}) &&\\
    &&\\
    \text{Proof.} &&\\
    \text{Recall that } a \in f^{-1}(B) \Leftrightarrow f(a) \in B. &&\\
    (\subseteq, \supseteq) &&\\
    \text{Let } a \in f^{-1}(B_1^{\complement}). &&\\
    \Leftrightarrow f(a) \in B_1^{\complement} &&\\
    \Leftrightarrow f(a) \notin B_1 &&\\
    \Leftrightarrow \neg(f(a) \in B_1) &&\\
    \Leftrightarrow \neg(a \in f^{-1}(B_1)) &&\\
    \Leftrightarrow a \notin f^{-1}(B_1) &&\\
    \Leftrightarrow a \in f^{-1}(B_1)^{\complement} &&\\
    \end{flalign}`$

    </details>

</details>

### References

- Patrick Keef, David Guichard, \<An Introduction to Higher Mathematics\>
- [수학의 즐거움, Enjoying Math, "수학 공부, 기초부터 대학원 수학까지, 1. 집합론 기초 (a)"](https://youtu.be/9HUk8zays2E?feature=shared)
- [수학의 즐거움, Enjoying Math, "\[기초부터 대학원 수학까지 시리즈 스터디 3기\] 2. 집합론 기초 2강\]"](https://youtu.be/PPYhmRwbEno?feature=shared)
- [Hacker-Code-J, GitHub repository](https://github.com/Hacker-Code-J/Modern-Mathematics/blob/main/grad-math-mini/grad-math-mini-1.pdf)

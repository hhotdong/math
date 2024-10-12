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
    \text{Proof.} &&\\
    \text{Recall that } b \in f(A) \Leftrightarrow \exists a \in A(b = f(a)). &&\\
    (\subseteq) &&\\
    \text{Let } b \in f(A_1 \cup A_2). &&\\
    \quad f(A_1 \cup A_2) &&\\
    = \{ b = f(a) | a \in (A_1 \cup A_2) \} &&\\
    = \{ b = f(a) | a \in A_1 \lor a \in A_2) \} &&\\
    \text{(Case 1) } a \in A_1 \Rightarrow f(a) \in f(A_1) &&\\
    \text{(Case 2) } a \in A_2 \Rightarrow f(a) \in f(A_2) &&\\
    \text{Thus, } f(A_1 \cup A_2) \subseteq f(A_1) \cup f(A_2). &&\\
    (\supseteq) &&\\
    \text{Let } b \in f(A_1) \cup f(A_2). &&\\
    \quad f(A_1) \cup f(A_2) &&\\
    = \{ b | b \in f(A_1) \lor b \in f(A_2) \} &&\\
    \text{(Case 1) } b \in f(A_1) \Rightarrow \exists a_1 \in A_1(b = f(a_1)) &&\\
    \text{(Case 2) } b \in f(A_2) \Rightarrow \exists a_2 \in A_2(b = f(a_2)) &&\\
    \text{That is, } \exists a \in A_1 \cup A_2(b = f(a)). \text{Thus, } b \in f(A_1 \cup A_2). &&\\
    \end{flalign}`$

    </details>

  - <details><summary>f(A₁ ∩ A₂) ⊆ f(A₁) ∩ f(A₂)</summary>

    $`\begin{flalign}
    \text{Need to show.} &&\\
    f(A_1 \cap A_2) \subseteq f(A_1) \cap f(A_2) \;\; and \;\; f(A_1) \cap f(A_2) \nsubseteq f(A_1 \cap A_2) &&\\
    \text{Proof.} &&\\
    (\subseteq) &&\\
    \text{Let } b \in f(A_1 \cap A_2). &&\\
    \quad f(A_1 \cap A_2) &&\\
    = \{ b = f(a) | a \in (A_1 \cap A_2) \} &&\\
    = \{ b = f(a) | a \in A_1 \land a \in A_2) \} &&\\
    \Rightarrow b \in f(A_1) \land b \in f(A_2) &&\\
    \Leftrightarrow b \in f(A_1) \cap f(A_2) &&\\
    \end{flalign}`$

    - If b $\in$ B is in f(W $\cap$ X), then b = f(a) for some a $\in$ W $\cap$ X. Since a $\in$ W $\cap$ X, a is in both W and X. Therefore, b = f(a) is in both f(W) and f(X), that is, b $\in$ f(W) $\cap$ f(X).
    </br>
    
    $`\begin{flalign}
    (\nsupseteq) &&\\
    \text{Counter example. Let } A_1 = \{ 1, 2 \}, A_2 = \{ 2, 3 \}, B = \{ 4, 5 \}, S_f = \{ (1, 4), (2, 5), (3, 4) \}. &&\\
    f(A_1) \cap f(A_2) = \{ 4, 5 \} &&\\
    f(A_1 \cap A_2) = \{ 5 \} &&\\
    \end{flalign}`$

    </details>

  - <details><summary>$f^{-1}$(A₁ ∪ A₂) = $f^{-1}$(A₁) ∪ $f^{-1}$(A₂)</summary>

    </details>

  - <details><summary>$f^{-1}$(A₁ ∩ A₂) = $f^{-1}$(A₁) ∩ $f^{-1}$(A₂)</summary>

    </details>

</details>

### References

- Patrick Keef, David Guichard, \<An Introduction to Higher Mathematics\>
- [수학의 즐거움, Enjoying Math, "수학 공부, 기초부터 대학원 수학까지, 1. 집합론 기초 (a)"](https://youtu.be/9HUk8zays2E?feature=shared)
- [수학의 즐거움, Enjoying Math, "\[기초부터 대학원 수학까지 시리즈 스터디 3기\] 2. 집합론 기초 2강\]"](https://youtu.be/PPYhmRwbEno?feature=shared)
- [Hacker-Code-J, GitHub repository](https://github.com/Hacker-Code-J/Modern-Mathematics/blob/main/grad-math-mini/grad-math-mini-1.pdf)

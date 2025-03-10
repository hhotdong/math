## Definitions

<details><summary>Function</summary>

  -  Given two sets A, B, we call $`f : A \rightarrow B`$ is a function, where $`S_f \subseteq A \times B \text{ satisfying for each } a \in A, \text{ there exists } b \in B \text{ uniquely s.t. } (a, b) \in S_f`$. That is, every element of A relates to exactly one element of B.

![image](images/function_diagram.jpg)

  - The domain of $`f`$ is $`Dom(f)=A`$.

  - The codomain of $`f`$ is $`Cdm(f)=B`$.

  - The image$`_{range}`$ of $`f`$ is the set, which is defined as $`Img(f) = f(A) = f[A]`$ </br>
    $`:= \{ b = f(a) | a \in A \}$`$ </br>
    $`= \{ b \in B | \exists a \in A(f(a) = b)\} \subseteq B`$.

  - The inverse$`_{pre}`$ image of $`B_1\subset B`$ under f is the set, which is defined as $`Img^{-1}(f) = f^{-1}(B_1) = f^{-1}[B_1]`$ </br>
    $`:= \{ a \in A | f(a) \in B_1 \} \subseteq A`$ </br>
    $`= \{ a \in A | \exists b \in B_1(b = f(a)) \} \subseteq A`$

    - If there is no element of A whose images lie in $B_1$, $`f^{-1}(B_1) = \emptyset`$.

</details>

<details><summary>Injective</summary>

  - Let f: A $\rightarrow$ B a function, f is one to one if $`f(x_1) = f(x_2)`$ then $`x_1 = x_2 \Leftrightarrow \text{if } x_1 \neq x_2 \text{then } f(x_1) \neq f(x_2)`$.

</details>

<details><summary>Surjective</summary>

  - Let f: A $\rightarrow$ B a function, f is onto if $`\forall b \in B \exists a \in A(f(a) = b)`$.

</details>

<details><summary>Inverse function</summary>

  - Let f: A $\rightarrow$ B a function, which is bijective(one to one, onto). Then we can define $f^{-1}$: B $\rightarrow$ A, called inverse function.  i.e., $`S_{f^{-1}} := \{ (b, a) \in B \times A | f(a) = b \} \subset B \times A`$.

</details>

<details><summary>Function composition</summary>

  - Given two functions f: A $\rightarrow$ B, g: B $\rightarrow$ C, define g $\circ$ f: A $\xrightarrow{f}$ B $\xrightarrow{g}$ C, i.e., (g $\circ$ f)(x) = g(f(x)), $`S_{g \circ f} = \{ (x, g(f(x)) | x \in A \} \subset A \times C`$.

</details>

<details><summary>Relation</summary>

  - Given two sets A, B, a relation R $`\subset A \times B`$, i.e., for each (a, b) $\in$ R, denote $`a`$ ~ $_{R}b$.
    - ex. $`A = \{ 1, 2 \}, B = \{ 4, 5 \}, A \times B = \{ (1, 4), (1, 5), (2, 4), (2, 5) \}`$. </br>
      $`R = \{ (1, 4), (2, 5) \} \Leftrightarrow`$ $`1`$ ~ $`_{R}4`$ , $`2`$ ~ $`_{R}5`$

</details>

<details><summary>Equivalence relation</summary>

  - Let R $\subseteq$ A $\times$ A be a relation. We say that R is an equivalence relation if R satisfies ...
    1. Reflexive: For each x $\in$ A, (x, x) $\in$ R, i.e., $`x`$ ~ $`_{R}x`$.
    2. Symmetric: If (x, y) $\in$ R then (y, x) $\in$ R, i.e., if $`x`$ ~ $`_{R}y`$ then $`y`$ ~ $`_{R}x`$.
    3. Transitive: If (x, y) $\in$ R and (y, z) $\in$ R, then (x, z) $\in$ R, i.e., if $`x`$ ~ $`_{R}y`$ and $`y`$ ~ $`_{R}z`$ then $`x`$ ~ $`_{R}z`$.
  
  - ex. $`A = \{ 1, 2, 3, 4 \}, R = \{ (1, 1), (2, 2), (3, 3), (4, 4), (1, 2), (2, 1) \}`$.[^equivalence_relation_0]

</details>

<details><summary>Partition</summary>

  - Given a set $`E`$, consider the index set $`I`$(i.e., for each $`\alpha\in I`$, there exists $`E_{\alpha}\subset E`$).</br>
  Define $`F := \{ E_{\alpha} \subseteq E \; | `$</br>
  $`\quad ① E_{\alpha} \neq \emptyset.`$</br>
  $`\quad ② \alpha\neq\beta, \alpha,\beta\in I \Rightarrow E_{\alpha} \cap E_{\beta} = \emptyset.`$</br>
  $`\quad ③ \bigcup_{\substack{\alpha \in I}} E_{\alpha} = \{ x \in E | \text{there exists } \alpha \in I \text{ s.t. } x \in E_{\alpha} \} = E`$</br>
  We call $`F`$ the partition of E.

  - ex. Let $`\mathbb{Z}`$ be set of integers. Denote $`[k] = \{ x \in \mathbb{Z} | x = 3a+k, a \in \mathbb{Z} \} \Rightarrow [0],[1],[2] \subseteq \mathbb{Z}`$.</br>
  $`\quad [0] \neq \emptyset, [1] \neq \emptyset, [2] \neq \emptyset`$</br>
  $`\quad [0]\cap[1] = [1]\cap[2] = [2]\cap[0] = \emptyset`$</br>
  $`\quad [0]\cup[1]\cup[2]=\mathbb{Z}`$</br>
  $`F = \{\; [0], [1], [2] \; \}`$: partition of $`\mathbb{Z}`$

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

  </details>

<details><summary>Given f: A $\rightarrow$ B a function, let A₁ ⊆ A, B₁ ⊆ B, show that ...</summary>

  - <details><summary>$f(f^{-1}(B_1)) \subseteq B_1$</summary>

    $`\begin{flalign}
    \text{Proof.} &&\\
    \text{Let } b \in f(f^{-1}(B_1)). &&\\
    \Leftrightarrow \exists a \in f^{-1}(B_1)(b = f(a)) &&\\
    \Leftrightarrow \exists a (a \in f^{-1}(B_1) \land b = f(a)) &&\\
    \text{Since } a \in f^{-1}B_1, f(a) \in B_1. &&\\
    \Rightarrow b \in B_1
    \end{flalign}`$

    </details>

  - <details><summary>$f^{-1}(f(A_1)) \supseteq A_1$</summary>

    $`\begin{flalign}
    \text{Proof.} &&\\
    \text{Recall that } &&\\
    \quad f^{-1}(B_1)    := \{ a \in A | f(a) \in B_1 \}, &&\\
    \quad f(A_1)         := \{ f(a) \in B | a \in A_1 \}, &&\\
    \quad f(f^{-1}(B_1)) := \{ f(a) \in B | a \in f^{-1}(B_1) \}, &&\\
    \quad f^{-1}(f(A_1)) := \{ a \in A | f(a) \in f(A_1) \}. &&\\
    \text{Let } a \in A_1. &&\\
    \Rightarrow f(a) \in f(A_1) &&\\
    \Rightarrow a \in f^{−1}(f(A_1)) \text{ (by the definition of the preimage)} &&\\
    \end{flalign}`$

    </details>

  - <details><summary>$f(f^{-1}(B_1)) \nsupseteq B_1$</summary>

    $`\begin{flalign}
    \text{Proof.} &&\\
    \text{Suppose that } b \in B_1, \text{but } b \notin f(A). &&\\
    \text{Then, } b \notin f(f^{-1}(B_1)) \text{ since there is no element in } f^{-1}(B_1) \text{ such that } f(a) = b. &&\\
    \end{flalign}`$

    </details>

  - <details><summary>$f^{-1}(f(A_1)) \nsubseteq A_1$</summary>

    $`\begin{flalign}
    \text{Proof.} &&\\
    \text{Suppose that } a \in A_1^{\complement}, a \in A, f(a) \in f(A_1). &&\\
    \text{Then, } a \in f^{-1}(f(A_1)), \text{but } a \notin A_1. &&\\
    \end{flalign}`$

    </details>

</details>

<details><summary>Given two sets A, B($\subset$ X) and functions f: A $\rightarrow$ B, $id_A$: A $\rightarrow$ A(a $\mapsto$ a), $id_B$: B $\rightarrow$ B(b $\mapsto$ b). Show that ...</summary>

  - <details><summary>f is one to one if and only if there exists g: B $\rightarrow$ A such that g $\circ$ f = $id_A$.</summary>

    $`\begin{flalign}
    \text{Proof.} &&\\
    (\Rightarrow) &&\\
    \text{Pick any } p \in A. &&\\
    \text{Define } g(=g_p): B \rightarrow A, \begin{cases}
      b \mapsto a \text{ if }b \in img(f)(\Leftrightarrow \text{there exists unique } a \in A \text{ such that } b = f(a)) \\
      b \mapsto p \text{ if } b \notin img(f) \\
    \end{cases} &&\\
    \text{Then g is well-defined.} &&\\
    &&\\
    (\Leftarrow) &&\\
    \text{Assume that there exists } g: B \rightarrow A \text{ s.t. } g \circ f = id_A. &&\\
    \text{Suppose that } f(a_1) = f(a_2) \text{ for any } a_1, a_2 \in A. \text{ Then, } g(f(a_1)) = g(f(a_2)) \text{ (by def. of function)}. &&\\
    \text{Therefore } a_1 = a_2 \text{ (by assumption } g \circ f = id_A). &&\\
    \end{flalign}`$

    </details>

  - <details><summary>f is onto if and only if there exists g: B $\rightarrow$ A such that f $\circ$ g = $id_B$.</summary>
  
    </details>

</details>

<details><summary>Given a set A, consider F = P(A) = { subsets of A }. Define R := { (x, y) $\in$ F x F | there exists a one to one, onto function f: X → Y }. Show that R is an equivalence relation.</summary>

  - Reflexive
    - $`\text{For each } x \in F, \text{we have } id_{X}: X \rightarrow X.`$
  
  - Symmetric
    - Suppose $`X`$~$`_{R}Y`$, i.e., there exists a one to one, onto function f: X $\rightarrow$ Y. Then there also exist g: Y $\rightarrow$ X s.t. g $\circ$ f = $`id_{X}`$ and f $\circ$ g = $`id_{Y}`$.
    - Given f: A $\rightarrow$ B and g: B $\rightarrow$ C,
      - If g $\circ$ f: A $\rightarrow$ C is onto, then g is onto.</br>
        Proof.</br>
        $`\forall z \in C \exists x \in A(g(f(x)) = z)`$</br>
        $`\Rightarrow \forall z \in C \exists y = f(x) \in B(g(y) = z)`$
      - If g $\circ$ f: A $\rightarrow$ C is one to one, then f is one to one.</br>
        Proof.</br>
        Suppose $`f(x_{1}) = f(x_{2})`$. Since g is a function, $`g(f(x_{1})) = g(f(x_{2}))`$. Hence, $`x_{1} = x_{2}`$($\because$ g $\circ$ f is injective).
      - Therefore g must be one to one, onto. In fact, $`g = f^{-1}`$(Inverse function). Hence, $`Y`$~$`_{R}X`$
  
  - Transitive
    - Suppose $`X`$~$`_{R}Y`$, $`Y`$~$`_{R}Z`$, i.e., there exist bijective f: X $\rightarrow$ Y and bijective g: Y $\rightarrow$ Z. Consider g $\circ$ f: X $\rightarrow$ Y $\rightarrow$ Z.
      - If f: X $\rightarrow$ Y and g: Y $\rightarrow$ Z are injective, then g $\circ$ f: X $\rightarrow$ Z is injective.</br>
        Proof.</br>
        Suppose $`g(f(x_{1})) = g(f(x_{2}))`$. Since g is injective, $`f(x_{1}) = f(x_{2})`$. Since f is also injective, $`x_{1} = x_{2}`$.
      - If f: X $\rightarrow$ Y and g: Y $\rightarrow$ Z are surjective, then g $\circ$ f: X $\rightarrow$ Z is surjective.</br>
        Proof.</br>
        $`\forall y \in Y \exists x \in X(f(x) = y)`$ and $`\forall z \in Z \exists y \in Y(g(y) = z)`$</br>
        $`\Rightarrow \forall z \in Z \exists x \in X(g(f(x)) = z)`$
      - Therefore g $\circ$ f: X $\rightarrow$ Z is bijective. Hence, $`X`$~$`_{R}Z`$

</details>

<details><summary>Given a set X, ...</summary>

  - <details><summary>consider the equivalence relation $R \subset X \text{ x } X$. For each x $\in X$, define $[x] = \{ y \in X | x R y \}$: the equivalence class of x. Show that $F = \{ [x] | x \in X \}$ becomes a partition of X.</summary>
    
    $`\begin{flalign}
    \text{Proof.} &&\\
    \text{NTS 1. Equivalence class is not empty set.} &&\\
    \text{Lemma 1. } \forall x \in X, x \in [x].
    \text{Proof of lemma 1.} &&\\
    \text{Let } x \in X. \text{Then } x \in [x] by reflexivity. &&\\
    &&\\
    \text{NTS 2. Equivalence classes are disjoint.} &&\\
    \text{Lemma 2. }x R y \Leftrightarrow [x] = [y] &&\\
    \text{Proof of lemma 2.} &&\\
    (\Rightarrow)\text{ Let } x R y. \text{We NTS that } [x] = [y]. &&\\
    (\subseteq) \text{ Let } \alpha \in [x], i.e., x R \alpha \Rightarrow y R \alpha \text{(by transitivity)} \Rightarrow \alpha \in [y]. &&\\
    (\supseteq) \text{ Let } \beta \in [y], i.e., y R \beta \Rightarrow x R \beta \text{(by transitivity)} \Rightarrow \beta \in [x]. &&\\
    (\Leftarrow)\text{ Let } [x] = [y]. \text{ Then, } x \in X \Rightarrow x \in [x] = [y] \Rightarrow x \in [y] \Rightarrow x R y. &&\\
    \text{Lemma 3. }\neg(x R y) \Leftrightarrow [x] \cap [y] = \emptyset &&\\
    \text{Proof of lemma 3.} &&\\
    (\Rightarrow)\text{ Let } \neg(x R y). \text{ Suppose that } [x] \cap [y] \neq \emptyset \text{ then } \exists \gamma \in X \text{ s.t. } \gamma \in [x] \cap [y]. \text{ Then, } \gamma \in [x] \cap [y] \Rightarrow \gamma \in [x] \land \gamma \in [y] \Rightarrow x R \gamma \land \gamma R y \Rightarrow x R y. (↯) &&\\
    (\Leftarrow)\text{ Let } [x] \cap [y] = \emptyset. \text{ Suppose that } x R y. \text{ By lemma 1, 2, we have } x \in [x] = [y]. (↯) &&\\
    \text{By lemma 2,3 it's proved.} &&\\
    &&\\
    \text{NTS 3. Union of equivalence classes is whole set.} &&\\
    \text{We NTS that } \bigcup \{ [x]_{R} | x \in X \} = X. &&\\
    (\subseteq) \text{ Since, } [x]_{R} \subseteq X, \bigcup \{ [x]_{R} | x \in X \} = \bigcup{\substack{x \in X}} [x]_{R} \subseteq X. &&\\
    (\supseteq) \text{ Let } \alpha \in X. \text{ We want to show that } \alpha \in \bigcup{\substack{x \in X}} [x]_{R}, \text{ i.e.}, \exists x \in X \text{ s.t. } \alpha \in [x]. \text{ By lemma 1, we obtain } \alpha \in [\alpha]. &&\\
    \text{ Thus, for every } \alpha \in X, \alpha \in \bigcup{\substack{x \in X}} [x]_{R}. &&\\
    \end{flalign}`$

    </details>

  - <details><summary>consider a partition $F = \{ E_{\alpha} | \alpha \in I \}$ of X. Define xRy, x,y $\in$ X, if there exists $\alpha \in I$ s.t. x,y $\in E_{\alpha}$. Show that R is an equivalence relation.</summary>
    
    $`\begin{flalign}
    \text{Proof.} &&\\
    \text{NTS 1. Reflexivity} &&\\
    \text{Let } x, y \in E_{1}, \text{ i.e., } x R y. \text{ Since } x \in E_{1}, x R x. &&\\
    \text{NTS 2. Symmetry} &&\\
    \text{Let } x, y \in E_{1}, \text{ i.e., } x R y. \text{ Since } y \in E_{1} \text{ and } x \in E_{1}, y R x. &&\\
    \text{NTS 3. Transitivity} &&\\
    \text{Let } x, y \in E_{i}, \text{ i.e., } x R y \text{ and } y, z \in E_{j}, \text{ i.e., } y R z. &&\\
    \text{Since } E_{i} \cap E_{j} = \emptyset, \text{ then } i = j. \text{ Therefore, } x R z. &&\\
    \end{flalign}`$

    </details>

  - Consequently, there is the one to one correspondence between equivalence relation on X and partition on X.

</details>

## TODO

<details><summary>Given f: A $\rightarrow$ B a function, show that A $\subseteq$ B $\Rightarrow$ f(A) $\subseteq$ f(B).</summary>

</details>

### References

- Patrick Keef, David Guichard, *An Introduction to Higher Mathematics*
- James Munkres, *Topology*
- [수학의 즐거움, Enjoying Math, "수학 공부, 기초부터 대학원 수학까지, 1. 집합론 기초 (a)"](https://youtu.be/9HUk8zays2E?feature=shared)
- [수학의 즐거움, Enjoying Math, "수학 공부, 기초부터 대학원 수학까지, 2. 집합론 기초 (b)"](https://youtu.be/k53Sr9Q9NR8?feature=shared)
- [수학의 즐거움, Enjoying Math, "수학 공부, 기초부터 대학원 수학까지, 3. 집합론 기초 (c)"](https://youtu.be/2gM-Vh8CY8I?feature=shared)
- [수학의 즐거움, Enjoying Math, "\[기초부터 대학원 수학까지 시리즈 스터디 3기\] 2. 집합론 기초 2강"](https://youtu.be/PPYhmRwbEno?feature=shared)
- [수학의 즐거움, Enjoying Math, "\[기초부터 대학원 수학까지 시리즈 스터디 3기\] 3. 집합론 기초: 단사, 전사 및 역함수와 합성함수"](https://youtu.be/YJWaI8RW_zE?feature=shared)
- [수학의 즐거움, Enjoying Math, "\[기초부터 대학원 수학까지 시리즈 스터디 3기\] 4. 집합론 기초: 관계와 분할"](https://youtu.be/qfCuWL6cg_c?feature=shared)
- [Hacker-Code-J, GitHub repository](https://github.com/Hacker-Code-J/Modern-Mathematics/blob/main/grad-math-mini/grad-math-mini-1.pdf)

[^equivalence_relation_0]: It's also equivalence relation if we remove (1, 2), (2, 1), i.e. symmetric is optional.

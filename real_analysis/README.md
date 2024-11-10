## Definitions

<details><summary>Bounded</summary>

  - Let $E \subseteq \mathbb{R}$. We say $E$ is bounded above(below) if there exists $\beta(\alpha) \in \mathbb{R}$ s.t. for each $x \in E, x \leq \beta(x \geq \alpha)$. In this case, $\beta(\alpha)$ is called an upper(lower) bound.
  
  - $E$ is bounded if $E$ is both bounded above and below.

  - Remark.
    1. $E = \emptyset$ is possible.
    2. $\beta, \alpha$ are not unique.
       - $\beta, \beta + 1, \beta + 2, \dots$
       - $\alpha, \alpha - 1, \alpha - 2, \dots$
       - ex. $`A = \{ 1 - \frac{1}{n} | n \in \mathbb{N} \} `$
       - ex. $\mathbb{N}$ has a lower bound, but doesn't have an upper bound.
       - ex. $`B = \{ r \in \mathbb{Q} | r > 0 \text{ and } r^2 < 2 \}`$. Then $B$ has a lower bound($\alpha = 0$). However, $B$ doesn't have the maximum element. \
         To show it, it is enough to show that if $p \in B$, then there exists $q \in B$ s.t. $p < q$.
         Take any $p \in B(\Leftrightarrow p > 0, p^2 < 2, p \in \mathbb{Q})$. \
         Take $q = p + \frac{2 - p^2}{p + 2}$. Since $\mathbb{Q}$ is field, then $q \in \mathbb{Q}$. \
         $2 - q = (\dots) = \frac{-2p^2 + 4}{(p+2)^2} > 0$ \
         $\therefore q \in B< 2$

</details>

<details><summary>Least upper bound property(=Completeness axiom)</summary>

  - Let $\emptyset \neq E \subseteq \mathbb{R}$ be bounded above. We say $\beta \in \mathbb{R}$ is the least upper bound of $E$ if:
    1. $\beta$ is an upper bound of $E$.
    2. If $\alpha < \beta$, then $\alpha$ is not an upper bound of $E$.
    
    We denote $\beta = supE$, called the supremum of $E$.

    ![image](images/supremum_illustration.jpg)

  - Remark.
    1. If $supE$ exists, then $supE$ must be unique. \
       $\because$ Let $\alpha, \beta$ be supremum of $E$. Then either:
       - $\alpha < \beta$(↯, by def. of least upper bound)
       - $\alpha = \beta$
       - $\alpha > \beta$(↯, by def. of least upper bound).
    2. Suppose $\emptyset \neq E \subseteq \mathbb{R}$ is not bounded above, i.e., ~(there exists $\beta$ s.t. for each $x \in E, x \leq \beta$). \
       $\Leftrightarrow$ For all $\beta \in \mathbb{R}$ there exists $x_{\beta} \in E \text{ s.t. } x_{\beta} > \beta$.<a name="remark_second_item"></a>
    3. Let $\emptyset \neq E \subseteq \mathbb{R}$ be not bounded above. \
       $\Rightarrow supE = \infty(\notin \mathbb{R})$
    4. $sup\emptyset = -\infty$
    5. Let $\emptyset \neq E \subseteq \mathbb{R}$ be bounded above. \
       $\Rightarrow$ There exists $supE = \beta \in \mathbb{R}$. (by def.) \
       Then for each $\epsilon > 0, \beta - \epsilon$ is not an upper bound. Thus by [ii.](#remark_second_item), there exists $x_{\epsilon} \in E$ s.t. $\beta - \epsilon < x_{\epsilon}$.<a name="#remark_fifth_item"></a> \
       Consequently, for each $\epsilon > 0$, there exists $x_{\epsilon} \in E$ s.t. $\beta - \epsilon < x_{\epsilon} \leq \beta$. \
       This is equivalent statement to say $\beta = supE$.
    6. For each $n \in \mathbb{N}(\epsilon = \frac{1}{n} > 0)$, by [v.](#remark_fifth_item), there exists $x_{n} \in E$ s.t. $\beta - \frac{1}{n} < x_{n} \leq \beta$.<a name="#remark_sixth_item"></a> \
       In particular, this shows that we can find a sequence ($x_{n}$) s.t. $\lim_{n\to\infty} x_{n} = \beta$. \
       In fact, [vi.](#remark_sixth_item) is equivalent to [v.](#remark_fifth_item). This is called Archimedean property.

</details>

<details><summary>Mathematical induction, Well-ordering principle</summary>

  - Mathematical induction \
    Let $A \subseteq \mathbb{N}$. If \
    $\quad$ ① $1 \in A$, \
    $\quad$ ② If $n \in A, \text{ then } n + 1 \in A$, \
    then $A = \mathbb{N}$.

  - Well-ordering principle \
    Let $A \subseteq \mathbb{N}, A \neq \emptyset$. Then there exists minimum of $A$.

</details>

## Exercises

<details><summary>Let $A = \{ 1 - \frac{1}{n} | n \in \mathbb{N} \}$. Show that $A$ has an upper bound and a lower bound.</summary>

  Proof. \
  For all $n \in \mathbb{N}, 1 - \frac{1}{n} = \frac{n-1}{n} < 1 = \frac{n}{n}$. \
  $\Rightarrow$ 1 is an upper bound of A. \
  For all $n \in \mathbb{N}, 1 - \frac{1}{n} \geq 0.$ \
  $\Rightarrow$ 0 is an lower bound of A.


</details>

### References

- [수학의 즐거움, Enjoying Math, "수학 공부, 기초부터 대학원 수학까지, 4. 해석학 개론 (a) 완비성 공리"](https://youtu.be/pHIImTBdBRs?feature=shared)

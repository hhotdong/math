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

  - $`\text{Mathematical induction}_{M.I.}`$ \
    Let $A \subseteq \mathbb{N}$. If \
    $\quad$ ① $1 \in A$, \
    $\quad$ ② If $n \in A, \text{ then } n + 1 \in A$, \
    then $A = \mathbb{N}$.

  - $`\text{Well-ordering principle}_{W.O.}`$ \
    Let $A \subseteq \mathbb{N}, A \neq \emptyset$. Then there exists minimum of $A$.

  - $Proposition.$ $M.I.$ and $W.O.$ are equivalent. \
    $Proof.$ \
    ($W.O. \Rightarrow M.I.$) \
    Suppose $M.I.$ is false, i.e., let $`A \subseteq \mathbb{N} \text{ satisfying ①, ②, but } A \neq \mathbb{N}(*)`$. \
    By $`(*), \mathbb{N} - A \neq \emptyset(\mathbb{N} - A \text{ is proper subset of } \mathbb{N})`$. \
    Apply $W.O.$ Then there exists the minimum $m_0 \in \mathbb{N} - A$. \
    But, $1 \in A, 2 \in A, \dots , m_0 \in A$. (↯, $m_0 \in \mathbb{N} - A$) \
    Thus $A = \mathbb{N}$. \
    <br/>
    ($M.I. \Rightarrow W.O.$) \
    Let $A$ be non-empty subset of $\mathbb{N}$. \
    Suppose $W.O.$ is false for $A$. \
    i.e., there is no minimum of $A$. \
    Define $`B := \{ k \in \mathbb{N} | k \leq n \text{ for any } n \in A \}`$. \
    Since $`1 \notin A(\because \; 1 \text{ is minimum}), 1 \in B(\Rightarrow B \neq \emptyset).`$ \
    Let $m \in B$, then $m \notin A$. \
    Thus $`m + 1 \in B(\because\; \text{For any } n \in A, m < n, m + 1 \leq n)`$. \
    $\Rightarrow B = \mathbb{N}$ (by $M.I.$)\
    $\Rightarrow A = \emptyset$ (↯)

</details>

<details><summary>Archimedean property</summary>

  - Let $x, y \in \mathbb{R}$ with $x > 0$. Then there exists $n \in \mathbb{N}$ s.t. $nx > y$. \
    $Proof.$ \
    If $y \leq 0$, take $n = 1.(1 \times x > y).$ So suppose $y > 0$. \
    $Claim$: there exists $`n \in \mathbb{N} \;\:s.t.\;\: nx > y`$. \
    Suppose not, i.e., for each $n \in \mathbb{N}, nx \leq y$. \
    Define $`E :=  \{ nx | n \in \mathbb{N} \},`$ \
    Then $\emptyset \neq E \subseteq \mathbb{R}$, $E$ is bounded above by $y$. \
    Thus there exists $supE = \beta \in \mathbb{R}$. \
    Since $x > 0, \text{ then } \beta - x < \beta.$ \
    $\Rightarrow \beta - x$ is not an upper bound. \
    So there exists $`n \in \mathbb{N} \;\:s.t.\;\: \beta - x < nx \in E \leq \beta`$. \
    $\Rightarrow \beta < (n + 1)x, n + 1 \in \mathbb{N}$ \
    $\Rightarrow (n + 1)x \in E$ (↯, $\beta$ is an upper bound)
  
  - Remark.
    1. Take $x = \epsilon > 0, y = 1$.<a name="#ap_remark_first_item"></a> \
       Then by this property, there exists $`n \in \mathbb{N} \;\:s.t.\;\: n - \epsilon > 1(\Leftrightarrow \frac{1}{n} < \epsilon)`$.
    2. Let $\emptyset \neq E \subseteq \mathbb{R}$ be a non-empty, bounded above. \
       $\Rightarrow$ There exists $supE = \beta \in \mathbb{R}$. \
       $\Leftrightarrow$ For each $\epsilon > 0$, there exists $`x_{\epsilon} \in E \;\:s.t.\;\: \beta - \epsilon < x_{\epsilon} \leq \beta`$. \
       $\Leftrightarrow$ For each $n \in \mathbb{N}(\epsilon = \frac{1}{n})$, there exists $`x_n \in E \;\:s.t.\;\: \beta - \frac{1}{n} < x_n \leq \beta`$. $\dots$ (\*\*) \
       In fact , ($\Leftarrow$) holds as well. \
       Suppose (\*\*) holds, \
       Let $\epsilon > 0$ be fixed. Then by $A.P.$, there exists $`n \in \mathbb{}N \;\:s.t.\;\: \frac{1}{n} < \epsilon`$. (by [i.](#ap_remark_first_item)) \
       $\Leftrightarrow -\frac{1}{n} > -\epsilon \Leftrightarrow \beta - \frac{1}{n} > \beta - \epsilon$ \
       Thus for each $\epsilon > 0$, there exists $`n \in \mathbb{N} \;s.t.`$ for corresponding $x_n \in E$ satisfying \
       $\beta - \epsilon < \beta - \frac{1}{n} < x_n \leq \beta$. \
       Consequently, we have a sequence $`(x_n)_{n=1}^{\infty} \text{ s.t. } \lim_{n\to\infty} x_{n} = \beta`$. \
       \
       Note. 위의 논지(argument)는 $\beta$를 handling하는데 있어서 $\beta$로 수렴하는 수열로 다룰 수 있고, uncountable한 $\epsilon > 0$의 선택지를 countable한 $n$으로 다룰 수 있음을 시사한다.
   
   - Density of $\mathbb{Q}$(유리수의 조밀성) \
     For any $x, y \in \mathbb{R}$ with $x < y$, there exists $`r \in \mathbb{Q} \;\:s.t.\;\: x < r < y`$. \
     $Proof.$ \
     There are 3 cases for $x < y$. \
     ①$`x < 0 < y`$ \
     ②$`0 < x < y`$ \
     ③$`x < y < 0`$ \
     It suffices to show ②. \
     With 1, there exists $`n \in \mathbb{N} \;\:s.t.\;\: n(y - x) > 1`$ by $A.P.$($\Leftrightarrow nx + 1 < ny$) \
     $`Purpose.\; x < \frac{m}{n} < y`$ \
     Define $`A := \{ k \in \mathbb{N} | nx < k \} \neq \emptyset`$ \
     $`\Rightarrow \emptyset \neq A \subseteq \mathbb{N}`$. \
     By $W.O.$, there exists the smallest element $m_0 \in A$, i.e., $nx < m_0$ but $nx \geq m_0 - 1$. \
     So, $m_0 - 1 \leq nx < m_0$ \
     $\Rightarrow nx < m_0 \leq nx + 1 < ny$ \
     $\Rightarrow nx < m_0 < ny$ \
     $\Leftrightarrow x < \frac{m_0}{n} < y$. \
     $Remark.$ $m_0$ was coming from $W.O.$ and $n$ was coming from $sup$.

</details>

<details><summary>Convergence of sequences</summary>

  - We say $`\{ a_{n} \}_{n = 1}^{\infty}(\subseteq X, \text{X is topological space})`$ is a sequence if it is a function $`\{ a_{n} \}_{n = 1}^{\infty}: \mathbb{N} \rightarrow X(n \mapsto a_{n})`$. In advanced calculus, $`X = \mathbb{R}`$.
  
  - We say a sequence $`\{ a_{n} \}_{n = 1}^{\infty}(\subseteq \mathbb{R})`$ converges to $`\alpha \in \mathbb{R}`$ if for each $`\epsilon > 0`$, there exists $`N_{\epsilon} \in \mathbb{N} \;s.t.\;`$ for any $`n \geq N_{\epsilon}, n \in \mathbb{N}, |a_{n} - \alpha| < \epsilon`$. We denote $`\lim_{x\to\infty}a_{n} = \alpha`$. Otherwise, we say $`\{ a_{n} \}`$ diverges.

    Remark.
    - Step ⓪: For each $`\epsilon > 0`$($`\epsilon`$ is fixed)
    - Step ①: there exists corresponding $`N_{\epsilon} \in \mathbb{N}`$,
    - Step ②: for any $`n \geq N_{\epsilon}, n \in \mathbb{N}`$($n$ is fixed but arbitrary),
    - Step ③: $`|a_{n} - \alpha| < \epsilon`$.
  
  - ex. $`a_{n} = \frac{1}{n},`$ for each $`n \in \mathbb{N}`$. \
    Claim: $`\lim{n\to\infty}\frac{1}{n} = 0`$ \
    By Archimedean property, there exists $`N_{\epsilon} \in \mathbb{N} \;s.t.\; N_{\epsilon} \times \epsilon > 1 \Leftrightarrow \frac{1}{N_{\epsilon}} < \epsilon`$. \
    Then for any $`n \geq N_{\epsilon} \Leftrightarrow \frac{1}{n} \leq \frac{1}{N_{\epsilon}},`$ \
    $`|a_{n} - \alpha| = |\frac{1}{n} - 0| = \frac{1}{n} \leq \frac{1}{N_{\epsilon}} < \epsilon, \;i.e.\; |a_{n} - \alpha| < \epsilon`$. \
    Hence, $`\lim{n\to\infty}a_{n} = 0`$.

  - (counter example) $`b_{n} = 1-(-1)^{n}`$ for each $n$. \
    Prove: $`b_{n}`$ diverges. \
    Observe that $`|b_{m} - b_{m+1}| = 2 > 0`$ for any $`m \in \mathbb{N}`$. \
    Choose $`\epsilon > 0`$ satisfying $`\epsilon < 2`$. \
    If $`\{ b_{n} \}`$ converges to some $`\beta \in \mathbb{R}`$. \
    $`|b_{n} - \beta| = | b_{n} - b_{n+1} + b_{n+1} - \beta |`$ \
    $`\leq | b_{n} - b_{n+1} | + | b_{n+1} - \beta | = k`$ (by triangle inequality) \
    Then $`k \geq 2, \;i.e.\; k`$ cannot be smaller than $\epsilon$ for any $`n \in \mathbb{N}`$. \
    Thus there is no $`N_{\epsilon} \in \mathbb{N}`$ satisfying for any $`n \geq N_{\epsilon}, |b_n - \beta| < \epsilon`$. \
    Note that '≤' is used while applying triangle inequality in the proof above.

  - Remark. Property of the absolute value \
    $`|x| = x(\text{if } x \leq 0) \text{ or } -x(\text{if} x < 0)`$
    1. $`|x| = |-x| = \sqrt{x^2}`$
    2. $`|xy| = |x| \times |y|`$
    3. For each $`r > 0, |x| < r \Leftrightarrow -r < x < r`$
    4. $`-|x| \leq x \leq |x|`$
    5. $`|x+y| \leq |x| + |y|`$
      - $\because$ $`-|x| \leq x  \leq |x|, -|y| \leq y  \leq |y|`$ \
        $`\Leftrightarrow -(|x| + |y|) \leq x + y \leq |x| + |y|`$ (by iv.) \
        $`\Leftrightarrow |x + y| \leq |x| + |y|`$ (by iii.)
    6. $`|x| > d \Leftrightarrow x > d \lor x < -d`$

</details>

<details><summary>Boundedness</summary>

  - A sequence $`\{ a_{n} \}_{n = 1}^{\infty} \;in\; \mathbb{R}`$ is bounded if there exists $`M > 0 \;s.t.\;`$ for any $`n \in \mathbb{N}, |a_{n}| \leq M`$.

  - Remark.
    - (Wrong) A sequence $`\{ a_{n} \}_{n = 1}^{\infty} \;in\; \mathbb{R}`$ is bounded if for any $`n \in \mathbb{N}`$ there exists $`M > 0 \;s.t.\; |a_{n}| \leq M`$.
    - Boundedness is not a topological property.
  
  - Proposition. If $`\{ a_{n} \}_{n = 1}^{\infty} \;in\; \mathbb{R}`$ is convergent, then $`\{ a_{n} \}_{n = 1}^{\infty}`$ is bounded. \
    Proof. Let $`\alpha = \lim{n\to\infty}a_{n} \in \mathbb{R}`$. \
    Take $`\epsilon = 1`$. \
    Then there exists $`N_{1} \in \mathbb{N} \;s.t.\;`$ for any $`n \geq N_{1}, n \in \mathbb{N}, |a_{n} - \alpha| < \epsilon = 1`$. \
    $`\Leftrightarrow -1 < a_{n} - \alpha < 1`$ \
    $`\Leftrightarrow \alpha - 1 < a_{n} < \alpha + 1`$ \
    We can choose $`M = max\{ |\alpha + 1|, |a_1|, \dots, |a_{N_1 - 1}| \}`$. \
    Then for any $`n \in \mathbb{N}, |a_{n}| \leq M`$. \
    Q. What about the converse? i.e. if $`\{ a_{n} \}_{n = 1}^{\infty} \in \mathbb{R}`$ is bounded then is it convergent? \
    In general, no(counter-example. $`b_{n} = 1 - (-1)^{n}`$) \
    However, we can say something on this, since it is "partially" true.

</details>

<details><summary>Limit theorem</summary>

Let $`\lim{n\to\infty}a_{n} = \alpha, \lim{n\to\infty}b_{n} = \beta, \alpha, \beta \in \mathbb{R}`$. Then the followings hold: \
    $`\;\;\;\text{(a)}\lim{n\to\infty}(a_{n} + b_{n}) = \alpha + \beta`$ \
    $`\;\;\;\text{(b)}\lim{n\to\infty}(ka_{n}) = k\alpha \text{ for any } k \in \mathbb{R}`$ \
    $`\;\;\;\text{(c)}\lim{n\to\infty}(a_{n} - b_{n}) = \alpha - \beta`$ \
    $`\;\;\;\text{(d)}\lim{n\to\infty}(a_{n} \times b_{n}) = \alpha \times \beta`$ \
    $`\;\;\;\text{(e)}\lim{n\to\infty}(\frac{a_{n}}{b_{n}}) = \frac{\alpha}{\beta}`$ provided $`b_{n}, \beta \neq 0`$ for any $`$n \in \mathbb{N}`$

</details>

## Exercises

<details><summary>Let $A = \{ 1 - \frac{1}{n} | n \in \mathbb{N} \}$. Show that $A$ has an upper bound and a lower bound.</summary>

  Proof. \
  For all $n \in \mathbb{N}, 1 - \frac{1}{n} = \frac{n-1}{n} < 1 = \frac{n}{n}$. \
  $\Rightarrow$ 1 is an upper bound of A. \
  For all $n \in \mathbb{N}, 1 - \frac{1}{n} \geq 0.$ \
  $\Rightarrow$ 0 is an lower bound of A.

</details>

<details><summary>Prove limit theorem.</summary>

  - <details><summary>Proof of (a).</summary>
    
    Let $`c_{n} = a_{n} + b_{n}`$. \
    NTS. $`\lim{n\to\infty}c_{n} = \alpha + \beta`$ \
    Let $`\epsilon > 0`$ be fixed. \
    By the assumption, $`\lim{n\to\infty}a_{n} = \alpha`$, $`\lim{n\to\infty}b_{n} = \beta \;,\;i.e.,`$
      - there exists $`N_{\epsilon} \in \mathbb{N} \;s.t.\; \text{ for any } n \geq N_{\epsilon} |a_{n} - \alpha| < \epsilon`$.
      - there exists $`N_{\epsilon}' \in \mathbb{N} \;s.t.\; \text{ for any } n \geq N_{\epsilon}' |b_{n} - \beta| < \epsilon`$. \
    The propositions above also hold for $`\frac{\epsilon}{2} \;,\;i.e.,`$
      - there exists $`N_{\epsilon} \in \mathbb{N} \;s.t.\; \text{ for any } n \geq N_{\epsilon} |a_{n} - \alpha| < \frac{\epsilon}{2}`$.
      - there exists $`N_{\epsilon}' \in \mathbb{N} \;s.t.\; \text{ for any } n \geq N_{\epsilon}' |b_{n} - \beta| < \frac{\epsilon}{2}`$. \
    Take $`N = max \{ N_{\epsilon}, N_{\epsilon}' \}`$. \
    Then $`|c_{n} - (\alpha + \beta)|`$ \
    $`= |(a_{n} - \alpha) + (b_{n} - \beta)|`$ \
    $`\leq |(a_{n} - \alpha)| + |(b_{n} - \beta)| `$ \
    $`< \frac{\epsilon}{2} + \frac{\epsilon}{2} = \epsilon`$. \
    Hence, for each $`\epsilon > 0`$, there exists $`N \in \mathbb{N} \;s.t.\; \text{ for any } n \geq \mathbb{N}, |C_{n} - (\alpha + \beta)| < \epsilon`$ \
    $`\Leftrightarrow \lim{n\to\infty}c_{n} = \lim{n\to\infty}(a_{n} + b_{n}) = \alpha + \beta`$.
  
    </details>
  
  - <details><summary>Proof of (d).</summary>
    
    Let $`c_{n} = a_{n}b_{n}`$. \
    NTS. $`\lim{n\to\infty}c_{n} = \alpha\beta`$ \
    Idea. $`|a_{n}b_{n} - \alpha\beta| = |(a_{n} - \alpha)b_{n} + \alpha b_{n} - \alpha\beta|`$ \
    $`= |(a_{n} - \alpha)b_{n} + \alpha(b_{n} - \beta)|`$ \
    $`\leq |a_{n} - \alpha| \times |b_{n}| + |\alpha| \times |b_{n} - \beta|`$ \
    $`\leq M \times |a_{n} - \alpha| + |\alpha| \times |b_{n} - \beta| < \epsilon`$ \
    Let $`\epsilon > 0`$ be fixed. \
    Since $`\lim{n\to\infty}b_{n} = \beta`$, there exists $`M > 0 \;s.t.\; |b_{n}| \leq M \text{ for any } n \in \mathbb{N}`$. (by boundedness) \
    Since $`\lim{n\to\infty}a_{n} = \alpha`$, $`\lim{n\to\infty}b_{n} = \beta`$, there exists $`N_{\epsilon}, N_{\epsilon}' \in \mathbb{N} \;s.t.\;`$ \
    $`\;\;\text{ for any } n \geq N_{\epsilon}, |a_{n} - \alpha| < \frac{\epsilon}{2M}`$ \
    $`\;\;\text{ for any } n \geq N_{\epsilon}', |b_{n} - \beta| < \frac{\epsilon}{2|\alpha|}`$. \
    Put $`N = max \{ N_{\epsilon}, N_{\epsilon}' \}`$ \
    Then for any $`n \geq N, |c_{n} - \alpha\beta| = |a_{n}b_{n} - \alpha\beta|`$ \
    $`\leq M \times |a_{n} - \alpha| + |\alpha| \times |b_{n} - \beta|`$. \
    $`< M \times \frac{\epsilon}{2M} + |\alpha| \times \frac{\epsilon}{2|\alpha|} = \epsilon`$ \
    Hence $`\forall \epsilon > 0, \exists N \in \mathbb{N} \;s.t.\; \forall n \geq N, |c_{n} - \alpha\beta| < \epsilon`$.
  
    </details>

  - <details><summary>Proof of (e).</summary>
    
    Let $`c_{n} = \frac{a_{n}}{b_{n}}`$. \
    NTS. $`|\frac{a_{n}}{b_{n}} - \frac{\alpha}{\beta}| < \epsilon`$ \
    Idea. $`|\frac{a_{n}}{b_{n}} - \frac{\alpha}{\beta}|`$ $`= |\frac{\beta a_{n} - \alpha b_{n}}{\beta b_{n}}| = \frac{1}{\beta b_{n}}|\beta(a_{n} - \alpha) - \alpha(b_{n} - \beta)| (*)`$ \
    From triangular inequality, $`|x + y| \leq |x| + |y|`$. \
    $`\Leftrightarrow |y| = |y - x + x| \leq |y - x| + |x|`$ \
    $`\Leftrightarrow |y| - |x| \leq |y - x|`$ \
    Let $`y = \beta, x = b_{n}`$. \
    $`\Rightarrow |\beta| - |b_{n}| \leq |b_{n} - \beta| < \epsilon`$ \
    Take $`\epsilon \text{ as } \frac{1}{2}|\beta|`$. \
    $`\Rightarrow |\beta| - |b_{n}| < \frac{1}{2}|\beta|`$ \
    $`\Leftrightarrow |b_{n}| > \frac{1}{2}|\beta|`$ \
    $`\Leftrightarrow \frac{1}{b_{n}} < \frac{2}{|\beta|}`$ \
    $`(*) \leq \frac{2}{|\beta|^2} \times |\beta(a_{n} - \alpha) - \alpha(b_{n} - \beta)|`$ \
    $`= \frac{2}{|\beta|^2} \times |\beta(a_{n} - \alpha) + \alpha(\beta - b_{n})|`$ \
    $`\leq \frac{2}{|\beta|^2}(|\beta(a_{n} - \alpha)| + |\alpha(\beta - b_{n})|) < \frac{\epsilon}{2} + \frac{\epsilon}{2} = \epsilon`$ \
    $`(\because |a_{n} - \alpha| < \frac{|\beta|^2}{2} \times \frac{\epsilon}{2} \times \frac{1}{|\beta|}, |\beta - b_{n}| < \frac{|\beta|^2}{2} \times \frac{\epsilon}{2} \times \frac{1}{|\alpha|})`$ \
    Now let us prove (e). \
    Fix $`\epsilon > 0`$. \
    NTS: $`\exists N \in \mathbb{N} \;s.t.\; \forall n \geq N, |\frac{a_{n}}{b_{n}} - \frac{\alpha}{\beta}| < \epsilon`$. \
    Take $`\epsilon_{1} = \frac{1}{2}|\beta| > 0`$. (By assumption, $`\beta \neq 0`$) \
    Since $`\lim{n\to\infty}b_{n} = \beta, \exists N_{1} \in \mathbb{N} \;s.t.\; \forall n \geq N_{1}, |b_{n} - \beta| < \epsilon_{1}`$. \
    $`\Rightarrow \forall n \geq N_{1}, |\beta| - |b_{n}| \leq |b_{n} - \beta| < \epsilon_{1} = \frac{1}{2}|\beta|`$. \
    $`\Leftrightarrow \forall n \geq N_{1}, |b_{n}| > \frac{1}{2}|\beta|`$ \
    $`\Leftrightarrow \forall n \geq N_{1}, \frac{1}{|b_{n}|} < \frac{2}{|\beta|}`$ \
    Next, take $`\epsilon_{2} = \frac{\epsilon}{2} \times \frac{1}{|\beta|} \times \frac{|\beta|^2}{2}, \epsilon_{3} = \frac{\epsilon}{2} \times \frac{1}{|\alpha|} \times \frac{|\beta|^2}{2}`$. \
    From the assumption $`\lim{n\to\infty}a_{n} = \alpha, \lim{n\to\infty}b_{n} = \beta`$, \
    $`\exists N_{2}, N_{3} \in \mathbb{N} \;s.t.\; \forall n \geq N_{2}, |a_{n} - \alpha| < \epsilon_{2}, \forall n \geq N_{3}, |b_{n} - \beta| < \epsilon_{3}`$. \
    Choose $`N = max \{ N_{1}, N_{2}, N_{3} \}`$ \
    Then $`\forall n \geq N,`$ \
    $`|\frac{a_{n}}{b_{n}} - \frac{\alpha}{\beta}| = |\frac{\beta a_{n} - \alpha b_{n}}{\beta b_{n}}| = |\frac{\beta(a_{n} - \alpha) + \alpha(\beta - b_{n})}{\beta b_{n}}|`$ \
    $`\leq \frac{2}{|\beta|^2}|\beta(a_{n} - \alpha) + \alpha(\beta - b_{n})|`$ \
    $`\frac{2}{|\beta|^2} \times (|\beta|\epsilon_{2} + |\alpha|\epsilon_{3})`$ \
    $`= \frac{\epsilon}{2} + \frac{\epsilon}{2} = \epsilon`$ \
    Thus, $`\lim{n\to\infty}\frac{a_{n}}{b_{n}} = \frac{\alpha}{\beta}`$.
  
    </details>

</details>

<details><summary>Suppose $\lim{n\to\infty}a_{n} = \alpha$ and $\lim{n\to\infty}b_{n} = \beta$. Show that $\alpha = \beta$.</summary>

</details>

### References

- [수학의 즐거움, Enjoying Math, "수학 공부, 기초부터 대학원 수학까지, 4. 해석학 개론 (a) 완비성 공리"](https://youtu.be/pHIImTBdBRs?feature=shared)
- [수학의 즐거움, Enjoying Math, "수학 공부, 기초부터 대학원 수학까지, 5. 해석학 개론 (b) 유리수의 조밀성와 실수, 자연수 공리"](https://youtu.be/RYjhQyXxTpQ?feature=shared)
- [수학의 즐거움, Enjoying Math, "수학 공부, 기초부터 대학원 수학까지, 6. 해석학 개론 (c) 수열의 수렴성"](https://youtu.be/jwLfzJyIxmU?feature=shared)

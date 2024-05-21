
## Math inside RMarkdown

In side a text chunk, you can use mathematical notation if you surround it by dollar signs `$` for “inline mathematics” and `$$` for “displayed equations”. **Do not leave a space between the `$` and your mathematical notation**.

Example: `$\sum_{n=1}^{10} n^2$` is rendered as ∑10n=1n2∑𝑛=110𝑛2.

Example: `$$\sum_{n=1}^{10} n^2$$` is rendered as

∑n=110n2∑𝑛=110𝑛2

.

The mathematical typesetting is based on LaTeX, so if you need to search for the way to make a particular symbol, include `latex` in your search. But note: Not all LaTeX macros are available without using additional packages, and those packages likely will only work if you are creating a PDF. On the plus side, if you are working in PDF, you can use additional packages that give much better control and/or easier syntax.

In LaTeX,

- macros begin with a backslash (`\`)
- curly braces (`{` and `}`) are used to surround items that are to be considered as one object from LaTeX’s perspective.  
    Without them, usually the next letter or digit will be used, but that isn’t usually what you want. For example `$$\sum_x=1^10 x^2$$` produces
    
    ∑x=110x2∑𝑥=110𝑥2
    

### Mathematical Notation

Here are some common mathematical things you might use in statistics

|                                                     |                                                                                                         |
| --------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| x=y𝑥=𝑦                                            | `$x = y $`                                                                                              |
| x<y𝑥<𝑦                                            | `$x < y $`                                                                                              |
| x>y𝑥>𝑦                                            | `$x > y $`                                                                                              |
| x≤y𝑥≤𝑦                                            | `$x \le y $`                                                                                            |
| x≥y𝑥≥𝑦                                            | `$x \ge y $`                                                                                            |
| xn𝑥𝑛                                              | `$x^{n}$`                                                                                               |
| xn𝑥𝑛                                              | `$x_{n}$`                                                                                               |
| x¯¯¯𝑥¯                                             | `$\overline{x}$`                                                                                        |
| x^𝑥^                                               | `$\hat{x}$`                                                                                             |
| x~𝑥~                                               | `$\tilde{x}$`                                                                                           |
| ab𝑎𝑏                                              | `$\frac{a}{b}$`                                                                                         |
| ∂f∂x∂𝑓∂𝑥                                          | `$\frac{\partial f}{\partial x}$`                                                                       |
| ∂f∂x∂𝑓∂𝑥                                          | `$\displaystyle \frac{\partial f}{\partial x}$`                                                         |
| (nk)(𝑛𝑘)                                          | `$\binom{n}{k}$`                                                                                        |
| x1+x2+⋯+xn𝑥1+𝑥2+⋯+𝑥𝑛                            | `$x_{1} + x_{2} + \cdots + x_{n}$`                                                                      |
| x1,x2,…,xn𝑥1,𝑥2,…,𝑥𝑛                            | `$x_{1}, x_{2}, \dots, x_{n}$`                                                                          |
| x=⟨x1,x2,…,xn⟩𝑥=⟨𝑥1,𝑥2,…,𝑥𝑛⟩                   | `\mathbf{x} = \langle x_{1}, x_{2}, \dots, x_{n}\rangle$` (`\bm` from the `bm` pacakge would be better) |
| x∈A𝑥∈𝐴                                            | `$x \in A$`                                                                                             |
| \|A\|𝐴\|                                           | `$\|A\|$`                                                                                               |
| x∈A𝑥∈𝐴                                            | `$x \in A$`                                                                                             |
| A⊂B𝐴⊂𝐵                                            | `$x \subset B$`                                                                                         |
| A⊆B𝐴⊆𝐵                                            | `$x \subseteq B$`                                                                                       |
| A∪B𝐴∪𝐵                                            | `$A \cup B$`                                                                                            |
| A∩B𝐴∩𝐵                                            | `$A \cap B$`                                                                                            |
| X∼Binom(n,π)𝑋∼𝐵𝑖𝑛𝑜𝑚(𝑛,𝜋)                    | `$X \sim {\sf Binom}(n, \pi)$` (`sf` for “slide font”)                                                  |
| P(X≤x)=pbinom(x,n,π)P(𝑋≤𝑥)=𝑝𝑏𝑖𝑛𝑜𝑚(𝑥,𝑛,𝜋) | `$\mathrm{P}(X \le x) = {\tt pbinom}(x, n, \pi)$` (`tt` for “typewriter type”)                          |
| P(A∣B)𝑃(𝐴∣𝐵)                                     | `$P(A \mid B)$`                                                                                         |
| P(A∣B)P(𝐴∣𝐵)                                      | `$\mathrm{P}(A \mid B)$` (`mathrm` for “math roman font”                                                |
| {1,2,3}{1,2,3}                                      | `$\{1, 2, 3\}$`                                                                                         |
| sin(x)sin⁡(𝑥)                                      | `$\sin(x)$`                                                                                             |
| log(x)log⁡(𝑥)                                      | `$\log(x)$`                                                                                             |
| ∫ba∫𝑎𝑏                                            | `$\int_{a}^{b}$`                                                                                        |
| (∫baf(x)dx)(∫𝑎𝑏𝑓(𝑥)𝑑𝑥)                        | `$\left(\int_{a}^{b} f(x) \; dx\right)$`                                                                |
| [∫∞−∞f(x)dx][∫−∞∞𝑓(𝑥)𝑑𝑥]                        | `$\left[\int_{\-infty}^{\infty} f(x) \; dx\right]$`                                                     |
| F(x)\|ba𝐹(𝑥)\|𝑎𝑏                                | `$\left. F(x) \right\|_{a}^{b}$`                                                                        |
| ∑bx=af(x)∑𝑥=𝑎𝑏𝑓(𝑥)                             | `$\sum_{x = a}^{b} f(x)$`                                                                               |
| ∏bx=af(x)∏𝑥=𝑎𝑏𝑓(𝑥)                             | `$\prod_{x = a}^{b} f(x)$`                                                                              |
| limx→∞f(x)lim𝑥→∞𝑓(𝑥)                             | `$\lim_{x \to \infty} f(x)$`                                                                            |
| limx→∞f(x)lim𝑥→∞𝑓(𝑥)                             | `$\displaystyle \lim_{x \to \infty} f(x)$`                                                              |

### Greek Letters

|   |   |   |   |
|---|---|---|---|
|αA𝛼𝐴|`$\alpha A$`|νN𝜈𝑁|`$\nu N$`|
|βB𝛽𝐵|`$\beta B$`|ξΞ𝜉Ξ|`$\xi\Xi$`|
|γΓ𝛾Γ|`$\gamma \Gamma$`|oO𝑜𝑂|`$o O$` (omicron)|
|δΔ𝛿Δ|`$\delta \Delta$`|πΠ𝜋Π|`$\pi \Pi$`|
|ϵεE𝜖𝜀𝐸|`$\epsilon \varepsilon E$`|ρϱP𝜌𝜚𝑃|`$\rho\varrho P$`|
|ζZ𝜁𝑍|`$\zeta Z \sigma \,\!$`|ΣΣ|`$\sigma \Sigma$`|
|ηH𝜂𝐻|`$\eta H$`|τT𝜏𝑇|`$\tau T$`|
|θϑΘ𝜃𝜗Θ|`$\theta \vartheta \Theta$`|υΥ𝜐Υ|`$\upsilon \Upsilon$`|
|ιI𝜄𝐼|`$\iota I$`|ϕφΦ𝜙𝜑Φ|`$\phi \varphi \Phi$`|
|κK𝜅𝐾|`$\kappa K$`|χX𝜒𝑋|`$\chi X$`|
|λΛ𝜆Λ|`$\lambda \Lambda$`|ψΨ𝜓Ψ|`$\psi \Psi$`|
|μM𝜇𝑀|`$\mu M$`|ωΩ𝜔Ω|`$\omega \Omega$`|

### Aligning equations

If you want a sequence of aligned equations (often very useful for demonstrating algebraic manipulation or for plugging values into equations), use `\begin{align*} ... \end{align*}`. Separate lines with `\\` and use `&` to mark where things should line up. Note: No dollar signs are needed when you use this method.

#### Example

This

```
\begin{align*}
a & = b \\
X &\sim {\sf Norm}(10, 3) \\
5 & \le 10
\end{align*}
```
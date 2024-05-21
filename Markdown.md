# <span class="h1">Mathématiques en Markdown</span>

> [!summary] 
> Dans un bloc de texte, vous pouvez utiliser la notation mathématique en l'entourant de signes dollar `$` pour les “mathématiques en ligne” et `$$` pour les “équations affichées”. <u>Ne laissez pas d'espace entre le `$` et votre notation mathématique.</u> 


Exemple : `$ \sum_{n=1}^{10} n^2 $` est rendu comme $\sum_{n=1}^{10} n^2$
Exemple : `$$ \sum_{n=1}^{10} n^2 $$` est rendu comme

$$
\sum_{n=1}^{10} n^2
$$

> [!info] 
> La composition mathématique est basée sur LaTeX, donc si vous devez rechercher comment faire un symbole particulier, incluez `latex` dans votre recherche. Mais notez : Toutes les macros LaTeX ne sont pas disponibles sans utiliser des packages supplémentaires, et ces packages ne fonctionneront probablement que si vous créez un PDF. En revanche, si vous travaillez dans un PDF, vous pouvez utiliser des packages supplémentaires qui offrent un meilleur contrôle et/ou une syntaxe plus facile. 

<u>En LaTeX :</u>

- Les macros commencent par une barre oblique inversée (`\`)
- Les accolades (`{` et `}`) sont utilisées pour entourer les éléments qui doivent être considérés comme un seul objet du point de vue de LaTeX. Sans elles, généralement, la lettre ou le chiffre suivant sera utilisé, mais ce n'est généralement pas ce que vous voulez. Par exemple, `$$ \sum_x=1^10 x^2 $$` produit

  $$\sum_x=1^10 x^2$$
  - Si vous voulez une séquence d'équations alignées (souvent très utile pour démontrer des manipulations algébriques ou pour insérer des valeurs dans des équations), utilisez `\begin{align*} ... \end{align*}`. Séparez les lignes avec `\\` et utilisez `&` pour marquer où les choses doivent s'aligner. Note : Pas besoin de signes dollar lorsque vous utilisez cette méthode.

$$
\begin{align*}
a & = b \\
X &\sim {\sf Norm}(10, 3) \\
5 & \le 10
\end{align*}$$






## <span class="h2">Notation Mathématique</span>

### <span class="h3">Opérateur</span>
 
| Symboles | code       |
| -------- | ---------- |
| $\cos$   | `$\cos$`   |
| $\sin$   | `$\sin$`   |
| $\lim$   | `$\lim$`   |
| $\exp$   | `$\exp$`   |
| $\to$    | `$\to$`    |
| $\infty$ | `$\infty$` |
| $\equiv$ | `$\equiv$` |
| $\bmod$  | `$\bmod$`  |
| $\times$ | `$\times$` |

### <span class="h3">Puissances et indices</span>

| Symboles  | code        |
| --------- | ----------- |
| $k_{n+1}$ | `$k_{n+1}$` |
| $n^2$     | `$n^2$`     |
| $k_n^2$   | `$k_n^2$`   |

### <span class="h3">Fractions et binômes</span>

| Symboles                    | code                          |
| --------------------------- | ----------------------------- |
| $\frac{n!}{k!(n-k)!}$       | `$\frac{n!}{k!(n-k)!}$`       |
| $\binom{n}{k}$              | `$\binom{n}{k}$`              |
| $\frac{\frac{x}{1}}{x - y}$ | `$\frac{\frac{x}{1}}{x - y}$` |
| $^3/_7$                     | `$^3/_7$`                     |


### <span class="h3">Racines</span>

| Symboles      | code            |
| ------------- | --------------- |
| $\sqrt{k}$    | `$\sqrt{k}$`    |
| $\sqrt[n]{k}$ | `$\sqrt[n]{k}$` |
### <span class="h3">Sommes et Intégrales</span>

| Symboles                                       | Code                                               |
| ---------------------------------------------- | -------------------------------------------------- |
| $\sum_{i=1}^{10} t_i$<br>$\sum\limits_{x}^{y}$ | `$\sum_{i=1}^{10} t_i$`<br>`$\sum\limits_{x}^{y}$` |
| $\int_0^\infty \mathrm{e}^{-x}\,\mathrm{d}x$   | `$\int_0^\infty \mathrm{e}^{-x}\,\mathrm{d}x$`     |
| $\sum$                                         | `$\sum$`                                           |
| $\prod$                                        | `$\prod$`                                          |
| $\coprod$                                      | `$\coprod$`                                        |
| $\bigoplus$                                    | `$\bigoplus$`                                      |
| $\bigotimes$                                   | `$\bigotimes$`                                     |
| $\bigodot$                                     | `$\bigodot$`                                       |
| $\bigcup$                                      | `$\bigcup$`                                        |
| $\bigcap$                                      | `$\bigcap$`                                        |
| $\biguplus$                                    | `$\biguplus$`                                      |
| $\bigsqcup$                                    | `$\bigsqcup$`                                      |
| $\bigvee$                                      | `$\bigvee$`                                        |
| $\bigwedge$                                    | `$\bigwedge$`                                      |
| $\int$                                         | `$\int$`                                           |
| $\oint$                                        | `$\oint$`                                          |
| $\iint$                                        | `$\iint$`                                          |
| $\iiint$                                       | `$\iiint$`                                         |
| $\idotsint$                                    | `$\idotsint$`                                      |
| $\sum_{\substack{0<i<m\\0<j<n}} P(i, j)$       | `$\sum_{\substack{0<i<m\\0<j<n}} P(i, j)$`         |
| $\int\limits_a^b$                              | `$\int\limits_a^b$`                                |


### <span class="h3">Parenthèses et Crochets</span>

| Symboles           | Code                    |
| ------------------ | ----------------------- |
| $(a)$              | `$(a)$`                 |
| $[a]$              | `$[a]$`                 |
| $\{a\}$            | `$\{a\}$`               |
| $\langle f \rangle$| `$\langle f \rangle$`   |
| $\lfloor f \rfloor$| `$\lfloor f \rfloor$`   |
| $\lceil f \rceil$  | `$\lceil f \rceil$`     |
| $\ulcorner f \urcorner$| `$\ulcorner f \urcorner$` |



### <span class="h3">Lettres Grecques</span>

| Résultat   | Formule      | Résultat          | Formule      |
| ---------- | ------------ | ----------------- | ------------ |
| $\alpha$   | `$\alpha$`   | $\nu$             | `$\nu$`      |
| $\beta$    | `$\beta$`    | $\xi$             | `$\xi$`      |
| $\gamma$   | `$\gamma$`   | $o$               | `$o$`        |
| $\delta$   | `$\delta$`   | $\pi$             | `$\pi$`      |
| $\epsilon$ | `$\epsilon$` | $\rho$            | `$\rho$`     |
| $\zeta$    | `$\zeta$`    | $\sigma$          | `$\sigma$`   |
| $\eta$     | `$\eta$`     | $\tau$            | `$\tau$`     |
| $\theta$   | `$\theta$`   | $\upsilon$        | `$\upsilon$` |
| $\iota$    | `$\iota`     | $\phi$            | `$\phi$`     |
| $\kappa$   | `$\kappa$`   | $\chi$            | `$\chi$`     |
| $\lambda$  | `$\lambda$`  | $\psi$            | `$\psi$`     |
| $\mu$      | `$\mu$`      | $\omega$ $\Omega$ | `$\omega$`   |
| $\nabla$   | `$\nabla$`   |                   |              |

### <span class="h3">Autres</span>

| Symboles               | Code                     |
| ---------------------- | ------------------------ |
| $a' a^{\prime}$        | `$a' a^{\prime}$`        |
| $a''$                  | `$a''$`                  |
| $\hat{a}$              | `$\hat{a}$`              |
| $\bar{a}$              | `$\bar{a}$`              |
| $\grave{a}$            | `$\grave{a}$`            |
| $\acute{a}$            | `$\acute{a}$`            |
| $\dot{a}$              | `$\dot{a}$`              |
| $\ddot{a}$             | `$\ddot{a}$`             |
| $\not{a}$              | `$\not{a}$`              |
| $\mathring{a}$         | `$\mathring{a}$`         |
| $\overrightarrow{AB}$  | `$\overrightarrow{AB}$`  |
| $\overleftarrow{AB}$   | `$\overleftarrow{AB}$`   |
| $a'''$                 | `$a'''$`                 |
| $\overline{aaa}$       | `$\overline{aaa}$`       |
| $\check{a}$            | `$\check{a}$`            |
| $\vec{a}$              | `$\vec{a}$`              |
| $\underline{a}$        | `$\underline{a}$`        |
| $\color{red}x$         | `$\color{red}x$`         |
| $\pm$                  | `$\pm$`                  |
| $\mp$                  | `$\mp$`                  |
| $\int y \mathrm{d}x$   | `$\int y \mathrm{d}x$`   |
| `\,`                   | `\,`                     |
| `\:`                   | `\:`                     |
| `\;`                   | `\;`                     |
| $\int y\, \mathrm{d}x$ | `$\int y\, \mathrm{d}x$` |
| $\dots$                | `$\dots$`                |
| $\ldots$               | `$\ldots$`               |
| $\cdots$               | `$\cdots$`               |
| $\vdots$               | `$\vdots$`               |
| $\ddots$               | `$\ddots$`               |



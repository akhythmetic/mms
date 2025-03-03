---
---
---

# REVISION CC1

## [Rappel]{.underline}

### V.A. $\mathbb{R}$

-   $$
    P(X=x) = F(x)
    $$

-   $$
    0 \leq F(x) \leq 1
    $$

-   $$
    E(X)=\int_{x\in \mathbb{R}} xf(x) dx
    $$

-   $$
    V(X)=E(X^2)-E(X)^2
    $$

### Couple de V.A. $\mathbb{R}$

-   $$
    F(x,y)=P(X\leq x,Y\leq y) 
    $$

$$
f(x,y)=\frac{\partial^2}{\partial x \partial y} F(x,y)
$$

-   Densités marginales :$$
    \begin{cases}
    f_X(x)=\int_{y\in \mathbb{R}} f(x,y) dy \\
    f_Y(y)=\int_{x\in \mathbb{R}} f(x,y) dx
    \end{cases}
    $$

-   $$
    f(x,y)=f_X(x)f_Y(y) \Leftrightarrow X\perp\!\!\!\perp Y
    $$

-   $$
    \int_{x\in \mathbb{R}}\int_{y\in \mathbb{R}} f(x,y)=1
    $$

-   $$
    E(X)= \int_{x\in\mathbb{R}} f(x) dx
    $$

-   

    $$
    Cov(X,Y)= E[(X-E(X))(Y-E(Y))] \\
    =E(XY)-E(X)E(Y)\\
    \\
    \text{avec } E(XY)=\int \int_{x\in \mathbb{R}}\int_{y\in \mathbb{R}} f(x,y) dx dy \\
    Cov(X,Y) \in ]-\infty,+\infty[
    $$

-   $$
    \rho_{X,Y}=\frac{Cov(X,Y)}{\sqrt{V(X)V(Y)}}
    $$ (cf : [remise à niveau sur la correlation](https://akhythmetic.github.io/mms/fiche_revision/ran_correlation.html))

    #### Propriété algébrique

-   

    $$
    E[aX+b]=aE(X)+b \\
    V[aX+b]=a^2V(X) \\
    E[aX+bY]=aE(X)+bE(Y) \\
    V[aX+bY]=a^2V(X)+b^2V(Y)+2Cov(X,Y)
    $$

-   

$$
E[AX+b]=AE(X)+b \\
=A\mu+b
\\ -\\
V[AX]=AV(X)A^T\\
=A\Sigma A^T
\\-\\
Cov[aX+bY,Z]=aCov(X,Z)+bCov(Y,Z) \qquad \text{Bilinéarité !!}
$$

## [Chap. 1]{.underline}

-   Matrice variance-covariance :$$
    V(X)=E[(X-E(X))(X-E(X))^T]
    $$

-   $$
    (AB)^T=B^TA^T
    $$

-   Une matrice $\Sigma$ est une matrice de variance-covariance si et seulement si elle rempli les conditions ci dessous:

    -   $\Sigma=\Sigma^T$ (Symetrie)

    -   $\forall X_{[d*1]}\in \mathbb{R}^d,  X^T\Sigma X\geq 0.\quad \Sigma$ est PSD (semie définie posfitif). Ou les val.p. sont tous supérieur ou egales à 0.

    -   $\forall i, \Sigma_{ii} \geq0$

-   

    $$
    \forall i\neq j, X_i\perp\!\!\!\perp X_j \Rightarrow Cov(X_i,X_j)=0\\
    \Rightarrow f(x_1,...,x_d)=f_1(x_1)\times...\times f_d(x_d)\\
    =\Pi_{i=1}^d f_i(x_i)
    $$

-   Conditionnel :

    $$
    X_A|X_B = x_b \sim \mathcal{N}(m,s),\\
    m=\mu_A+\Sigma_{AB}\Sigma_B^{-1}(x_B-\mu_b)\\
    s=\Sigma_{AA}-\Sigma_{AB}\Sigma_{BB}^{-1}\Sigma_{AB}^T
    $$

-   Loi $X^d\sim\mathcal{N}(\mu,\Sigma)$:

    $$
    \frac{1}{\sqrt{(2\pi)^d|\Sigma|}}e^{-\frac{1}{2}(x-\mu)^T\Sigma^{-1}(x-\mu)}
    $$

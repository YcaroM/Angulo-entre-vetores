---
author:
- Ycaro César Albano Martins
date: 2022-11-08
subtitle: Uma consequência da desigualdade de Cauchy-Schwarz
title: Ângulo entre vetores
---

::: frame
:::

::: frame
**Definição 1:** O produto interno entre dois vetores é uma operação que
associa dois vetores do ${\mathbb{R}}^n$ a um número real.
$$\left<\cdot,\cdot\right>:{\mathbb{R}}^n \times {\mathbb{R}}^n \rightarrow {\mathbb{R}}$$
O produto interno é definido por
$$\left<\vec{x},\vec{y}\right> = \sum_{i=1}^{n} x_{i}y_{i}$$
:::

::: frame
**Propriedades:** Sejam
$\vec{x},\vec{y},\vec{z} \in \mathbb{R}^n\ e\ \beta \in \mathbb{R}$

1.  $\left<\vec{x},\vec{y}\right> = \left<\vec{y},\vec{x}\right>$

2.  $\left<\beta \vec{x},\vec{y}\right> = \beta \left<\vec{x},\vec{y}\right>$

3.  $\left<\vec{x},\vec{y}+\vec{z}\right>=\left<\vec{x},\vec{y}\right>+\left<\vec{x},\vec{z}\right>$

4.  $\left<\vec{x},\vec{x}\right>\geq 0$, com
    $\left<\vec{x},\vec{x}\right> \Leftrightarrow \vec{x} =0$
:::

::: frame
Vamos dar mais uma atenção para o resultado do produto interno
$\left<\vec{x},\vec{x}\right>$:
$$\left<\vec{x},\vec{x}\right> = \sum_{i=1}^{n} x_{i}x_{i} = x_{1}x_{1} + x_{2}x_{2}+\cdots+x_{n}x_{n} = {x_{1}}^2 + {x_{2}}^2 +\cdots+{x_{n}}^2$$
Daí tiramos a segunda definição.\
**Definição 2:** Seja $\vec{x} \in {\mathbb{R}}^n$. O comprimento do
vetor $\vec{x}$ é chamado de norma do vetor $\vec{x}$ e é dado por
$$\|\vec{x}\| = \sqrt{\left<\vec{x},\vec{x}\right>} = \sqrt{{x_{1}}^2 + {x_{2}}^2 +\cdots+{x_{n}}^2}$$
:::

::: frame
**Propriedades da norma:**

1.  $\|\beta \vec{x}\|= |\beta|\|\vec{x}\|$, para todo
    $\beta \in \mathbb{R}$ e todo $\vec{x} \in {\mathbb{R}}^n$

2.  $\|\vec{x}+\vec{y}\| \leq \|\vec{x}\|+ \|\vec{y}\|$, para todo
    $\vec{x},\vec{y} \in {\mathbb{R}}^n$

3.  $\|\vec{x}\| \geq 0$, com $\|\vec{x}\|=0 \Leftrightarrow \vec{x}=0$.
:::

::: frame
**Teorema(Desigualdade de Cauchy-Schwarz):** Sejam
$\vec{x},\vec{y} \in {\mathbb{R}}^n$, então
$\left<\vec{x},\vec{y}\right>^2 \leq \|\vec{x}\|^2 \|\vec{y}\|^2$. A
igualdade é válida se, e somente se, $\vec{x}$ e $\vec{y}$ são
múltiplos.
:::

::: frame
*Prova:*
$$\left<\vec{x},\vec{y}\right>^2 = (x_{1}y_{1}+\cdots+x_{n}y_{n})^2 = \sum_{i=1}^{n} {x_{i}}^2 {y_{i}}^2 + \sum_{i<j} 2x_{i}y_{i}x_{j}y_{j}$$
$$\leq \sum_{i=1}^{n} {x_{i}}^2 {y_{i}}^2 + \sum_{i<j}({x_{i}}^2 {y_{j}}^2 + {x_{j}}^2 {y_{i}}^2)$$
$$= \sum_{i,j}{x_{i}}^2 {y_{j}}^2 = ({x_{1}}^2 +\cdots+{x_{n}}^2)({y_{1}}^2 + \cdots + {y_{n}}^2)
        = \|\vec{x}\|^2 \|\vec{y}\|^2$$\
Perceba que a igualdade só é satisfeita caso
$\vec{x} = \lambda \vec{y}$.
:::

::: frame
Concluímos da desigualdade de Cauchy-Schwarz que
$$\left<\vec{x},\vec{y}\right>^2 \leq \|\vec{x}\|^2 \|\vec{y}\|^2 \Rightarrow -1 \leq \frac{\left<\vec{x},\vec{y}\right>}{\|\vec{x}\| \|\vec{y}\|} \leq 1$$
Portanto, podemos definir o ângulo entre dois vetores $\vec{x}$ e
$\vec{y}$ como sendo
$$\theta =Arcos\left( \frac{\left<\vec{x},\vec{y}\right>}{\|\vec{x}\| \|\vec{y}\|}\right)$$
:::

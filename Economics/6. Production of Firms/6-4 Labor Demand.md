Based on the small firm's [[6-3 Intertemporal Profit Function|dynamic profit function]], the first-order conditions with respect to $n_1$ and $n_2$ are:
$$
\begin{align}
P_1f_n(k_1,n_1) - P_1w_1=0 \\
\\
\frac{P_2f_n(k_2,n_2)}{1+i}-\frac{P_2w_2}{1+i}=0
\end{align}
$$
	Where $f_n(k_t,n_t)$ denotes the [[6-2 Marginal Product|marginal product]] of labor (MPn) at period t. Because the labor demand function ==takes values from a single period at once==, it is a "static" phenomenon.

Simplifying, we get two equations:
$$
\begin{align}
w_1 = f_n(k_1,n_1) \\
w_2 = f_n(k_2, n_2)
\end{align}
$$
	This means that when the small firm is maximizing profit, it chooses its optimal quantity of labor so that the real MPn is equal to the real market wage.

>**Example**:  
```tikz
\begin{document}
  \begin{tikzpicture}[domain=0:4]
    \draw[->] (0,0) -- (4.2,0) node[right]{$n_t$};
    \draw[->] (0,0) -- (0,4.2) node[above]{$f_n(k_t,n_t)$};
    \draw[color=black] (1,3) -- (3.5, 1) node[right]{Firm's Labor Demand};
    \draw[color=black] plot(\x, 2) node[right]{$w_t$};
    \draw[dotted] (2.3, 2) -- (2.3, 0) node[below]{$n^*$};
  \end{tikzpicture}
\end{document}
```
>From the perspective of a small firm, the point where $w_t = f_n(k_t,n_t)$ is the optimal choice of labor for the small firm. Note that $slope(MPn) = Labor Demand$ since based on the $MPn$ the company will choose how many workers to employ. In essence, $MPn$ is the small firm's marginal benefit of one more worker, $w_t$ is the marginal cost of one more worker, and $n^*$ is the optimal amt. of workers. 

```tikz
\begin{document}
  \begin{tikzpicture}[domain=0:4]
    \draw[->] (0,0) -- (4.2,0) node[right]{$n_t$};
    \draw[->] (0,0) -- (0,4.2) node[above]{$w_t$};
    \draw[color=black] (1,3) -- (3.5, 1) node[right]{Market Labor Demand};
  \end{tikzpicture}
\end{document}
```
>Making $w_t$ a variable, as it decreases, the firm hires more labor. As it increases, the firm hires more labor. Therefore, market labor demand depends negatively on the real wage.
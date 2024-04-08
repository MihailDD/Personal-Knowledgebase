Also based on the small firm's [[6-3 Intertemporal Profit Function|dynamic profit function]], the first order conditions with respect to $k_2$ (the only variable $k$ in the two-period framework since $k_1=c$ and $k_3=0$) is:
$$
-P_1 + \frac{P_2f_k(k_2,n_2)}{1+i} + \frac{P_2}{1+i}=0 \
\text{or} \
\frac{(1+i)P_1}{P_2} - 1 = f_k(k_2,n_2)
$$
	Where $f_k(k_t,n_t)$ denotes the [[6-2 Marginal Product|marginal product]] of capital (MPk).

However, $r + 1 = (1+i)\frac{P_1}{P_2}$ (Fisher equation), so for a two-period framework:
$$
r_1 = f_k(k_2,n_2)
$$
	This means that a firm decides how much capital it'd like to have in the future based on the real interest rate $r_t$ between the two periods. Because capital demand ==takes values from both periods at once==, it is a "dynamic" phenomenon.

>**Example:**
```tikz
\begin{document}
  \begin{tikzpicture}[domain=0:4]
    \draw[->] (0,0) -- (4.2,0) node[right]{$k_2$};
    \draw[->] (0,0) -- (0,4.2) node[above]{$f_k(k_2,n_2)$};
    \draw[color=black] (1,3) -- (3.5, 1) node[right]{Firm's Capital Demand};
    \draw[color=black] plot(\x, 2) node[right]{$r$};
    \draw[dotted] (2.3, 2) -- (2.3, 0) node[below]{$k^*$};
  \end{tikzpicture}
\end{document}
```
>In the perspective of a small firm, the optimal point of capital $k^*$ is the point at which ${MPk} = r_t$.

However, desired capital is a stock (accumulation) measure, and we need something else in order to measure the optimal flow of investment.
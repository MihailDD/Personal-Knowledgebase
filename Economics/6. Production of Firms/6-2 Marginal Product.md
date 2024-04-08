Marginal product is the ==amount of extra output== produced by a ==little bit of extra input==.

>**Example (graph TBC):**
```tikz
\begin{document}
  \begin{tikzpicture}[domain=0:4]
    \draw[->] (0,0) -- (4.2,0) node[right]{$k_t$};
    \draw[->] (0,0) -- (0,4.2) node[above]{$A_tf(k_t,n_t)$};
    \draw[-] (0, 0) arc (180:90:3.5) node[right]{MPk};
   \end{tikzpicture}
\end{document}
```
>[[6-1 The Production Function|Production function ]]has a *strictly positive marginal product* ($A_tf_k(k_t,n_t)>0$ and $A_tf_n(k_t,n_t)>0$), and a *strictly diminishing marginal product* ($f_{kk}(A_tk_t,n_t)<0$ and $A_tf_{nn}(k_t,n_t)<0$) in both $k_t$ and $n_t$ since each of its two arguments is strictly increasing at a decreasing rate as the other is ==held constant==.
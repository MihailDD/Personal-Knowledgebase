As stated in the previous [[6-6 Capital Demand|desired (demanded) capital]] is a stock (accumulation) measure, and we need something else in order to measure the optimal flow of investment of a small firm... 

Enter capital **[[6-5 Net & Gross Investment||investment]]** demand (the change in a firm's capital stock demand between two periods).

>**Example:**
```tikz
\begin{document}
  \begin{tikzpicture}[domain=0:4]
    \draw[->] (0,0) -- (4.2,0) node[right]{$k_1$};
    \draw[->] (0,0) -- (0,4.2) node[above]{$f_k(k_2,n_2)$};
    \draw[color=black] (1,3) -- (3.5, 1) node[right]{Firm's Capital Investment Demand};
    \draw[color=black] plot(\x, 2) node[right]{$r$};
    \draw[dotted] (2.3, 2) -- (2.3, 0) node[below]{${inv}^*$};
  \end{tikzpicture}
\end{document}
```
>Considering $k^*$, we can denote ${inv}^* = k^*_2 - k_1$ to be the firm's optimal capital investment demand quantity (we assume that $k_1 < k_2^*$ as in most macroeconomic cases). This figure is qualitatively equivalent to the capital demand figure. However, here ${inv}^*$ is a flow variable that decides the optimal investment of the firm for period 2 in period 1 (using time-to-build).
```tikz
\begin{document}
  \begin{tikzpicture}[domain=0:4]
    \draw[->] (0,0) -- (4.2,0) node[right]{${inv}_1$};
    \draw[->] (0,0) -- (0,4.2) node[above]{$r$};
    \draw[color=black] (1,3) -- (3.5, 1) node[right]{Market Capital Investment Demand};
  \end{tikzpicture}
\end{document}
```
>We can generalize the previous figure into the market capital investment function. Sometimes $r$ is replaced by $P_1$, where $P_2$ and $i$ are fixed:
```tikz
\begin{document}
  \begin{tikzpicture}[domain=0:4]
    \draw[->] (0,0) -- (4.2,0) node[right]{${inv}_1$};
    \draw[->] (0,0) -- (0,4.2) node[above]{$P_1$};
    \draw[color=black] (1,3) -- (3.5, 1) node[right]{Market Investment Demand};
  \end{tikzpicture}
\end{document}
```
>This comes directly from the Fisher equation:
$$
1+r = \frac{1+i}{1+\pi_2}=(1+i)\frac{P_1}{P_2}
$$
>Where $\pi_2=\frac{P_2}{P_1}-1$ is the inflation rate from period 1 to period 2.

**Limitation:** Displaying the market investment demand as a function of ${inv}_1$ and $P_1$ makes it appear that a "static" price leads to a downward-sloping investment demand function. However, it is useful for horizontal summation with consumption demand from leisure or savings models.
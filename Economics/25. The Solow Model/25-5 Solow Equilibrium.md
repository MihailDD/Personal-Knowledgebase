In order to proceed further, we must [[25-4 Aggregate Savings & Investment|de-trend]] the framework since it cannot take infinite values of GDP (or inputs of savings, investment or consumption). We start by denoting two lowercase variables which denote **per unit of effective labor variables**:
$$
y_t \equiv \frac{Y_t}{X_tN_t} 
\ \ \text{ and } \ \
k_t \equiv \frac{K_t}{X_tN_t}
$$
	Where $y_t$ is the GDP "per capita", and $k_t$ is the capital "per capita."

Knowing these definitions, we can divide the [[25-3 Aggregate Production|GDP production function]] $Y_t=K_t^\alpha(X_tN_t)^{1-\alpha}$ from earlier by $X_tN_t$:
$$
\begin{alignat}{}
	\frac{Y_t}{X_t N_t} = \left(\frac{Y_t}{X_t N_t}\right)^\alpha \left(\frac{X_t N_t}{X_tN_t}\right)^{1-\alpha}
	\\ \text{or} \\
	y_t=k_t^\alpha
\end{alignat}



$$
	Which expresses per-capita output as a function of diminishing marginal product of capital (since $0<\alpha < 1$).

Using the same reasoning, we will divide the aggregate gross investment function $K_{t+1}-(1-\delta)K_t= I_t = s \cdot Y_t$ by $X_tN_t$:
$$
\begin{alignat}{0}
	\frac{K_{t+1}}{X_tN_t}-(1-\delta)\frac{K_{t}}{X_tN_t} = s\frac{Y_t}{X_tN_t}
	\\\text{or} \\
	\frac{K_{t+1}}{X_tN_t}-(1-\delta)k_t=s \cdot y_t
	\\\text{or} \\
	\frac{K_{t+1}}{X_tN_t}-(1-\delta)k_t=s \cdot k_t^\alpha
\end{alignat}
	
$$
>**Example:**
>
```tikz
\begin{document}
  \begin{tikzpicture}[domain=0:4]
    \draw[->] (0,0) -- (4.2,0) node[right]{Per-Capita Capital ($k_t$)};
    \draw[->] (0,0) -- (0,4.2) node[above]{Per-Capita Variables};
    \draw[-] (0, 0) arc (180:90:3.5) node[right]{Per-Capita Output ($y_t$)};
    \draw[dashed] (0, 0) arc (180:90:4 and 2) node[right]{Per-Capita Savings ($s \cdot y_t = s \cdot k_t^\alpha$)};
   \end{tikzpicture}
\end{document}
```
>Here, $C_t = y_t - s \cdot y_t = y_t(1-s)$ is the consumption at period c.

However, $K_{t+1}$ remains to be de-trended, which we do by multiplying by $\frac{X_{t+1}N_{t+1}}{X_{t+1}N_{t+1}}$:
$$
\begin{alignat}{}
\left(\frac{K_{t+1}}{X_{t+1}N_{t+1}}\right)\left(\frac{X_{t+1}N_{t+1}}{X_{t}N_{t}}\right)-(1-\delta)k_t=s \cdot k_t^\alpha
\end{alignat}
$$
Referring back to our [[25-2 Exogenous Growth Factors|exogenous growth factors]] $gr_N = \frac{N_{t+1}}{N_{t}} - 1$ and $gr_X = \frac{X_{t+1}}{X_{t}} - 1$ we substitute:
$$
\begin{alignat}{0}
k_{t+1}(1+{gr}_X)(1+{gr}_N)-(1-\delta)k_t=s \cdot k_t^\alpha
\\
\\ \text{or} \\
\\
k_{t+1}=\frac{s\cdot k_t^\alpha + (1-\delta)k_t}{(1+{gr}_X)(1+{gr}_N)}
\end{alignat}
$$
	This defines the equilibrium law of motion for the (per-capita) capital stock k in the Solow model. More importantly, it states that using the given values of $s, \alpha, {gr}_X, {gr}_N, and \ \delta$, at the beginning of period $t+1$ capital stock $k_{t+1}$ is completely determined solely by $k_t$.

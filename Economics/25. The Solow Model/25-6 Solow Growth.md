Imposing steady state (long-run) in the [[25-5 Solow Equilibrium|law of motion]] by arriving at $k^*$ gives us
$$
k^*=\frac{s\cdot (k^*)^\alpha + (1-\delta)k^*}{(1+{gr}_X)(1+{gr}_N)}
$$
Isolating $k^*$, this equates to:
>[!Theorem]
>$$
>\begin{equation}
>{k^* =\left(\frac{s}{(1+{gr}_X)(1+{gr}_N)-(1-\delta)}\right)}^\frac{1}{1-\alpha}
>\end{equation}
>$$
>Which is the Solow framework for steady-state $k^*$.

Simplifying in terms of basic economics, we set ${gr}_X={gr}_N=0$, which then leaves us with
$$
\begin{equation}
{k^* =\left(\frac{s}{\delta}\right)}^\frac{1}{1-\alpha}
\end{equation}
$$
	Which means that an increase in savings or a decrease in depreciation leads to an increase in wealth.

>[!example] 
>
>```tikz
>\begin{document}
>\begin{tikzpicture}[domain=0:4]
>\draw[->] (0,0) -- (4.2,0) node[right]{Per-Capita Capital ($k_t$)};
>\draw[->] (0,0) -- (0,4.2) node[above]{Per-Capita Variables};
>\draw[color=black] plot(\x, \x / 1.25) node[right]{Per-Capita Break-Even Investment $({gr}_X+{gr}_N+\delta)k_t$};
>\draw[dotted] (2.25,1.8) -- (2.25,0) node[below]{$k^*$};
>\draw[dashed] (0, 0) arc (180:90:4 and 2) node[right]{Per-Capita Savings ($s \cdot y_t = s \cdot k_t^\alpha$)};
>\end{tikzpicture}
>\end{document}
>```
>Where break-even investment is the amount of additional investment required to replace [[25-4 Aggregate Savings & Investment|depreciated capital]] or account for [[25-2 Exogenous Growth Factors|population or technological growth]] and $k^*$ is the long-run level of physical capital.
>
>**Note:** if $k < k^*$, savings exceed break-even investment and cause $k$ to converge toward $k^*$.

Does this mean that in the long-run an economy will always converge to steady-state $k^*$? In the model, yes. However:

>[!Warning]
>The Solow model makes a few assumptions:
>1.  All economies will eventually converge to steady state. However, if "mature" economies like the U.S., Japan, etc. have converged to $k^*$, then they would all have equal per-capita capital stocks.
>    This issue is resolved by introducing unique rates of saving or depreciation for every economy. Consider two economies with distinct savings rates $s_1$ and $s_2$:
>```tikz
>\begin{document}
>\begin{tikzpicture}[domain=0:4]
>\draw[->] (0,0) -- (4.2,0) node[right]{Per-Capita Capital ($k_t$)};
>\draw[->] (0,0) -- (0,4.2) node[above]{Per-Capita Variables};
>\draw[dashed] (1.65,1.65) -- (1.65,0) node[below]{$k^*_1$};
>\draw[->] (2.9,2.9) -- (2.9,0) node[below]{$k^*_1$};
>\draw[color=black] plot(\x, \x) node[right]{Per-Capita Break-Even Investment $({gr}_X+{gr}_N+\delta)k_t$};
>\draw[dashed] (0, 0) arc (180:90:4 and 2) node[right]{Per-Capita Savings of Economo 1 ($s_1y_t$)};
>\draw[->] (0, 0) arc (180:90:4 and 3) node[right]{Per-Capita Savings of Economy 2 ($s_2y_t$)};
>\end{tikzpicture}
>\end{document}
>```
>2. All economies eventually reach a state of 0 growth when a steady-state $k^*$ is achieved.
>    Reversing the [[25-5 Solow Equilibrium|de-trending procedure]] to get $Y_t=K_t^\alpha(X_tN_t)^{1-\alpha}$, we can see that the overall economy is experiencing growth for as long as population and productivity are growing. However, per-capita growth is the more important notion.
>3. Depreciation is constant and equal for all capital.

Based on the model, "mature" economies whose population growth is slowing down appear to be driven by total factor productivity, which accounts for their increased $k^*$.
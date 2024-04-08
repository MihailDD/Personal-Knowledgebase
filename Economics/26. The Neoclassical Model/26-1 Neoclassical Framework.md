>[!Theorem]
>The neoclassical framework works to maximize present discounted value of lifetime utility subject to the constraint $c_t+k_{t+1}-(1-\delta)k_t=k_t^\alpha$:
>$$
>\max_{\mathclap{\text{{$\{c_t,k_{t+1}\}^\infty_{t+1}$}}}} \ \ \ \sum^{\infty}_{t=1}\beta^{t-1}u(c_t)
>$$
>Where $\beta \in (0, 1)$ is the one-period-ahead subjective discount factor.

In order to implement the constraint, we must perform a Lagrange optimization on the neoclassical framework with respect to $c_t$ and $k_{t+1}$:
$$
\begin{alignat}{0}
u'(c_t)=\lambda_t \\
-\lambda_{t}+\beta \lambda_{t+1}(1+\alpha k_t^{\alpha - 1}-\delta) = 0
\end{alignat}
$$
...which lead to
$$u'(c_t) = \beta u'(c_{t+1})[1+\alpha k_t^{\alpha - 1}-\delta]$$

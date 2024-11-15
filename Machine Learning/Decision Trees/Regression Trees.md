- Constructed same way as classification trees
- Let for Node m, $x_{m}$, is the subset of X, reaching node m, then, condition on decision node:
$$b_{m}(x) = \Bigg\{ \begin{matrix}
1 &  if \ x \ \epsilon \ X_{m}:x \ reaches \ node \ m\\
0 & otherwise
\end{matrix}$$
- Goodness of split is measured by MSE
$$E_{m} = \frac{1}{N_{m}}\sum_{t}(r^{t}-g_{m})^{2}b_{m} (x^{t})$$
$$g_{m} = \frac{\sum_{t} b_{m}(x^t)r^{t}}{\sum_{t} b_{m}(x^t)}$$
- After Split:
$$b_{mj}(x) = \Bigg\{\begin{matrix}
1 &  if \ x \ \epsilon \ X_{m}:x \ reaches \ node \ m \ and \ branch \ j \\
0 & otherwise
\end{matrix}$$
$$E^{'}_{m} = \frac{1}{N_{m}}\sum_{j}\sum_{t}(r^{t}-g_{mj})^{2}b_{mj}(x^{t})$$
$$g_{mj} = \frac{\sum_{t}b_{mj}(x^t)r^{t}}{\sum_{t}b_{mj}(x^t)}$$
- Error drop is given by difference between errors before split and after split


>[!THEOREM] Theorem: Linearity of Differentiation
>
>The [differentiation](Differentiability%20of%20Curve%20Parameterisations.md) operation for [curve parameterisations](../Curve%20Parameterisation.md) is linear - for all [curve parameterisations](../Curve%20Parameterisation.md)  $\mathbf{u},\mathbf{v}:I\subseteq \mathbb{R}\to\mathbb{R}^n$ and all $\mu,\lambda \in \mathbb{R}$:
>
>$$\frac{\mathrm{d}}{\mathrm{d}t}[\lambda\,\mathbf{u}(t) + \mu\,\mathbf{v}(t)] = \lambda\,\mathbf{u}'(t) + \mu\,\mathbf{v}'(t)$$
>
>
>>[!PROOF]-
>>
>>TODO
>>

>[!THEOREM] Theorem: Chain Rule
>For every [differentiable real function](../../../Real%20Analysis/Differentiation/Differentiability%20of%20Real%20Functions.md) $f:I\subseteq\mathbb{R}\to\mathbb{R}$ and every [differentiable curve parameterisation](Differentiability%20of%20Curve%20Parameterisations.md) $\mathbf{r}:f(I)\to\mathbb{R}^n$:
>
>$$\frac{\mathrm{d}}{\mathrm{d}t}\mathbf{r}(f(t)) = f'(t)\,\mathbf{r}'(f(t))$$
>
>>[!PROOF]-
>>
>>TODO
>>
>
>^chainrule

>[!THEOREM] Theorem: Product Rules
>
>- *Basic Product Rule*: For every [differentiable curve parameterisation](Differentiability%20of%20Curve%20Parameterisations.md) $\mathbf{r}:I\to\mathbb{R}^n$ and every [differentiable real function](../../../Real%20Analysis/Differentiation/Differentiability%20of%20Real%20Functions.md) $f:I\subseteq\mathbb{R}\to\mathbb{R}$
>
>$$\frac{\mathrm{d}}{\mathrm{d}t}[f(t)\mathbf{r}(t)] = f'(t)\mathbf{r}(t) + \mathbf{r}'(t)f(t)$$
>
>- *Dot Product Rule*: For the [dot product](../../../../Algebra/Linear%20Algebra/Matrices/Row%20&%20Column%20Vectors/Real%20Vectors/Real%20Dot%20Product.md) of all [differentiable curve parameterisations](Differentiability%20of%20Curve%20Parameterisations.md) $\mathbf{u},\mathbf{v}:I\subseteq \mathbb{R}\to\mathbb{R}^n$
>
>$$\frac{\mathrm{d}}{\mathrm{d}t}[\mathbf{u}(t)\cdot\mathbf{v}(t)] = \mathbf{u}'(t)\cdot \mathbf{v}(t) + \mathbf{u}(t)\cdot\mathbf{v}'(t)$$
>
>- *Cross Product Rule*: For the [cross product](TODO) of all [differentiable curve parameterisations](Differentiability%20of%20Curve%20Parameterisations.md) $\mathbf{u},\mathbf{v}:I\subseteq \mathbb{R}\to\mathbb{R}^3$
>
>$$\frac{\mathrm{d}}{\mathrm{d}t}[\mathbf{u}(t)\times \mathbf{v}(t)] = \mathbf{u}'(t)\times\mathbf{v}(t) + \mathbf{u}(t)\times\mathbf{v}'(t)$$
>
>>[!PROOF]-
>>
>>TODO
>>
>
>[!DEFINITION] Definition: Curve
>
>A **curve** $\mathcal{C}$ in $\mathbb{R}^n$ is a [subset](../../../Set%20Theory/Subset.md) of the [real vector space](../../../Algebra/Linear%20Algebra/Matrices/Row%20&%20Column%20Vectors/Real%20Vectors/Structure%20of%20the%20Real%20Vector%20Space.md) $\mathbb{R}^n$ for which there is a [function](../../../Analysis/Vector%20Analysis/Curve%20Parameterisation/Curve%20Parameterisation.md) $\gamma: I \subseteq \mathbb{R} \to \mathbb{R}^n$ whose [image](../../../Set%20Theory/Functions/Function.md) is $\mathcal{C}$.
>
>The function $\gamma$ is called a **parameterisation** of $\mathcal{C}$.
>
>>[!NOTE]
>>
>>A curve may have multiple parameterisations.
>>
>
>>[!NOTE]
>>
>>The curve and its parameterisations are both often referred to as "curve".
>
>>[!DEFINITION] Definition: Start and End Points
>>
>>If a [curve parameterisation](Curve.md) has the form $\gamma: [a;b] \to \mathbb{R}^n$, then we call $\gamma(a)$ its **start point** and $\gamma(b)$ its **end point**.
>>
>

>[!THEOREM] Theorem: Curve Reparameterisation
>
>If $\gamma: [a;b] \to \mathbb{R}^n$ and $\varphi: [c;d] \to \mathbb{R}^n$ are [parameterisations](../../../Analysis/Vector%20Analysis/Curve%20Parameterisation/Curve%20Parameterisation.md) of the same [curve](Curve.md) $\mathcal{C}$, then there exists a [bijective](../../../Set%20Theory/Functions/Injection,%20Surjection,%20Bijection.md), [continuously differentiable real function](../../../Analysis/Real%20Analysis/Differentiation/Differentiability%20of%20Real%20Functions.md) $u: [a;b] \to [c;d]$ with a continuously differentiable [inverse](../../../Set%20Theory/Functions/Inverse%20Function.md) such that
>
>$$\varphi(u(t)) = \gamma(t)$$
>
>Moreover, one of the following must be true:
>
>- $u(a) = c$ and $u(b) = d$
>- $u(a) = d$ and $u(b) = c$
>
>>[!DEFINITION] Definition: Parameterisation Orientation
>>
>>If $u(a) = c$ and $u(b) = d$, then we say that $\gamma$ and $\varphi$ have the **same orientation**.
>>
>>If $u(a) = d$ and $u(b) = c$, then we say that $\gamma$ and $\varphi$ have **opposite orientations**.
>>
>>^orientation
>
>>[!PROOF]-
>>
>>TODO
>>
>

>
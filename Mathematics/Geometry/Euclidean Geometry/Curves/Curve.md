>[!DEFINITION] Definition: Curve
>
>A **curve** $\mathcal{C}$ in $\mathbb{R}^n$ is a [geometric figure](../../Geometric%20Figure.md) which is the [image](../../../Analysis/Functions/Function.md) of a nonconstant [curve parameterisation](../../../Analysis/Vector%20Analysis/Curve%20Parameterisations/Curve%20Parameterisation.md).
>
>>[!NOTE]
>>
>>A curve may have multiple parameterisations.
>>
>
>>[!NOTE]
>>
>>The curve and its parameterisations are both often referred to as "curve".
>>
>

>[!THEOREM] Theorem: Curve Reparameterisation
>
>If $\gamma: [a;b] \to \mathbb{R}^n$ and $\varphi: [c;d] \to \mathbb{R}^n$ are [parameterisations](../../../Analysis/Vector%20Analysis/Curve%20Parameterisations/Curve%20Parameterisation.md) of the same [curve](Curve.md) $\mathcal{C}$, then there exists a [bijective](../../../Analysis/Functions/Types%20of%20Functions/Injection,%20Surjection,%20Bijection.md), [continuously differentiable real function](../../../Analysis/Real%20Analysis/Differentiation/Differentiability%20of%20Real%20Functions.md) $u: [a;b] \to [c;d]$ with a continuously differentiable [inverse](../../../Analysis/Functions/Inverse%20Function.md) such that
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
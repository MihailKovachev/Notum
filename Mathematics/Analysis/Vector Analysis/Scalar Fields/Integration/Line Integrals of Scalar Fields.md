>[!THEOREM] Theorem: Line Integral of a Scalar Field
>
>Let $f: D \subseteq \mathbb{R}^n \to \mathbb{R}$ be a [real scalar field](../Real%20Scalar%20Field.md) and $\mathcal{C} \subset D$ be a [curve](../../../../Geometry/Topology/Curves/Curve.md).
>
>For all [piecewise continuously differentiable](../../Real%20Vector%20Functions/Differentiation/Partial%20Derivatives%20of%20Real%20Vector%20Functions.md) [parameterisations](../../Curve%20Parameterisation/Curve%20Parameterisation.md) $\gamma: [a;b] \to D$ and $\varphi: [c;d] \to D$ of $\mathcal{C}$, the following [definite integrals](../../../Real%20Analysis/Integration/Definite%20Integrals/Definite%20Integral.md) are equal:
>
>$$\int_a^b f(\gamma(t))\, ||\dot\gamma (t)||\mathop{\mathrm{d}t} = \int_c^d f(\varphi(t))\, ||\dot\varphi (t)||\mathop{\mathrm{d}t}$$
>
>>[!PROOF]-
>>
>>We will just show this for the case when $\gamma$ and $\varphi$ are *not* piecewise, since the proof is easily generalisable - if $\gamma$ and $\varphi$ *are* piecewise, then one can just apply the following proof to each of their partitions and obtain the same end result after summing the results from each partition.
>>
>>Since $\gamma$ and $\varphi$ parameterise the same curve $\mathcal{C}$, we can [reparameterise](../../../../Geometry/Topology/Curves/Curve.md) one in the other. More specifically, there exists a [bijective](../../../../Set%20Theory/Functions/Injection,%20Surjection,%20Bijection.md), [continuously differentiable function](../../../Real%20Analysis/Differentiation/Differentiability%20of%20Real%20Functions.md) $u: [a;b] \to [c;d]$ such that
>>
>>$$\varphi(u(t)) = \gamma (t)$$
>>
>>The [chain rule](../../Curve%20Parameterisation/Differentiation/Differentiation%20Rules%20for%20Curve%20Parameterisations.md#^chainrule) then gives us
>>
>>$$\int_a^b f(\gamma(t))\, ||\dot\gamma (t)||\mathop{\mathrm{d}t} = \int_a^b f(\varphi(u(t)))\, ||\dot\varphi (u(t)) u'(t)|| \mathop{\mathrm{d}t} =  \int_a^b f(\varphi(u(t)))\, ||\dot\varphi (u(t))|| \, |u'(t)|\mathop{\mathrm{d}t}$$
>>
>>If $\gamma$ and $\varphi$ have the [same orientation](../../../../Geometry/Topology/Curves/Curve.md#^orientation), then $u(a) = c$ and $u(b) = d$. Since $a \lt b, c \lt d$ and $u$ is bijective, $u$ must be [strictly increasing](../../../Real%20Analysis/Functions/Monotony/Monotony%20of%20Real%20Functions.md), i.e. $|u'(t)| = u'(t)$. We thus have
>>
>>$$\int_a^b f(\varphi(u(t)))\, ||\dot\varphi (u(t))|| \, |u'(t)|\mathop{\mathrm{d}t} = \int_a^b f(\varphi(u(t))) \, ||\dot\varphi (u(t))|| \, u'(t)\mathop{\mathrm{d}t}$$
>>
>>By applying the [substitution](../../../Real%20Analysis/Differentiation/Differentiation%20Rules.md) $\mathrm{d}u = u' \mathop{\mathrm{d}t}$, we obtain 
>>
>>$$\int_a^b f(\varphi(u(t)))\, ||\dot\varphi (u(t))|| \, u'(t)\mathop{\mathrm{d}t} = \int_c^d f(\varphi(u))\, ||\dot \varphi(u)|| \mathop{\mathrm{d}u}$$
>>
>>$$\int_a^b f(\gamma(t))\, ||\dot\gamma (t)||\mathop{\mathrm{d}t} = \int_c^d f(\varphi(u))\, ||\dot \varphi(u)|| \mathop{\mathrm{d}u}$$
>>
>>We are done with the case where $\gamma$ and $\varphi$ have the same orientation. Now, if $\gamma$ and $\varphi$ have [opposite orientations](../../../../Geometry/Topology/Curves/Curve.md#^orientation), then $u(a) = d$ and $u(b) = c$. Since $a \lt b, c \lt d$ and $u$ is bijective, $u$ must be [strictly decreasing](../../../Real%20Analysis/Functions/Monotony/Monotony%20of%20Real%20Functions.md), i.e. $|u'(t)| = -u'(t)$. We thus have
>>
>>$$\int_a^b f(\varphi(u(t)))\, ||\dot\varphi (u(t))|| \, |u'(t)|\mathop{\mathrm{d}t} = - \int_a^b f(\varphi(u(t)))\, ||\dot\varphi (u(t))|| \, u'(t)\mathop{\mathrm{d}t}$$
>>
>>By applying the substitution $\mathrm{d}u = u' \mathop{\mathrm{d}t}$, we obtain 
>>
>>$$- \int_a^b f(\varphi(u(t)))\, ||\dot\varphi (u(t))|| \, u'(t)\mathop{\mathrm{d}t} = - \int_d^c f(\varphi(u))\, ||\dot \varphi(u)|| \mathop{\mathrm{d}u} = \int_c^d f(\varphi(u))\, ||\dot \varphi(u)|| \mathop{\mathrm{d}u}$$
>>
>>$$\int_a^b f(\gamma(t))\, ||\dot\gamma (t)||\mathop{\mathrm{d}t} = - \int_d^c f(\varphi(u))\, ||\dot \varphi(u)|| \mathop{\mathrm{d}u} = \int_c^d f(\varphi(u))\, ||\dot \varphi(u)|| \mathop{\mathrm{d}u}$$
>>
>>And so the proof is complete.
>>
>
>>[!DEFINITION] Definition: Line Integral of a Scalar Field
>>
>>Let $f: D \subseteq \mathbb{R}^n \to \mathbb{R}$ be a [real scalar field](../Real%20Scalar%20Field.md) and $\mathcal{C} \subset D$ be a [curve](../../../../Geometry/Topology/Curves/Curve.md) with a [parameterisation](../../Curve%20Parameterisation/Curve%20Parameterisation.md) $\gamma: [a;b] \to D$. The **line integral** of $f$ over $\mathcal{C}$ is the [definite integral](../../../Real%20Analysis/Integration/Definite%20Integrals/Definite%20Integral.md)
>>
>>$$\int_a^b f(\gamma(t))\, ||\dot\gamma (t)||\mathop{\mathrm{d}t}$$
>>
>>>[!NOTATION]
>>>
>>>Since the line integral is independent of the curve parameterisation, we denote it by
>>>
>>>$$\int_\mathcal{C} f \mathop{\mathrm{d}s}$$
>>>
>>>If $\mathcal{C}$ is [closed](../../../../Geometry/Topology/Curves/Closed%20Curve.md), we write
>>>
>>>$$\oint_\mathcal{C} f \mathop{\mathrm{d}s}$$
>>>
>>
>

>[!THEOREM] Theorem: Linearity of the Scalar Line Integral
>
>The [scalar line integral](Line%20Integrals%20of%20Scalar%20Fields.md) is [linear](../../../../Algebra/Linear%20Algebra/Linear%20Transformations/Linear%20Transformation.md):
>
>$$\int_\mathcal{C} (\lambda\, f +\mu \, g)\mathop{\mathrm{d}s} = \lambda\int_\mathcal{C} f\mathop{\mathrm{d}s} + \mu \int_\mathcal{C} g\mathop{\mathrm{d}s}$$
>
>>[!PROOF]-
>>
>>$$\begin{align}\int_\gamma (\lambda\, f +\mu \, g)\mathop{\mathrm{d}s} &=\int_a^b [\lambda\, f(\gamma(t)) +\mu \, g(\gamma(t))]\,||\dot{\gamma}(t)||\mathop{\mathrm{d}t} \\ &=\int_a^b \lambda\, f(\gamma(t))\,||\dot{\gamma}(t)|| +\mu \, g(\gamma(t))\,||\dot{\gamma}(t)||\mathop{\mathrm{d}t} \\ &= \lambda \int_a^b f(\gamma(t)) \, ||\dot{\gamma}(t)|| \mathop{\mathrm{d}t} + \mu \int_a^b g(\gamma(t))\,||\dot{\gamma}(t)||\mathop{\mathrm{d}t} \\ &= \lambda\int_\gamma f\mathop{\mathrm{d}s} + \mu \int_\gamma g\mathop{\mathrm{d}s} \end{align}$$
>>
>

>[!THEOREM] Theorem: Partitioning of the Scalar Line Integral
>
>Let $f: D \subseteq \mathbb{R}^n \to \mathbb{R}$ be a [real scalar field](../Real%20Scalar%20Field.md) and $\mathcal{C} \subset D$ be a [curve](../../../../Geometry/Topology/Curves/Curve.md).
>
>If $\mathcal{C}$ can be represented as a [union](../../../../Set%20Theory/Operations%20with%20Sets/Union.md) $\mathcal{C} = \mathcal{C}_1 \cup \cdots \cup \mathcal{C}_k$ of finitely many [disjoint](../../../../Set%20Theory/Disjoint%20Sets.md) curves $\mathcal{C}_1, \cdots,\mathcal{C}_k$, then the [line integral](Line%20Integrals%20of%20Scalar%20Fields.md) of $f$ over $\mathcal{C}$ is just the sum of line integrals of $f$ over $\mathcal{C}_1, \cdots,\mathcal{C}_k$:
>
>$$\int_{\mathcal{C}} f\mathop{\mathrm{d}s} = \int_{\mathcal{C}_1} f\mathop{\mathrm{d}s} + \cdots + \int_{\mathcal{C}_k} f\mathop{\mathrm{d}s}$$
>
>>[!PROOF]-
>>
>>TODO
>>
>

>[!THEOREM] Mean value theorem for Scalar Line Integrals
>
>Let $f: D \subseteq \mathbb{R}^n \to \mathbb{R}$ be a [real scalar field](../Real%20Scalar%20Field.md) and $\mathcal{C} \subset D$ be a [continuous curve](../../../../Geometry/Topology/Curves/Continuous%20Curve.md).
>
>If $f$ is [continuous](../Continuity%20of%20Real%20Scalar%20Fields.md), then there exists a point $\vec{x} \in \mathcal{C}$ on the curve such that the [line integral](../../../../Geometry/Stereometry/Line.md) of $f$ over $\mathcal{C}$ is
>
>$$\int_\mathcal{C} f\mathop{\mathrm{d}s} = f(\vec{x})\cdot L$$
>
>where $L$ is the [length](../../../../Geometry/Topology/Curves/Arc%20Length.md) of $\mathcal{C}$.
>
>>[!PROOF]-
>>
>>TODO
>>
>
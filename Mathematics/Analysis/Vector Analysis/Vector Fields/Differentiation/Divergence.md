>[!DEFINITION] Definition: Divergence
>
>Let $\boldsymbol{v}: D \subseteq \mathbb{R}^n \to \mathbb{R}^n$ be a [real vector field](../Real%20Vector%20Field.md) with [component functions](../../Real%20Vector%20Functions/Real%20Vector%20Function.md) $v_1, \cdots, v_n$, where $v_i$ is [partially differentiable](../../Scalar%20Fields/Differentiation/Partial%20Derivatives%20of%20Real%20Scalar%20Fields.md) differentiable with respect to the $i$-th variable.
>
>The **divergence** of $\boldsymbol{v}$ is the [real scalar field](../../Scalar%20Fields/Real%20Scalar%20Field.md)
>
>$$\sum_{i=1}^n \partial_i v_i$$
>
>>[!NOTE]
>>
>>The divergence can be thought of as the [dot product](../../../../Algebra/Linear%20Algebra/Matrices/Row%20&%20Column%20Vectors/Real%20Vectors/Real%20Dot%20Product.md) of the [del operator](../Del%20Operator.md) with $\boldsymbol{v}$.
>>
>>$$\nabla \cdot \boldsymbol{v} = \begin{bmatrix}\frac{\partial}{\partial x_1} \\ \vdots \\ \frac{\partial}{\partial x_n}\end{bmatrix}\begin{bmatrix}v_1 & \cdots & v_n \end{bmatrix} = \frac{\partial v_1}{\partial x_1} + \cdots + \frac{\partial v_n}{\partial x_n}$$
>>
>
>>[!NOTATION]
>>
>>$$\nabla \cdot \boldsymbol{v} \qquad \mathop{\operatorname{div}}\boldsymbol {v}$$
>>
>
>>[!NOTE] Note: Geometric Meaning of Divergence
>>
>>
>>
>

>[!THEOREM] Theorem: Linearity of the Divergence
>
>The [divergence](Divergence.md) is [linear transformation](../../../../Algebra/Linear%20Algebra/Linear%20Transformations/Linear%20Transformation.md) - for all $\lambda, \gamma \in \mathbb{R}$ and all [vector fields](../Real%20Vector%20Field.md) $\boldsymbol{u}, \boldsymbol{v}: D \subseteq \mathbb{R}^n \to \mathbb{R}^n$ whose $i$-th [component functions](../../Real%20Vector%20Functions/Real%20Vector%20Function.md) are [partially differentiable](../../Scalar%20Fields/Differentiation/Partial%20Derivatives%20of%20Real%20Scalar%20Fields.md) with respect to the $i$-th variable:
>
>$$\mathop{\operatorname{div}} (\lambda \,\mathbf{u} + \mu\,\mathbf{v}) = \lambda \mathop{\operatorname{div}}(\mathbf{u})+\mu \mathop{\operatorname{div}}\mathbf{v}$$
>
>>[!PROOF]-
>>
>>TODO
>>
>

>[!THEOREM] Theorem: Product Rule for Divergence
>
>Let $\varphi: D \to \mathbb{R}$ be a [scalar field](../../Scalar%20Fields/Real%20Scalar%20Field.md) and $\mathbf{F}: D \to \mathbb{R}^n$ be a [vector field](../Real%20Vector%20Field.md) on an [open subset](../../../../Topology/Metric%20Spaces/The%20Metric%20Topology.md#^opensets) $D \subseteq \mathbb{R}^n$. 
>
>If $\varphi$ is [partially differentiable](../../Scalar%20Fields/Differentiation/Partial%20Derivatives%20of%20Real%20Scalar%20Fields.md) and $\mathbf{F}$'s $i$-th [component function](../../Real%20Vector%20Functions/Real%20Vector%20Function.md) is partially differentiable with respect to the $i$-th variable, then the [divergence](Divergence.md) of their product can be expressed via $\varphi$'s [gradient](../../Scalar%20Fields/Differentiation/Gradient.md) and $\mathbf{F}$'s divergence:
>
>$$\nabla\cdot(\varphi\mathbf{F}) = (\nabla\varphi)\cdot \mathbf{F} + \varphi\, (\nabla \cdot \mathbf{F})$$
>
>>[!PROOF]-
>>
>>TODO
>>
>
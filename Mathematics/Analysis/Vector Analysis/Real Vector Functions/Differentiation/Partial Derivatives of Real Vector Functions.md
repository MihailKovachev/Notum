>[!DEFINITION] Definition: Partial Derivative of a Real Vector Function
>
>Let $f: D \subseteq \mathbb{R}^m \to \mathbb{R}^n$ be a [real vector function](../Real%20Vector%20Function.md) with [component functions](../Real%20Vector%20Function.md) $f_1,\cdots,f_n$.
>
>The **partial derivative** of $f$ with respect to the variable $x_i$ is the [vector](../../../../Algebra/Linear%20Algebra/Matrices/Row%20&%20Column%20Vectors/Real%20Vectors/Real%20Vector.md) whose entries are the [partial derivatives](../../Scalar%20Fields/Differentiation/Partial%20Derivatives%20of%20Real%20Scalar%20Fields.md) of $f_1,\cdots,f_n$ with respect to $x_i$
>
>$$\frac{\partial f}{\partial x_i}(\vec{x}) \overset{\text{def}}{=} \begin{bmatrix}\frac{\partial f_1}{\partial x_i}(\vec{x}) \\ \vdots \\ \frac{\partial f_n}{\partial x_i}(\vec{x})  \end{bmatrix}$$
>
>>[!NOTATION]
>>
>>$$\frac{\partial f}{\partial x_i} (\vec{x}) \qquad  \frac{\partial}{\partial x_i} f(\vec{x})\qquad \partial_i f (\vec{x}) \qquad f_{x_i} (\vec{x}) \qquad f_{x_i}(\vec{x})$$
>>
>

>[!DEFINITION] Definition: (Continuous) Partial Differentiability
>
>A [real vector function](../Real%20Vector%20Function.md) is called $k$**-times (continuously) partially differentiable** if all of its $k$-th order [partial derivatives](Partial%20Derivatives%20of%20Real%20Vector%20Functions.md) exist (and are [continuous](../Continuity%20of%20Real%20Vector%20Functions.md)).
>
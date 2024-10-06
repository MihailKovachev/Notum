> [!DEFINITION] Definition: Field
>A **field** $(F, +, \cdot)$ is a [set](../../Set%20Theory/Set.md) $F$ which is equipped with an **addition** $+: F \times F \to F$ and a **multiplication** $\cdot: F \times F \to F$ [operations](../../Set%20Theory/Functions/Function.md) which have the following properties.
> 
>1. Addition:
>	- Commutativity: $\alpha + \beta = \beta + \alpha \qquad \forall \alpha,\beta \in F$
>	- Associativity: $(\alpha + \beta) + \gamma = \alpha + (\beta + \gamma) \qquad \forall \alpha,\beta,\gamma \in F$
>	- Existence and uniqueness of the additive identity: There is exactly one $0 \in F$ such that $\alpha + 0 = \alpha \qquad \forall \alpha \in F$
>	- Existence and uniqueness of additive inverses: For each $\alpha \in F$ there is exactly one $-\alpha \in F$ such that $\alpha + (-\alpha) = 0$
> 
>2. Multiplication:
>	- Commutativity: $\alpha \cdot \beta = \beta \cdot \alpha \qquad \forall \alpha,\beta \in F$
>	- Associativity: $(\alpha \cdot \beta) \cdot \gamma = \alpha \cdot (\beta \cdot \gamma) \qquad \forall \alpha,\beta,\gamma \in F$
>	- Existence and uniqueness of the multiplicative identity: There is exactly one $1 \in F$ such that $\alpha \cdot 1 = \alpha \qquad \forall \alpha \in F$
>	- Existence and uniqueness of multiplicative inverses: For each $\alpha \ne 0 \in F$ there is exactly one $\alpha^{-1} \in F$ mit $\alpha \cdot \alpha^{-1} = 1$
> 
>3. Distributive Law:
>$$\alpha\cdot(\beta + \gamma) = \alpha\cdot \beta + \alpha \cdot \gamma \qquad \forall \alpha,\beta,\gamma \in F$$

>[!THEOREM] 
>Every field is also a [commutative](../Rings/Commutative%20Ring.md) [ring](../Rings/Ring.md).
>>[!PROOF]-
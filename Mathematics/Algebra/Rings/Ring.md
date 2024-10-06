>[!DEFINITION] Definition: Ring
>A **ring** $(R, +, \cdot)$ is a [set](../../Set%20Theory/Set.md) $R$ equipped with an **addition** $+: R\times R \to R$ and a **multiplication** $\cdot: R\times R \to R$ [operations](../../Set%20Theory/Functions/Function.md) which satisfy the following properties.
>
>1. $R$ is an [abelian group](../Groups/Abelian%20Group.md) under addition, i.e.:
>	- $a + b = b + a$ for all $a,b \in R$
>	- $(a + b) + c = a + (b + c)$ for all $a,b,c \in R$;
>	- There exists an element $0 \in R$ such that $a + 0 = 0 + a = 0$ for all $a \in R$;
>	- For each $a \in R$ there exists $-a$ such that $a + (-a) = 0$.
>
>2. $R$ is a [monoid](../Monoid.md) under multiplication, i.e.:
>	- $(a\cdot b) \cdot c = a \cdot (b \cdot c)$ for all $a,b,c \in R$;
>	- There exists an element $1 \in R$ such that $a\cdot 1 = 1\cdot a = a$ for all $a \in R$.
>3. Multiplication is distributive with respect to addition, i.e.
>	- $a \cdot (b + c) = a \cdot b + a \cdot c$ for all $a,b,c \in R$
>	- $(a+b) \cdot c = a\cdot c + b \cdot c$ for all $a,b,c \in R$
>
>>[!NOTATION]
>>The multiplication is often denoted simply as $ab$ instead of $a\cdot b$.
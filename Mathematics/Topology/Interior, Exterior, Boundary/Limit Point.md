>[!DEFINITION] Definition: Limit Point
>
>Let $(X, \tau)$ be a [topological space](../Topological%20Space.md) and let $S$ be a [subset](../../../Set%20Theory/Subset.md) of $X$.
>
>A point $x \in X$ is a **limit point** of $S$ iff every [neighbourhood](../Neighbourhoods.md) of $x$ contains a point of $S$ different from $x$.
>
>>[!NOTE]
>>
>>Accumulation points are also known as **accumulation points** or **cluster points**.
>>
>
>>[!EXAMPLE]-
>>
>>Consider the topological space $(X, \tau)$, where $X = \{a,b,c,d,e\}$ and $\tau = \{\varnothing, X, \{a\}, \{c,d\}, \{a,c,d\}, \{b,c,d,e\}\}$. Suppose $S = \{a, b, c\}$. 
>>
>>The set $\{a\}$ is open but it does not contain any other element of $S$, hence $a$ is not a limit point of $S$.
>>
>>The sets which contain $b$ are $X$ and $\{b,c,d,e\}$. We see that $X$ contains $a$ (or alternatively $c$) which is another point of $S$. Similarly, we see that $\{b,c,d,e\}$ contain $c$ which is again another point of $S$. Therefore, all sets which contain $b$ also contain another point of $S$ and so $b$ is a limit point of $S$.
>>
>>The set $\{c,d\}$ contains $c$ but the only other element it contains is $d$ which is not an element of $S$. Therefore, $c$ is not a limit point of $S$.
>>
>>The sets which contain $d$ are $X$, $\{c,d\}$, $\{a,c,d\}$ and $\{b,c,d,e\}$. The set $\{c,d\}$ also contains $c$ which is a point of $S$. The set $\{a,c,d\}$ contains both $a$ and $c$ which are points of $S$. The set $\{b,c,d,e\}$ contains $b$ and $c$ which are points of $S$. Hence, $d$ is a limit point of $S$ even though $d$ is not in $S$.
>>
>>The sets which contain $e$ are $X$ and $\{b,c,d,e\}$. Both contain multiple elements which belong to $S$ and thus $e$ is a limit point.
>>
>
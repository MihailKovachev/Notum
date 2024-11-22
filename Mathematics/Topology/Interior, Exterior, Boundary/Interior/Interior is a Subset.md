>[!THEOREM] Theorem: Interior is a Subset
>
>Let $(X, \tau)$ be a [topological space](Topological%20Space.md).
>
>The [interior](Interior.md) $\operatorname{int} S$ of each [subset](../../../Set%20Theory/Subset.md) $S \subseteq X$ is a [subset](../../../Set%20Theory/Subset.md) of $S$.
>
>$$\operatorname{int} S \subseteq S$$
>
>>[!PROOF]-
>>
>>Suppose that $\operatorname{int} S$ is not a [subset](../../../Set%20Theory/Subset.md) of $S$. Then there must exist some $s \in \operatorname{int} S$ such that $s \notin S$. Since $s \in \operatorname{int} S$, there must exist some [open set](Open%20Sets/Open%20Subset.md) $O$ such that $s \in O$ and $O \subseteq S$. However, $s \notin S$ implies that $O$ is not a [subset](../../../Set%20Theory/Subset.md) of $S$, which is a contradiction.
>>
>
>^interior-is-a-subset
>
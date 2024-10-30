>[!DEFINITION] Definition: Basis
>
>Let $(S, \tau)$ be a [topological space](Topological%20Space.md).
>
>A **basis** for the [topology](Topology.md) $\tau$ is a [set system](../../Set%20Theory/Set%20Systems/Set%20System.md) $\mathcal{B}$ of [open subsets](../Open%20Subset.md) of $S$ such that every open set can expressed as a [union](../../Set%20Theory/Operations%20with%20Sets/Union.md) of members of $\mathcal{B}$.
>
>>[!THEOREM] Theorem: Topology Generation
>>
>>Let $\mathcal{B}$ be a [basis](Basis.md) for a [topology](Topology.md) $\tau$ on a [set](../../Set%20Theory/Set.md) $S$.
>>
>>A [subset](../../Set%20Theory/Subset.md) $U$ of $S$ is [open](../Open%20Subset.md) if and only if for each $u \in U$ there exists a $B \in \mathcal{B}$ such that $B \subseteq U$ and $u \in B$.
>>
>>
>>>[!PROOF]-
>>>
>>>TODO
>>
>>>[!NOTE]
>>>
>>>This allows us to uniquely determine the topology $\tau$, hence why we often specify topologies by giving a basis for them.
>>>
>>
>
>>[!THEOREM] Theorem
>>
>>Let $S$ be a [non-empty](../../Set%20Theory/The%20Empty%20Set.md) [set](../../Set%20Theory/Set.md) and let $\mathcal{B}$ be a [set system](../../Set%20Theory/Set%20Systems/Set%20System.md) of [subsets](../../Set%20Theory/Subset.md) of $S$.
>>
>>The set system $\mathcal{B}$ is a [basis](Basis.md) for a [topology](Topology.md) on $S$ if and only if
>>
>>- $S = \bigcup \mathcal{B}$ and
>>- for all $B_1,B_2 \in \mathcal{B}$, the [intersection](../../Set%20Theory/Operations%20with%20Sets/Intersection.md) $B_1 \cap B_2$ is a [union](../../Set%20Theory/Operations%20with%20Sets/Union.md) of members of $\mathcal{B}$.
>>
>>>[!PROOF]-
>>>
>>>TODO
>>>
>


>[!THEOREM] 
>
>Let $(S,\tau)$ be a [topological space](Topological%20Space.md).
>
>A [family](../../Set%20Theory/Set%20Systems/Set%20System.md) $\mathcal{B}$ of [open sets](../Open%20Subset.md) is a [basis](Basis.md) for $\tau$ if and only if for each 
>
>[!THEOREM] Theorem: Boundedness of Convergent Sequences
>
>Every [convergent](Sequence%20Convergence.md) [sequence](../Real%20Sequence.md) is [bounded](../../Functions/Function%20Bounds.md).
>
>>[!PROOF]-
>>Let $(a_n)_{n\in \mathbb{N}}$ be a convergent sequence which approaches $L$. Then for every $\varepsilon \gt 0$ there is an integer $N\in\mathbb{N}$ such that
>>
>>$$|a_n - L| \le \varepsilon \qquad \forall n \ge N$$
>>
>>From this it follows that
>>
>>$$|a_n| = |a_n - L + L| \le |a_n - L| + |L| \lt \varepsilon + |L|$$
>>for every $n \ge N$. This means that $a_n$ is bounded by $(-\varepsilon - |L|)$ and $(\varepsilon + |L|)$ for every index $n$ after $N$. It now remains to show that the sequence is also bounded for the indices $1,\cdots,N$. But this is only a finite number of indices and so the smallest and the largest value amidst $a_1, \cdots, a_N$ serve as bounds for the sequence for the indices $1,\cdots, N$.
>>
>>Since the sequence $(a_n)$ is bounded both for indices up until $N$ and after $N$, the sequence must be bounded as a whole.
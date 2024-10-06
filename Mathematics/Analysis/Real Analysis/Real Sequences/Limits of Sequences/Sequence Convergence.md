>[!DEFINITION] Definition: Convergent Sequence
>
>A [sequence](../Real%20Sequence.md) $(a_n)_{n\in \mathbb{N}}$ **approaches** or **converges to** $L \in \mathbb{R}$ if for every $\varepsilon \gt 0$ there is an integer $N \in \mathbb{N}$ (usually dependent on $\varepsilon$) such that
>
>$$|a_n - L| \lt \varepsilon \qquad \forall n \ge N$$
>
>>[!DEFINITION] Definition: Limit of a Sequence
>>The number $L \in \mathbb{R}$ is called the **limit** of the sequence.
>>>[!THEOREM] Theorem: Uniqueness of the Limit
>>>Every convergent sequence has exactly one limit.
>>>
>>>>[!PROOF]-
>>>>Let's assume that a convergent sequence $(a_n)_{n\in \mathbb{N}}$ has two limits $L_1 \ne L_2$. Then for every $\varepsilon \gt 0$ there is an integer $N_1' \in \mathbb{N}$ such that $|a_n - L_1| \lt \varepsilon$ for every $n \ge N_1'$. Since this must by definition be true for every positive real number, there must also be an integer $N_1 \in \mathbb{N}$ for $\frac{\varepsilon}{2}$ such that
>>>>
>>>>$$|a_n - L_1| \lt \frac{\varepsilon}{2} \qquad \forall n \ge N_1$$
>>>>
>>>>Since $L_2$ is also a limit, then for the same $\frac{\varepsilon}{2}$ there must be an integer $N_2 \in \mathbb{N}_1$ such that
>>>>
>>>>$$|a_n - L_2| \lt \frac{\varepsilon}{2} \qquad \forall n \ge N_2$$
>>>>
>>>>It follows then that for all $n \ge \max\{N_1, N_2\}$
>>>>
>>>>$$|L_1 - L_2| = |L_1 - a_n + a_n - L_2|\le |L_1-a_n|+|a_n-L_2| \lt \frac{\varepsilon}{2} + \frac{\varepsilon}{2} = \varepsilon$$
>>>>
>>>>This must be true for every positive real number $\varepsilon$, so $|L_1 - L_2|$ is smaller than every positive number which means it must be 0.
>>>>
>
>>[!NOTATION]
>>$$\lim_{n\to \infty} a_n = L$$

>[!THEOREM] 
>A [real sequence](../Real%20Sequence.md) $(a_n)_{n\in\mathbb{N}}$ converges towards $L \in \mathbb{R}$ if and only if
>
>$$\lim_{n \to \infty} |a_n - L| = 0$$
>
>>[!PROOF]-
>>TODO
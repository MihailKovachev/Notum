>[!ALGORITHM] Algorithm: Calculating the Determinant of a Matrix
>To calculate the [determinant](determinant.md) of a [square matrix](../Square%20Matrix.md) $A\in K^{n\times n}$:
>1. Multipliziere den ersten Eintrag der ersten Zeile $a_{11}$ mit der Determinante Matrix $A_{11}$, also derjenigen Matrix, die man erhält, indem man die erste Zeile und die erste Spalte loswird und den Rest der Spalten zusammen bringt. 
>2. Wiederhole denselben Vorgang mit dem Rest der Einträge in der ersten Zeile, aber alterniere dabei das Vorzeichen vor jedem Eintrag. Also, multipliziere den $j$-ten Eintrag der ersten Zeile $a_{1j}$ mit der Determinante der Matrix $A_{1j}$, also derjenigen Matrix, die man erhält, indem man die erste Zeile und die $j$-te Spalte loswird und den Rest der Spalten zusammen bringt. Falls $1+j$ nicht eben ist, stelle ein Minus voran.
>3. Summiere die Ergebnisse aus den Schritten 1 und 2, um die Determinante zu erhalten.
> 
> > [!NOTE] Tipps
> > 1. Suche nach einer Zeile oder Spalte mit vielen Nullen und vertausche sie mit der ersten.
> > 2. Falls die erste Spalte viele Nullen enthält, berechne die [Determinante des Transponierten](Eigenschaften%20der%20Determinante.md).
> 
> > [!EXAMPLE]- Beispiel
> > Wir betrachten die Matrix
> > $$A = \begin{bmatrix}1 & 2 & 3 & 4 \\ 5 & 6 & 7 & 8 \\ 4 & 3 & 2 & 1 \\ 8 & 7 & 6 & 5\end{bmatrix}$$
> > Laut Algorithmus gilt
> > $$\det(A) = 1\left|\begin{matrix}6 & 7 & 8 \\ 3 & 2 & 1 \\ 7 & 6 & 5\end{matrix}\right| - 2 \left|\begin{matrix}5 & 7 & 8 \\ 4 & 2 & 1 \\ 8 & 6 & 5\end{matrix}\right| + 3 \left|\begin{matrix}5 & 6 & 8 \\ 4 & 3 & 1 \\ 8 & 7 & 5\end{matrix}\right| - 4 \left|\begin{matrix}5 & 6 & 7 \\ 4 & 3 & 2 \\ 8 & 7 & 6\end{matrix}\right|$$
> > 
> > Jetzt müssen wir die Determinanten der $3 \times 3$-Untermatrizen berechnen.
> > 1. Für die erste Untermatrix:
> > $$\begin{vmatrix}6 & 7 & 8 \\3 & 2 & 1 \\7 & 6 & 5\end{vmatrix} = 6\begin{vmatrix} 2 & 1 \\ 6 & 5 \end{vmatrix} - 7\begin{vmatrix} 3 & 1 \\ 7 & 5 \end{vmatrix} + 8\begin{vmatrix} 3 & 2 \\ 7 & 6 \end{vmatrix}$$
> > $$= 6 (2 \cdot 5 - 1 \cdot 6) - 7 (3 \cdot 5 - 1 \cdot 7) + 8 (3 \cdot 6 - 2 \cdot 7)$$
> > $$= 6 (10 - 6) - 7 (15 - 7) + 8 (18 - 14)$$
> > $$= 6 \cdot 4 - 7 \cdot 8 + 8 \cdot 4$$
> > $$= 24 - 56 + 32 = 0$$
> >
> > 2. Für die zweite Untermatrix:
> > $$\begin{vmatrix}5 & 7 & 8 \\4 & 2 & 1 \\8 & 6 & 5 \end{vmatrix} = 5\begin{vmatrix}2 & 1 \\6 & 5\end{vmatrix} - 7\begin{vmatrix}4 & 1 \\8 & 5\end{vmatrix} + 8\begin{vmatrix}4 & 2 \\8 & 6\end{vmatrix}$$
> > $$= 5 (2 \cdot 5 - 1 \cdot 6) - 7 (4 \cdot 5 - 1 \cdot 8) + 8 (4 \cdot 6 - 2 \cdot 8)$$
> > $$= 5 (10 - 6) - 7 (20 - 8) + 8 (24 - 16)$$
> > $$= 5 \cdot 4 - 7 \cdot 12 + 8 \cdot 8$$
> > $$= 20 - 84 + 64 = 0$$
> > 
> > 3. Für die dritte Untermatrix: 
> > $$\begin{vmatrix}5 & 6 & 8 \\4 & 3 & 1 \\8 & 7 & 5\end{vmatrix} = 5\begin{vmatrix}3 & 1 \\7 & 5\end{vmatrix} - 6\begin{vmatrix}4 & 1 \\8 & 5\end{vmatrix} + 8\begin{vmatrix}4 & 3 \\8 & 7\end{vmatrix}$$
> > $$= 5 (3 \cdot 5 - 1 \cdot 7) - 6 (4 \cdot 5 - 1 \cdot 8) + 8 (4 \cdot 7 - 3 \cdot 8)$$
> > $$= 5 (15 - 7) - 6 (20 - 8) + 8 (28 - 24)$$
> > $$= 5 \cdot 8 - 6 \cdot 12 + 8 \cdot 4$$
> > $$= 40 - 72 + 32 = 0$$
> > 
> > 4. Für die vierte Untermatrix:
> > $$\begin{vmatrix}5 & 6 & 7 \\4 & 3 & 2 \\8 & 7 & 6\end{vmatrix} = 5\begin{vmatrix}3 & 2 \\7 & 6\end{vmatrix} - 6\begin{vmatrix}4 & 2 \\8 & 6\end{vmatrix} + 7\begin{vmatrix}4 & 3 \\8 & 7\end{vmatrix}$$
> > $$= 5 (3 \cdot 6 - 2 \cdot 7) - 6 (4 \cdot 6 - 2 \cdot 8) + 7 (4 \cdot 7 - 3 \cdot 8)$$
> > $$= 5 (18 - 14) - 6 (24 - 16) + 7 (28 - 24)$$
> > $$= 5 \cdot 4 - 6 \cdot 8 + 7 \cdot 4$$
> > $$= 20 - 48 + 28 = 0$$
> > 
> > Nun sehen wir, dass alle Determinanten der $3 \times 3$-Untermatrizen null sind. Also ist die Determinante der $4 \times 4$-Matrix:
> > $$\det(A) = 1 \cdot 0 - 2 \cdot 0 + 3 \cdot 0 - 4 \cdot 0 = 0$$

>[!THEOREM] Theorem: Determinant of a $2\times 2$-Matrix
>
>The [determinant](Determinant.md) of every $2\times 2$-[matrix](../Square%20Matrix.md) $A = \begin{bmatrix}a & b \\ c & d\end{bmatrix}$ is given by
>
>$$\det (A) = ad - bc$$
>
>>[!PROOF]-
>>
>>By definition
>>
>>$$\left|\begin{matrix}a & b \\ c & d\end{matrix}\right| = a\det(\begin{bmatrix}d\end{bmatrix}) - b\det(\begin{bmatrix}c\end{bmatrix}) = ad - bc$$
>>

>[!THEOREM] Theorem: Determinant of a $3\times 3$-Matrix
> 
>The [determinant](Determinant.md) of every $3 \times 3$-[matrix](../Square%20Matrix.md) $A = \begin{bmatrix}a & b & c \\ d & e & f \\ g & h & i\end{bmatrix}$ is given by
>
>$$\left|\begin{matrix}a & b & c \\ d & e & f \\ g & h & i\end{matrix}\right| = a(ei - fh) - b(di - fg) + c(dh - ge)$$
>
>>[!PROOF]-
>>
>>By definition
>>
>> $$\left|\begin{matrix}a & b & c \\ d & e & f \\ g & h & i\end{matrix}\right| = a\left|\begin{matrix}e & f \\ h & i\end{matrix}\right| - b \left|\begin{matrix}d & f \\ g & i\end{matrix}\right| + c \left|\begin{matrix}d & e \\ g & h\end{matrix}\right|$$
>> 
>>The $2\times 2$-determinants can be calculated with the previous theorem.
>>

Wir leiten nun einen allgemeinen Lösungsalgorithmus für ein beliebiges Linearses Gleichungssystem der From $A x = b$ mit $A \in K^{n,m}$ und $b \in K^{n}$

1) Wende den Gaußschen Algorithmus (siehe Kapitel 5) an, um die
    erweiterte Koeffizientenmatrix $[A \vdots b] \in K^{n.m+1}$ in TNF zu überführen. 
    D.h. wir erhalten eine Matrix $S \in GL_{n}(K)$ mit $L(A,b) \stackrel{Lem\ VI.3}= L(SA, Sb)$
    und $Sb = b', $SA$ in TNF.
    Notiere mit $j_{1},\dots,j_{r}$ die Pivotspalten von SA mit $r = rang(A)$

2) Wir wissen: $rang(A) = rang(SA)$
    Ist mindestens einer der Einträge $b'_{r-1},\dots,b'_{n}$ ungleich 0, dann folgt $L(A,b) = L(SA,b') = \es$, d.h. das LGS $Ax = b$ hat keine Lsg.

3) Es gelte nun $b'_{r+1} = \dots = b'_{n}$
    (-> Es gibt mindestens eine Lsg.)
    a) Ist r = m, dann ist (4) von der Form
    $$SA = \begin{bmatrix}
I_{r} \\ \dots \\ 0_{n-r,r}
\end{bmatrix} \begin{bmatrix}
x_{1} \\ \vdots \\ x_{r}
\end{bmatrix} = b' = \begin{bmatrix}
b'_{1} \\ \vdots \\ b'_{r} \\ 0 \\ \vdots \\ 0
\end{bmatrix}$$
-> $x_{1} = b'_{1}, \dots, x_{r} = b'_{r}$

Somit ist $x = [b_{1}',\dots,b'_{r}]$ die eindeutige Lösung
$\RA L(A,b) = \{ [b'_{1},\dots,b'_{r}] \}$

3) b) Ist r < m, dann betrachte die Permutationsmatrix 
    $P^{T} \in K^{m,m}$ $P^{T}=[e_{j_{1}}, \dots , e_{j_{r}}, e_{1},\dots,e_{j_{1}-1}, e_{j_{1}+1},\dots,e_{j_{2}-1}, e_{j_{2}+1},\dots,e_{m}]$
    Die Matrix $P^{T}$ wird von recchts an SA multipliziert. Dies hat den Effekt, dass die Pivotspalten von SA der Reihe nach vorne in $SAP^{T}$ stehen.
    Dies liefert $$A' = SAP^{T} = \begin{bmatrix}
    I_{r} & \vdots & A'_{1,2} \\
    \dots & \dots & \dots \\
    0_{n-r,r} & \vdots & 0_{n-r,m-r} 
    \end{bmatrix}$$
	wobei $A'_{1,2} \in K^{r,m-r}$
	Da für alle Permutationsmatrizen $P^{-1} = P^{T} \RA P^{T}P=I_{m}$
	$\RA SAx = SAP^{T} Px = b' = Sb$
	$\RA L(A',b')$
	
	Betrachte die eweiterte Koeffizientenmatrix $[A'\ \vdots\ b'] \in K^{n,m+1}$
	Für diese gilt $rang([A'\ \vdots\ b']) = rang([SAP^{T}\ \vdots\ Sb])$
    $$=rang(S[A \ \vdots\ b] \begin{bmatrix}
	P^{T} & \vdots  & 0 \\
	\dots & + & \dots \\
	0 & \vdots & 1
    \end{bmatrix})$$
    $= rang([A\ \vdots\ b])$
    Weiter wissen wir $rang(A) = rang(A') \leq rang([A'\ \vdots\ b'])$
    $= rang([A\ \vdots\ b])$
    
    Wegen $b'_{r+1}= \dots = b'_{n} = 0$ folgt $rang(A') = rang([A'\ \vdots\ b'])$
    und somit folgt $rang(A) = rang([A\ \vdots\ b])$
    
    In diesem Fall kann das LGS also gelöst werden. 
    Wir erhalten $$\begin{bmatrix}
	y_{1} \\
	\vdots \\
	y_{r}
    \end{bmatrix} = \begin{bmatrix} \\
    b'_{1} \\
	\vdots \\
	b'_{r}
    \end{bmatrix} - A'_{1,2} \begin{bmatrix}
	y_{r+1} \\
	\vdots \\
	y_{m}
    \end{bmatrix}$$
    Daraus kann man unmittelbar eine spezielle Lösung von $A'y=b'$ ablesen. Dazu setze die freien Varaiblen $y_{r+1},\dots,y_{m}$ auf 0.
    $\RA y' = [b'_{1},\dots,b'_{r}, 0,\dots,0]^{T}\in K^{m}$
    (-> $x' = P^{T}y'$ ist dann eine Lösung von $Ax = b$)
    

4) Bestimmung der Lösungmeng
    Um alle Lösungen des homogenen Problems $L(A',0)$ zu bekommen, betrachte die Mengee
    $L(A',0) = \{ [y_{1},\dots,y_{m}]^{T} \in K^{m} \mid y_{r+1},\dots,y_{m}\in K\ beliebig$
    $und\ [y_{1},\dots,y_{r}]^{T}=0=A'_{1,2}[y_{r+1},\dots,y_{m}]^{T} \}$
    Durch die Wahl der freien Variablen $y_{r+1},\dots,y_{m}$ können so also alle Lösungen von $A'y=b'$ angegeben werden. Mit $x = P^{T}y$ für $y \in L(A',b')$ erhalten wir dann Lösungen von $Ax = b$
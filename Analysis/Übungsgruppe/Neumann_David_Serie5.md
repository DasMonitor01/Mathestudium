# Aufgabe 1
Geg:
Sei $(a_n)_{n \in \N}$ eine Folge

a)
Z.z: 
$\limin a_n = a \Rightarrow \Limin{k} a_{(n_k)}= a$ 

Sei $\limin a_n = a$ 
$\Rightarrow \forall \epsilon > 0 \E N \in \N: |a_n - a| < \epsilon \F n \geq N$ 

Neu zu zeigen:
$\forall \epsilon > 0 \E N_0 \in \N: |a_{(n_k)}- a|< \epsilon \F k \geq N_0$ 

Mit der Definition von Teilfolgen ist folgendes möglich:
Wähle $N_0$ so, dass $n_{N_0} > N$ gilt. 
(Teilfolgenglieder müssen streng monoton steigend sein, also finden wir immer ein Glied so dass dies gilt.
$n_{N_0}\Rightarrow |a_{m} - a|< \epsilon \F m \geq N_0$ (nach der Vorraussetzung)
$n_{N_0} > N \Rightarrow n_{k} > N \F k \geq N_0$ 
(wieder nach Teilfolgendefinition (streng monoton steigend))

$\Rightarrow \forall \epsilon > 0 \E N_0 : |a_{n_k} - a| < \epsilon \F k \geq N_0$ 
$\blacksquare$ 
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


b)
Zu zeigen:
$\Limin{k} a_{2k} = a \land \Limin{k} a_{3k}= b \Rightarrow a = b$

Beweis:
Sei $\Limin k a_{2k} = a$ 
und $\Limin k a_{3k} = b$ 

Sei $a_{2k} = a_{b_k}$
und $a_{3k} = a_{c_k}$

Betrachte $a_{6k}$
Es gilt $a_{6k} = a_{b_{3k}}$ ($6k = 2 \cdot 3k$) und folglich ist $a_{6k}$ eine Teilfolge von $a_{2k}$ 
nach a) gilt somit:
$\Limin k a_{6k} = a$ 

Es gilt außerdem $a_{6k} = a_{c_{2k}}$ ($6k = 3 \cdot 2k$) und folglich ist $a_{6k}$ eine Teilfolge von $a_{3k}$.
nach a) gilt somit:
$\Limin k a_{6k} = b$ 

Es gilt folglich (mit der eindeutigkeit des Grenzwertes)
$a = \Limin k a_{6k} = b$
$\Rightarrow a = b$ 
$\blacksquare$ 
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

c) 
Z.z.:
$\Limin k a_{2k} = a = \Limin k a_{2k+1} \Rightarrow \limin a_n$ 

Also:
$\forall \epsilon > 0 \E N \in \N: |a_n - a|< \epsilon \F n \geq N$ 

Sei $a_{2k} = a_{b_k}$ und $a_{2k+1} = a_{c_k}$ .

Da $b_{k\in \N} := 2k$ die Menge aller geraden Zahlen größergleich 2 und
$c_{k \in \N} := 2k +1$ die Menge aller ungeraden Zahlen größergleich 2 dastellen, folgt:
$\forall n \geq 2 \Rightarrow a_n \in a_{2k} \lor a_n \in a_{2k+1}$  
(jedes Glied von $a_n$ liegt in $a_{2k}$ oder in $a_{2k+1}$)

Sei $\Limin k a_{2k} = a = \Limin k a_{2k +1}$ 
$\Rightarrow \forall \epsilon > 0 \E N_1,N_2 \in \N : \biggl\{ \begin{matrix} {|a_{2k} - a| < \epsilon \F k \geq N_1} \\ {|a_{2k+1} - a| < \epsilon \F k \geq N_2} \end{matrix}$ 

$\Rightarrow$ Für $N = 2 \max(N_1, N_2) + 1$ (also $a_N = a_{2N_1 +1}$ oder $a_N = a_{2N_2 + 1}$) folgt:
$|a_n - a| < \epsilon \F n \geq N$
$\Rightarrow \F \epsilon > 0 \E N \in \N: |a_n - a|< \epsilon \F n \geq N$ 
$\Rightarrow \limin a_n = a$
$\blacksquare$ 
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

# Aufgabe 2
a)
Geg:
$a_n = \frac{n-(-1)^n}{4 + (-1)^n}$

Errinerung aus 1:
Die Folgen $a_{2k}$ und $a_{2k+1}$ bilden zusammen fast alle (also alle bis auf endlich viele) Glieder der Folge $a_n$
Stellen diese beiden Teilfolgen also jeweils einen Häufungspunkt da, so sind dies die einzigen beiden Häufungspunkte

Häfungspunkte:
Betrachte $a_{2k} = \frac{2k - (-1)^{2k}}{4 + (-1)^{2k} \cdot 2k}$ 
Da $(-1)^n = 1 \F n: 2 \mid n$ und $2 \mid 2k \F k \in \N$ gilt, folgt:
$a_{2k} = \frac{2k - 1}{4 + 2k} = \frac{2k -1}{2k + 4}$

mit einer (sehr simplen) Polynomdivision erhalten wir die alternative Form
$a_{2k} = 1 - \frac{5}{2k + 4}$ 
(gleichheit lässt sich leicht durch Rückmultiplizieren prüfen)
und folglich gilt 
$\Limin k a_{2k} = \Limin k 1 - \frac{5}{2k + 4} =  \Limin k 1 - \Limin k \frac{5}{2k + 4}$
$= 1 - 0 = 1$ 
$\Rightarrow$ 1 ist HP
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


Betrachte $a_{2k+1} = \frac{2k+1 - (-1)^{2k + 1}}{4 + (-1)^{2k+1}\cdot (2k + 1)}$ 
Da $(-1)^n = -1 \F n : 2 \not \mid n$ und $2 \not \mid 2k + 1 \F k \in \N$ gilt, folgt
$a_{2k+1} = \frac{2k + 1 - 1}{4 - 2k - 1} = \frac{2k}{-2k + 3}$ 

erneut können wir eine (wieder sehr leichte) Polynomdivision durchführen, um auf die Form
$a_{2k + 1} = -1 + \frac{3}{-2k + 3}$ zu kommen

und folglich gilt:

$\Limin k a_{2k+1} = \Limin k -1 + \frac{3}{-2k + 3} = \Limin k -1 + \Limin k \frac{3}{-2k + 3}$
$= -1 + 0 = -1$
$\Rightarrow -1$ ist HP von $a_n$

Folglich sind die Häfungspunkte der Folge $1$ und $-1$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


b) 
Geg:
$b_n = 2 \cdot (-1)^{(\frac{n(n+1)}{2})}+ 4 \cdot (-1)^n$

Wie in a) können wir auch $b_n$ in eine Gruppe von Teilfolgen aufteilen. 
In diesem Fall bietet sich die Aufspaltung in 4 Teilfolgen 
(in die Vier Restklassen von n mod 4) an:
$b_{4k}$
$b_{4k +1}$
$b_{4k+2}$
$b_{4k+3}$
Erneut bilden diese 4 Teilfolgen zusammen die Gesammte Folge $b_n$ wieder, es liegen also alle Glieder von $b_n$ in (genau) einer dieser Teilfolgen.

1.: $b_{4k}$
$b_{4k} = 2 \cdot (-1)^{(\frac{4k (4k + 1)}{2})} + 4 \cdot (-1)^{4k}$ 
$= 2\cdot (-1)^{2k (4k + 1)} + 4 \cdot (-1)^{2\cdot(2k)}$ 
$= 2 \cdot (-1)^{2\cdot (k(4k+1))} + 4 \cdot (-1)^{2 \cdot (2k)}$
Mit $(-1)^{2m} = 1 \F m \in \N$ folgt:
$b_{4k} = 2 \cdot 1 + 4 \cdot 1$
$= 2 + 4$
$= 6$ (für alle $k \in \N$)

$\Rightarrow b_{4k} = 6 \F k \in \N$
$\Rightarrow \Limin k b_{4k} = 6$
$\Rightarrow$ 6 ist HP von $b_n$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

2.: $b_{4k+1}$
$b_{4k+1} = 2 \cdot (-1)^{(\frac{(4k+1)(4k+2)}{2})} + 4 \cdot (-1)^{4k+1}$
$= 2 \cdot (-1)^{(\frac{(2(4k+1)(2k+1))}{2})} + 4 \cdot (-1)^{2(2k)+1}$
$= 2 \cdot (-1)^{(4k+1)(2k+1)} + 4 \cdot (-1)^{2(2k)+1}$
$= 2 \cdot (-1)^{8k^2 + 6k + 1} + 4 \cdot (-1)^{2(2k)+1}$
$= 2 \cdot (-1)^{2(4k^2+3k)+1} + 4 \cdot (-1)^{2(2k)+1}$
Mit $(-1)^{2m+1} \F m \in \N$ folgt:
$b_{4k+1} = 2 \cdot (-1) + 4 \cdot (-1)$ 
$= -2 - 4$
$= - 6$ (für alle $k \in \N$)

$\Rightarrow b_{4k+1} = -6 \F k \in \N$
$\Rightarrow \Limin k b_{4k+1} = -6$

$\Rightarrow$ -6 ist HP von $b_n$ 
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

3.: $b_{4k+2}$
$b_{4k+2} = 2 \cdot (-1)^{(\frac{(4k+2)(4k+3)}{2})} + 4 \cdot (-1)^{4k+2}$
$= 2 \cdot (-1)^{(\frac{2(2k+1)(4k+3)}{2})}+4 \cdot (-1)^{2(2k+1)}$
Mit $(-1)^{2m} = 1 \F m \in \N$ folgt:
$b_{4k+2} = 2 \cdot (-1)^{(2k+1)(4k+3)}+ 4 \cdot 1$
$= 2 \cdot (-1)^{8k^2 + 10k + 3} + 4$ 
$= 2 \cdot (-1)^{8k^2 + 10k + 2 + 1}+ 4$
$= 2 \cdot (-1)^{2(4k^2+5k + 1) + 1} + 4$
Mit $(-1)^{2m+1} = -1 \F m \in \N$ folgt:
$b_{4k+2} = 2 \cdot (-1) + 4$
$= -2 + 4$
$= 2$ (für alle $k \in \N$)

$\Rightarrow b_{4k+2} = 2 \F k \in \N$
$\Rightarrow \Limin k b_{4k+2} = 2$ 
$\Rightarrow$ 2 ist HP von $b_n$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


4.: $b_{4k+3}$
$b_{4k+3} = 2 \cdot (-1)^{(\frac{(4k+3)(4k+4)}{2})} + 4 \cdot (-1)^{4k+3}$
$= 2 \cdot (-1)^{(\frac{2(4k+3)(2k+2)}{2})}+4 \cdot (-1)^{4k + 2 +1}$
$= 2 \cdot (-1)^{(4k+3)(2k+2)}+4 \cdot (-1)^{2(2k+1)+1}$
Mit $(-1)^{2m + 1} = -1 \F m \in \N$ folgt:
$b_{4k+3} = 2 \cdot (-1)^{2(4k+3)(k+1)}+4 \cdot (-1)$
$= 2 \cdot (-1)^{2((4k+3)(k+1))} - 4$
Mit $(-1)^{2m} = 1 \F m \in \N$ folgt:
$b_{4k+3} = 2 \cdot 1 -4$
$= 2 - 4$
$= -2$ (für alle $k \in \N$)

$\Rightarrow b_{4k+3} = -2 \F k \in \N$
$\Rightarrow \Limin k b_{4k+3} = -2$
$\Rightarrow$ -2 ist HP von $b_n$ 

$\Rightarrow$ Die vier Teilfolgen decken alle Häufungspunkte von $b_n$ ab, die Häufungspunkte von $b_n$ sind also: $\set{-6, -2, 2, 6}$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


# Aufgabe 3
Sei $(a_n)_{n \in \N}$ eine Folge
Zu zeigen:
a Hochpunkt von $a_n$
$\Leftrightarrow \forall \epsilon > 0 \F N \in \N \E n \geq N: |a_n -a| < \epsilon$

"$\Rightarrow$":
Sei a Hochpunkt von $a_n$
$\Rightarrow \exists a_{n_k}:\Limin k a_{n_k} = a$
Sei $(n_k)_{k \in \N}$ eine Folge mit dieser Eigenschaft
$\Rightarrow \forall \epsilon > 0 \E N_0 \in \N : |a_{n_k}-a| < \epsilon \F k \geq N_0$ 

Wir finden also für jedes $\epsilon$ ein $N_0$, so dass für alle! $k \geq N_0$ gilt, $|a_{n_k} - a| < \epsilon$ 

Damit können wir jedoch sagen: 
Sei $\epsilon > 0$
Für $N \in \N$ beliebig finden wir $M \in \N$ mit $M > N$.
Nach der Definition einer Teilfolge muss außerdem der Index einer Teilfolge streng monoton wachsend und unbeschränkt sein, es gilt also:
$\forall m \in \N \E k \in \N: n_k > m$ 
$\Rightarrow \exists N_2 \in \N: n_k > N \F k \geq N_2$ 

$\Rightarrow \forall \epsilon > 0 \F N \in \N \E k \geq \max{N_1, N_2} \geq N : |a_{n_k} - a| < \epsilon$
$\Rightarrow \forall \epsilon > 0 \F N \in \N \E n \geq N: |a_n - a| < \epsilon$
$\checkmark$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

"$\Leftarrow$"
Sei $(a_n)_{n \in \N}$ eine Folge mit der Eigenschaft
$\forall \epsilon > 0 \F N \in \N \E n \geq N : |a_n -a| < \epsilon$

Sei $(h_n)_{n\in \N}$ eine Folge mit den Folgenden eigenschaften:
$h_1 = m$
$h_k = m :( m > h_{k-1} \land |a_m - a | \leq \frac{|a_{h_{k-1}} - a|}{2})$  
(funktioniert, da wir für jedes $N \geq h_{k-1}$ ein m finden, sodass $m \geq N$ finden, sodass $|a_m -a| < \epsilon \F \epsilon > 0$ und insbesondere auch für $\epsilon = \frac{|a_{h_{k-1}} - a|}{2}$)
Somit wird $|a_{h_k} -a|$ beliebig klein für große k, da für ein beliebiges $h_k$ immer gelten muss: $h_k = m : (m > k_{k-1}) \land |a_{h_{k}} - a| \leq \frac{|a_{h_1} - a|}{2^k}$ 
und dies offensichtlich für k gegen unendlich gegen Null konvergiert 

$\Rightarrow a_{h_{k}}$ hat somit die Eigenschaft, dass wir für alle $\epsilon >0$ ein $K \in \N$ finden, sodass $|a_{h_{k}} - a|< \epsilon \F k \geq K$
$\Rightarrow \Limin k a_{h_{k}} = a$ 
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


# Aufgabe 4
a)
Z.z:
Es existiert eine Folge $(a_n)_{n \in \N}$ mit genau K Häufungspunkten 
(ich nehme hier mal an, das auch $K \in \N$ gelten soll, da ein halber Häfungspunkt nicht so viel Sinn ergeben würde :) (einziger sonderfall ist dann vielleicht noch 0 HP, der wird unten nochmal kurz behandelt))

Betrachte die Folge $(a_n) := n \mod K$ mit Parameter K
Wir können diese Folge in K Teilfolgen (die K Restklassen von $n \mod K$) unterteilen.
Die hierbei entstehenden Teilfolgen werden im Folgenden mit dem zusätzlichen Parameter t als Folgenschaar wie folgt notiert werden:$(a_{Km+t})_{m\in \N} = Km+t \mod K$ wobei $0 \leq t < K$ gilt.
Die K Teilfolgen bilden zusammen wieder $a_n$, d.h. alle Glieder von $a_n$ sind Element von (genau) einer Teilfolge $(a_{Km+t})_{m \in \N}: 0 \leq t < K$ 

Nach dieser Definition der Teilfolgen und der Definition des Modulo Operators (Restoperator der Division) folgt aber direkt:
$(a_{Km+t})_{m\in \N} = t \F m \in \N$ für alle $t \in \N: 0 \leq t < K$
Folglich gilt für alle $t: 0 \leq t < K$:
$\Limin m a_{Km+t} = t$ 
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

Foglich besitzt $a_n$ die Häufungspunkte $\set{0,1,...,K-1}$
und dies sind alle Häufungspunkte von $a_n$.
$a_n$ besitzt also genau K häfungspunkte.

Folglich existiert eine Folge $(a_n)_{n\in \N}$ mit genau K Häufungspunkten wobei $K \in \N$ gilt.
$\blacksquare$
(Zusatz: Für $a_n = n$ folgt aus 
der strengen Monotonie (die offensichtlich ist (n < n+1 gilt immer in $\R$) 
und der Unbeschränktheit (Für alle n gilt $a_{n+1} > n$ folglich kann keine Schranke existieren)
direkt, dass es keine Konvergente Teilfolge geben kann, 
da auch die Glieder der Teilfolge diese Eigenschaften zwingend besitzen müssen,
und somit auch alle Teilfolgen von $a_n$ gegen Unendlich divergieren. 
Folglich hat diese Folge 0 Häufungspunkte, es existiert somit sogar eine Folge mit genau $K\in \N_0$ Häfungspunkten)
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


b)
Z.z:
Es existiert eine Folge $(a_n)_{n\in \N}$ mit jedem $k \in \N$ als Häfungspunkt.

Beweis:
Wir definieren zunächst die Hilfsfolge
$h_n := \Sum_{k=1}^n k$ 

und die Hilfsmenge $H := \set{x \mid x \in h_n}$ 
(H ist also: $\set{1,3,6,10,15,21,28,...}$)

Nun definieren wir unsere Folge mit der gewünschten Eigenschaft:
Sei $(a_n)_{n\in \N}$ eine Folge mit:
$a_n := \biggl \{ \begin{matrix} {1\ falls\ n \in H} \\ {a_{n-1} + 1\ sonst} \end{matrix}$ 

Um die Idee der Folge zu verdeutlichen, ist es Sinnvoll sich das ganze in einer Tabelle anzusehen:

n | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 | 12 | 13 | 14 | 15 | ...
--- | --- | --- |  --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | ---
$a_n$| 1 | 2 | 1 | 2 | 3 | 1 | 2 | 3 | 4 | 1 | 2 | 3 | 4 | 5 | 1 | ...

Diese Folge besitzt offensichtlich jede natürliche Zahl unendlich oft als Teilglieder. Dies wird im Folgenden nochmal etwas verdeutlicht.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

Folgendes wird festgehalten:
Jede natürliche Zahl kommt ab einem bestimmten Startwert unendlich oft in der Folge vor. Diese Startwerte liegen als Glieder dem Anschein nach immer genau einen Index vor einem Index der Glied von $h_n$ ist. Dies liegt daran, das nach jedem Glied von $h_n$ als Index die Folge eine natürliche Zahl mehr in dem Durchlauf (also dem Bereich zwischen zwei Einsen) mitnimmt. Da $h_n$ bei 1 startet und somit mit jedem Glied von $h_n$ im Index eine weitere natürliche Zahl hinzukommt, gilt sogar, das jede natürliche Zahl k in $a_n$ das erste mal beim Index $h_k -1$ (= $(\Sum_{i = 1}^k i) - 1$) vorkommt. Ab da ist der Abstand jeden weiteren Gliedes das diese Zahl darstellt zu einem Index von $a_n$ dann immer $k-1$, da (k - 1) mal 1 zu eins addiert werden muss, um bis zu k (also $1 + (k -1) \cdot 1 = k$) zu kommen. 
Damit liegen diese Glieder dann immer genau beim Index $h_n + k - 1$ 

Damit können wir nun die folgenden abgewandelte Hilfsfolge definieren (bei der k ein Parameter der natürlichen Zahlen ist):
$h^k_{n} := (\Sum_{i=1}^n i) + k -1$ wobei $n \in \set{k, k + 1, k + 2, ...}$ 

Nach dieser Definition der Folge $h_n^k$ mit k als Paramter, folgt nach dem was oben beschrieben wurde nun offensichtlich, dass
$a_{h_m^k} = k \F m \in \N$ gelten muss.
Folglich gilt dann
$\Limin m a_{h^k_m} = k$ 

Da k eine hierbei eine beliebige natürliche Zahl sein kann, haben wir für jedes $k \in \N$ eine Teilfolge von $a_n$ gefunden, die gegen k Konvergiert, folglich ist jede natürliche Zahl ein Häufungspunkt von $a_n$.
Es existiert somit eine Folge mit jeder natürlichen Zahl als Häfungspunkt.
$\blacksquare$ 
A3.4:
a)
z.z.: 
$\P(M) \cap \P(N) = \P(M \cap N)$
$\Leftrightarrow (\P(M) \cap \P(N) \subseteq \P(M \cap N)) \land (\P(M \cap N) \subseteq \P(M) \cap \P(N))$

$\P(M) \cap \P(N) \subseteq \P(M \cap N)$:
$\forall X \in \P(M) \cap \P(N) \Rightarrow X \in \P(M) \land X \in \P(N)$
$\Rightarrow X \subseteq M \land X \subseteq N$
$\Rightarrow X \subseteq M\cap N$
$\Rightarrow X \in \P(M\cap N) \F X \in \P(M) \cap \P(N)$
$\Rightarrow \P(M) \cap \P(N) \subseteq \P(M \cap N)$


$\P(M \cap N) \subseteq \P(M) \cap \P(N)$
$\forall X \in \P(M \cap N) \Rightarrow X \subseteq M \cap N$
$\Rightarrow X \subseteq M \land X \subseteq N$
$\Rightarrow X \in \P(M) \land X \in \P(N)$
$\Rightarrow X \in \P(M) \cap \P(N) \F X \in \P(M \cap N)$
$\Rightarrow \P(M \cap N) \subseteq \P(M) \cap \P(N)$


b)
z.z. $\P(M) \cup \P(N) \subseteq \P(M\cup N)$

$\forall X \in \P(M) \cup \P(N) \Rightarrow X \subseteq M \lor X \subseteq N$
$\Rightarrow X \subseteq M\cup N$
$\Rightarrow \P(M) \cup \P(N) \subseteq \P(M \cup N)$
$\blacksquare$

Bsp:
$M = \set{1}$, $N = \set{2}$ $\Rightarrow M \cup N = \set{1,2}$
$\Rightarrow$
$\P(M) = \set{\es, \set{1}}$, $\P(N) = \set{\es, \set{2}}$ $\Rightarrow \P(M) \cup \P(N) = \set{\es, \set{1}, \set{2}}$
$\P(M \cup N) = \set{\es, \set{1}, \set{2}, \set{1,2}} \neq \P(M) \cup P(N)$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


A3.5
Erinnerung:
Sei $f: M \to M$, $A \subseteq M$
$\invers f(A) := \set{x \mid x \in X \land f(x) \in A}$

Geg.:
$f: M \to M$; $M_1,M_2, D_1, D_2 \subseteq M$ 

a)
Beh.: $\invers f(M_1 \cup M_2) = \invers f(M_1) \cup \invers f(M_2)$

Beweis:
$\inv f(M_1 \cup M_2)$ 
$:= \set{x \mid x \in M \land f(x) \in (M_1 \cup M_2)}$
$= \set{x \mid x \in M \land f(x) \in \set{y \mid y \in M_1 \lor y \in M_2}}$
$= \set{x \mid x \in M \land (f(x) \in M_1 \lor f(x) \in M_2)}$
$= \set{x \mid (x \in M \land f(x) \in M_1) \lor (x \in M \land f(x) \in M_2)}$ (Logisches Distributivgesetz)
$= \inv f(M_1) \cup \inv f(M_2)$
$\blacksquare$


b)
Beh.: $\inv f(M_1 \cap M_2) = \inv f(M_1) \cap \inv f(M_2)$

Beweis:
$\inv f(M_1 \cap M_2)$
$:= \set{x \mid x \in M \land f(x) \in (M_1 \cap M_2)}$
$= \set{x \mid x \in M \land f(x) \in \set{y \mid y \in M_1 \land y \in M_2}}$
$= \set{x \mid (x \in M \land x \in M) \land (f(x) \in M_1 \land f(x) \in M_2)}$
$= \set{x \mid (x \in M \land f(x) \in M_1) \land (x \in M \land f(x) \in M_2)}$
$= \inv f(M_1) \cap \inv f(M_2)$
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


c)
Beh.: $f(D_1 \cap D_2) = f(D_1) \cap f(D_2)$

Falsch:
Wiederlegung durch Beispiel:

Sei $f: \R \to \R, x \onto x^2$
$\Rightarrow f(\set{3}) = \set{9}$, $f(\set{-3}) = \set{9}$
$\Rightarrow f(\set{3}) \cap f(\set{-3}) = \set{9}$
$\set{3} \cap \set {-3} = \es$ $\Rightarrow f(\set{3} \cap \set{-3}) = f(\es) = \es \neq \set{9}$
$\blacksquare$


d)
Beh.: $f(\inv f(M_1)) = M_1$

Falsch:
Wiederlegung durch Beispiel:

Sei $f: \set{0,1} \to \set{0, 1}, x \onto 0$

$f(\inv f(\set{1})) = f(\es) = \es \neq \set{1}$
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


A3.6
a)
$f: \Z \to \Z, x \onto 2x + 3$
injektiv:
z.z.:
$\forall x_1,x_2 \in \Z: f(x_1) = f(x_2) \Rightarrow x_1 = x_2$

Seien $x_1, x_2 \in \Z : f(x_1) = f(x_2)$
$\Rightarrow 2x_1 +3 = 2x_2 + 3$
$\stackrel{-3, :2}\Leftrightarrow x_1 = x_2$
$\blacksquare$

nicht surjektiv:
f surjektiv $\Leftrightarrow \forall y \in \Z \E x \in \Z: y=f(x)$

Gegenbeispiel:
Sei y = 0
$\Rightarrow 0 = 2x +3$
$\stackrel{-3, :2}\Leftrightarrow x = \frac{-3}{2}$ 
$\Rightarrow x \nin \Z$
$\Rightarrow$ f ist nicht surjektiv

$g: \Q \to \Q, x \onto 2x + 3$

Surjektiv:
z.z.:
$\forall y \in \Q \E x \in \Q: y = f(x)$

Sei $y \in \Q$
$\Rightarrow y = 2x +3$
$\stackrel{-3, :2}\Leftrightarrow x = \frac{y- 3}{2}$
$\Rightarrow x \in \Q$
$\Rightarrow$ g ist surjektiv
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


b)
Merke folgendes:
Seien A und B Mengen und sortiert nach der Relation: $|A| \geq |B|$
(man kann die Mengen immer nach der größe Sortieren)
Direkte folge:
Wenn $|A| \geq |B|$ dann gilt nie $A \subset B$ (A kann keine echte Teilmenge von B sein, wenn es mehr oder gleich viele Elemente hat)

Dann gilt folgendes:

$| A \cup B | \geq |A| \geq |B|$ 
(die Vereinigung hat mindestens so viele Elemente wie A)

und insbesondere:

$|A \cup B| = |A| \geq |B|$ wenn $B \subseteq A$ 
(ist B eine Teilmenge von A, liefert die Vereinigung A(alle Elemente von B liegen auch in A), und somit besitzt die Vereinigung so viele Elemente wie A)

und

$|A \cup B| \geq |A| + 2 > |A| \geq |B|$ wenn $B \not \subseteq A$ 
(ist B keine Teilmenge von A, gibt es mindestens ein Element in B das nicht in A ist, die Vereinigung muss somit mehr Elemente als A haben. Da außerdem gilt $A \not \subset B$ folgt, dass es mindestens ein Element in A geben muss, dass nicht in B liegt. Die Vereinigung ist somit mindestens um zwei größer als $|A|$)

Außerdem gilt:

$|A \cap B| \leq |B| \leq |A|$ 
(der Schnitt hat höchstens so viele Elemente wie B)

und insbesondere:

$|A \cap B| = |B| \leq |A|$ wenn $B \subseteq A$ 
(ist B eine Teilmenge von A, dann liefert der Schnitt B, und somit genauso viele Elemente wie in B sind)

und

$|A \cap B| \leq |B-2| < |B| \leq |A|$ wenn $B \not \subseteq A$ 
(ist B keine Teilmenge von A, so gibt es mindestens ein Element in B, dass nicht in A liegt, und somit auch nicht im Schnitt mit dabei ist. Da außerdem gilt, $A \not \subset B$ folgt, dass es mindestens ein Element in A geben muss, dass nicht in B liegt, und somit im Schnitt fehlt. Der Schnitt ist also folglich mindestens 2 kleiner als $|B|$)


geg:
$|A \cap B| = 6$, $|A \cup B| = 8$.
Man kann die Mengen wieder der größe nach Ordnen, d.h.
$|A| \geq |B|$
$\Rightarrow 6 \leq |B| \leq |A| \leq 8$

Angenommen $|B|>6$ Elemente:
Wenn $B \subseteq A$, dann gilt wie oben beschrieben $|A \cap B| = |B| > 6$ $\rightarrow \leftarrow$

Wenn $B \not \subseteq A$ dann gilt wie oben beschrieben $|A \cup B| \geq |A| + 2$
da aber $|A| \geq |B| > 6$ gilt, würde folgen, dass $|A \cup B| > 8$ $\contrana$

Folglich muss gelten: $|B| = 6$

Somit gilt für $|A|$:
Wenn $B \subseteq A$ dann gilt wie oben beschrieben $|A\cap B| = |A|$
folglich muss $|A| = 8$ gelten

Wenn $B \not \subseteq A$, dann gilt wie oben beschrieben: $|A \cap B| \leq |B| - 2$
und somit wäre $|A \cap B| < 6$

Es folgt, dass gelten muss:
$|A| = 8$ und $|B| = 6$ 
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


A3.7)
$M = \set{1,2,3,4,...,10}$

$f: M \to M, n \onto 5n \mod 11$

$\Rightarrow$ Folgende Werte gelten:

n | f(n) 
--- | ---
1 | 5
2 | 10
3 | 4
4 | 9
5 | 3
6 | 8
7 | 2
8 | 7
9 | 1
10 | 6

Durch ansehen der Tabelle erkennt man, dass es keine f(n) gibt, auf dass mehrfach abgebildet wird. Es folgt somit das f(n) = f(n') $\Rightarrow$ n = n'. f ist somit injektiv
Außerdem wird auf jeden Wert von M abgebildet, zu jedem f(n) findet man also mindestens ein n mit f(n) = n. f ist somit surjektiv.
Somit ist f bijektiv, und damit existiert die Umkehrfunktion $\inv f$
$\blacksquare$


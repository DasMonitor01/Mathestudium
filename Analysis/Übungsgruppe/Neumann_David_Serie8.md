# Aufgabe 1
Sei $F := \{ f:\N \to \{ 0,1 \} \}$
Zu zeigen:
F ist überabzählbar.

#### Beweis:
Angenommen F wäre abzählbar.
Dann existiert $\varphi: \N \to F$, dass jeder Funktion $f_{n}$ eine Zahl n zuweist, die dieser Funktion eindeutig identifiziert.

Wir können dies mit einer Liste Ausdrücken, wobei die Spalten die natürliche Zahl ist, die der Funktion zugeordnet wurde, und die Zeilen die Verschiedenen Zuordnungen der Funktionen:

$n \in\N$ | $f_{n}(1)$ | $f_{n}(2)$ | $f_{n}(3)$ | $f_{n}(4)$ | $f_{n}(5)$ | ... 
--- | --- | --- | --- | --- | --- | --- 
1 | 1 | 0 | 1 | 1 | 0 | ...
2 | 0 | 1 | 0 | 0 | 1 | ...
3 | 0 | 1 | 1 | 1 | 0 | ...
4 | 1 | 1 | 1 | 1 | 0 | ...
5 | 1 | 0 | 0 | 0 | 0 | ...
...

Nun können wir aber eine neue Funktion finden, die in der Tabelle nicht vorkommt:
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

Sei $f_{x}: \N \to \{  0,1\} : n \onto \biggl \{ \begin{matrix} 1 : f_{n}(n)=0 \\ 0: f_{n}(n)=1\end{matrix}$ 

Offensichtlich kann diesem f kein $k \in \N$ zugewiesen werden, da sonst gelten müsste: 
$f_{x} = f_{k}$ aber damit müsste $f_{k}(k)$ der Wert 1 zugewiesen, genau dann, wenn $f_{k}(k) = 0$ und der Wert 0 genau dann, wenn $f_{k}(k)=1$ also $1 = f_{k}(k) = 0$

Folglich existiert eine Funktion die nicht in der Menge der gezählten Funktionen vorkommt, also ist F überabzählbar
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

# Lemma Ü.8.0:
Sei $(a_{n})_{n \in \Z}$ eine Folge und $b,c,d \in \Z: b<c < d$. 
und $\Sum_{n=c}^{\infty} a_{n}$ konvergent.
Dann konvergieren auch
a) $\Sum_{n=b}^{\infty}a_{n}$ 
und 
b) $\Sum_{n=d}^{\infty} a_{n}$
und es gilt:
c) $\Sum_{n=b}^{\infty} a_{n} = \Sum_{n=c}^{\infty}a_{n} + \Sum_{n=b}^{c-1}a_{n}$
und
d) $\Sum_{n=d}^{\infty}a_{n} = \Sum_{n=c}^{\infty}a_{n} - \Sum_{n=c}^{d-1}a_{n}$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

### Beweis:
Sei $S_{m} := \Sum_{n=c}^{m} a_{n}$.
Es gilt: $\Sum_{n=c}^{\infty} a_{n} = \Limin m S_{m}$

Betrachte: $S_{m} + \Sum_{n=b}^{c-1}a_{n}$
Es gilt: $\Limin m S_{m}$ existiert und $\Limin m \Sum_{n=b}^{c-1}a_{n} = \Sum_{n=b}^{c-1}a_{n}$
$\RA \Limin m S_{m} + \Limin m \Sum_{n=b}^{c-1}a_{n} = \Limin m (S_{m} + \Sum_{n=b}^{c-1}a_{n})$ 
$= \Limin m (\Sum_{n=c}^{m} a_{n} + \Sum_{n=b}^{m}a_{n}) = \Limin m \Sum_{n=b}^{m}a_{n} = \Sum_{n=b}^{\infty} a_{n}$ $\checkmark$

Betrachte: $S_{m} - \Sum_{n=c}^{d-1}a_{n}$

Es gilt: $\Limin m S_{m}$ existiert und $\Limin m \Sum_{n=c}^{d-1}a_{n} = \Sum_{n=c}^{d-1}a_{n}$
$\RA \Limin m S_{m} - \Limin m \Sum_{n=c}^{d-1} a_{n} = \Limin m (S_{m} - \Sum_{n=c}^{d-1} a_{n})$
$= \Limin m (\Sum_{n = c}^{m} a_{n} - \Sum_{n=c}^{d-1}a_{n})$ 
$= \Limin m (\Sum_{n= d}^{m}a_{n} + \Sum_{n=c}^{d-1}a_{n} - \Sum_{n=c}^{d-1}a_{n})$
$= \Limin m \Sum_{n=d}^{m} a_{n}$
$= \Sum_{n=d}^{\infty}a_{n}$ 
$\bs$

# Korollar Ü.8.1
Sei $(a_{n})_{n \in \Z}$ eine Folge, die für alle $n \in \Z : n \geq b$ definiert ist, und $b,c,d \in \Z: b<c < d$. 
und $\Sum_{n=c}^{\infty} a_{n}$ absolut konvergent.
Dann konvergieren auch $\Sum_{n=b}^{\infty}a_{n}$ und $\Sum_{n=d}^{\infty}a_{n}$ absolut.
### Beweis:
$\Sum_{n=c}^{\infty}a_{n}$ absolut konvergent $\LRA \Sum_{n=c}^{\infty}|a_{n}|$ konvergent.
Sei $b_{n} = |a_{n}|$
$\RA \Sum_{n=c}^{\infty}b_{n}$ konvergiert
$\stackrel{S.Ü.8.0.a}\RA \Sum_{n=b}^{\infty}b_{n}$ konvergiert
$\LRA \Sum_{n=b}^{\infty}|a_{n}|$ konvergiert $\RA \Sum_{n=b}^{\infty}a_{n}$ konvergiert absolut.
Außerdem:
$\stackrel{S.Ü.8.0.b}\RA \Sum_{n=d}^{\infty}b_{n}$ konvergiert
$\LRA \Sum_{n=d}^{\infty}|a_{n}|$ konvergiert $\RA \Sum_{n=b}^{\infty}a_{n}$ konvergiert absolut.
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>



# Aufgabe 2
### a)
Beh.:
$\Sum_{n=0}^{\infty}a_{n}$ konvergent $\RA \Sum_{n=0}^{\infty}a_{n}^{2}$ konvergent
Gegenbeispiel:
Betrachte $(a_{n})_{n \in \N_{0}} :=\Biggl \{ \begin{matrix} {\frac{1}{\sqrt{\frac{n}{2} + 1}}: 2 \mid n} \\ -\frac{1}{\sqrt{\frac{n-1}{2}+1}}: 2\not \mid n\end{matrix}$
Also $(a_{n}) = \left( 1, - 1, \frac{1}{\sqrt 2}, - \frac{1}{\sqrt 2}, \frac{1}{\sqrt 3}, - \frac{1}{\sqrt 3},\dots \right)$

Sei $(b_{n}) := \biggl \{ \begin{matrix} a_{n} : 2 \mid n \\ -a_{n} : 2 \not \mid n\end{matrix}$

Merke: $a_{n} = (-1)^{n} b_{n}$

Für $b_{n}$ gilt: 
$b_{n}$ ist monoton fallend:

z.z:
$\forall n \in \N_{0}: b_{n} \geq b_{n+1}$

Für n gerade:
$b_{n} = \frac{1}{\sqrt{\frac{n}{2}+1}}$
$b_{n+1} = -\left(- \frac{1}{\sqrt{\frac{n+1-1}{2}+1}}\right) = \frac{1}{\sqrt{\frac{n}{2}+1}} = b_{n}$

Für n ungerade:
$b_{n} = -\left(- \frac{1}{\sqrt{\frac{n-1}{2}+1}} \right) = \frac{1}{\sqrt{\frac{n-1}{2}+1}}$

$b_{n+1} = \frac{1}{\sqrt{\frac{n+1}{2}+1}}$

Aber merke:
$n+1 > n-1$
$\RA \frac{n+1}{2} > \frac{n-1}{2}$
$\RA \frac{n+1}{2}+1 > \frac{n-1}{2}+1$

Da $n \in \N_{0}$ und n gerade gilt, folgt: $n \geq 1$
$\RA$ wir können die Wurzel ziehen, und die Gleichheit bleibt erhalten 
$\RA \sqrt{\frac{n+1}{2}+1} > \sqrt{\frac{n-1}{2}+1}$
$\RA \frac{1}{\sqrt{\frac{n-1}{2}+1}}> \frac{1}{\sqrt{\frac{n+1}{2}+1}}$
$\RA b_{n} > b_{n+1}$

$\RA b_{n}\geq b_{n+1} \F n \in \N_{0}$
$\RA b_{n}$ ist monoton fallend.

Außerdem ist $\limin b_{n} = 0$:
Beweis: 
...

$\RA b_{n}$ ist monoton fallend und konvergent gegen 0
$\RA \Sum_{n=0}^{\infty}(-1)^{n}b_{n} = \Sum_{n=0}^{\infty}a_{n}$ konvergiert nach Leibnitzkriterium.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

Aber $\Sum_{n=0}^{\infty}a_{n}^{2}$ konvergiert nicht:

$(a_{n}^{2}) = \left( 1,1, \frac{1}{2}, \frac{1}{2}, \frac{1}{3}, \frac{1}{3}, \frac{1}{4}, \frac{1}{4},\dots \right)$
$\RA a_{n}^{2} \geq \frac{1}{n} \F n \in \N$

Aber $\Sum_{n=1}^{\infty} \frac{1}{n}$ divergiert, und folglich divergiert auch $\Sum_{n=0}^{\infty}a_{n}^{2}$
Folglich existiert eine Folge $(a_{n})$ mit $\Sum_{n=0}^{\infty}a_{n}$ konvergent aber $\Sum_{n=0}^{\infty}a_{n}^{2}$ divergent
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


### b)
Z.z:
$\Sum_{n=1}^{\infty}a_{n}$ konvergiert absolut $\RA \Sum_{n=1}^{\infty}a_{n}^{2}$ konvergiert.

#### Beweis:
Im folgenden wird eine stärkere Aussage bewiesen werden, nähmlich $\Sum_{n=1}^{\infty}a_{n}$ konvergiert absolut $\RA \Sum_{n=1}^{\infty}a_{n}^{k}, k > 1$ konvergiert absolut.
(im folgenden wird hierfür $k \in \N$ vorrausgesetzt, da hierfür die folgende Aussage einfach gültig ist: ($a >1 \RA a^{k} > a$). Diese Aussage kann aber auch für $k \in \R$ bewiesen werden, dann ist der folgende Beweis auch für alle $k \in \R: k > 1$ gültig.)

Beweis:
Sei $k \in \N, k > 1$ und $(a_n)$ eine Folge mit der Eigenschaft:
$\Sum_{n=1}^{\infty}a_{n}$ absolut konvergent, also $\Sum_{n=1}^{\infty}|a_{n}|$ konvergent.
Es gilt, $b > 1 \RA b^{k}>b$ 
Sei also b > 1. Dann gilt:
$\exists a: 0 < a < 1: a = \frac{1}{b}$
Betrachte $b^{k}> b$
$\RA \frac{1}{b} > \frac{1}{b^{k}}$
$\RA \frac{1}{b} > \left( \frac{1}{b} \right)^{k}$
$\RA a > a^{k}$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

Analog dazu gilt aber auch:
$|a| < 1 \RA |a| > |a|^{k}$, da $|a|$ immer positiv ist, mann also einfach $|a| := b$ definieren kann, und gilt, $0 < b < 1$ und somit die obere ungleichung gilt. Außerdem gilt auch $|a|^{k} = |a^{k}|$ (weil $a^{k}= |a^{k}|$ für k gerade und $a^{k} = - |a|^{k}$ für k ungerade, a < 1, also $|a^{k}| = |a|^{k}$)

$\Sum_{n=1}^{\infty}|a_{n}|$ konvergent $\RA \forall \varepsilon > 0 \E N \in \N: \mid \Sum_{i=m}^{n}|a_{k}| \mid< \varepsilon \F n \geq m \geq N$

$\RA \exists N_{1} \in \N: \mid \Sum_{i=m}^{n}|a_{k}| < 1 \F n \geq m \geq N_{1}\mid$
Da aber $|a_{n}| > 0 \F n \in \N$ gelten muss, folgt direkt:
$|a_{n}| < 1 \F n \geq N_{1}$ (ansonsten wäre bereits ein einzelnes Glied der Summe größer als Epsilon)

$1 > |a_{n}| \F n \geq N_{1} \RA |a_{n}|> |a_{n}|^{k} \F n \geq N_{1}$

$\RA \Sum_{n=N_{1}}^{\infty} |a_{n}|^{k}$ hat als eine majorante durch $\Sum_{n=N_{1}}^{\infty}|a_{n}|$

$\RA \Sum_{n=N_{1}}^{\infty} |a_{n}|^{k} = \Sum_{n=N_{1}}^{\infty} |a_{n}^{k}|$ konvergiert absolut

$\RA \Sum_{n=N_{1}}^{\infty} a_{n}^{k}$ konvergiert absolut

$\stackrel{Ü.8.0 \land Ü.8.1}\RA \Sum_{n=1}^{\infty}a_{n}^{k}$ konvergiert absolut.
$\bs$
(in diesem Beweis ist der Fall $\Sum_{n=1}^{\infty}a_{n}^{2}$ bereits enthalten, und absolute konvergenz impliziert Konvergenz!)
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

### c)
Z.z:
$\Sum_{k=1}^{\infty}a_{n}^{2}$ konvergent$\land\Sum_{k=1}^{\infty}b_{n}^{2}$ konvergent $\RA \Sum_{k=1}^{\infty}a_{n}b_{n}$ konvergent.

Beweis:
Seien $(a_{n}),(b_{n})$ folgen, sd. $\Sum_{k=1}^{\infty}a_{n}^{2}, \Sum_{k=1}^{\infty}b_{n}^{2}$ konvergieren.

Es gilt $\forall a,b \in \R: 0 \leq (a-b)^{2}$
$\RA 0 \leq a^{2} + b^{2} - 2ab$
$\RA 2ab \leq a^{2} + b^{2}$ 
Aber auch $ab \leq a^{2}+b^{2}$, da:
Für $a,b \geq 0$ gilt:
$2ab \geq ab$
und für $a,b < 0$ gilt $ab = (-a)(-b) \leq 2ab$

Für $a >0, b \geq 0$ gilt aber $ab < 0$, aber es gilt $a^{2} + b^{2} >0$ also gilt folglich auch $a^{2}+b^{2} \geq ab$ (analog für $b \geq 0, a < 0$)

Damit gilt aber allgemein $ab \leq a^{2} + b^{2}$

Da $\Sum_{k=1}^{\infty}a_{k}^{2}, \Sum_{k=1}^{\infty}a_{k}^{2}$ konvergent, gilt auch $\Sum_{k=1}^{\infty}a_{k}^{2} + \Sum_{k=1}^{\infty}b_{k}^{2}$ konvergent
und $\Sum_{k=1}^{\infty}a_{k}^{2} + \Sum_{k=1}^{\infty}b_{k}^{2} = \Sum_{k=1}^{\infty} a_{k}^{2} + b_{k}^{2}$ 
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

(Genauer: Sei $S_{m} := \Sum_{k=1}^{m}a_{k}^{2}$ und $S'_{n} := \Sum_{k=1}^{n}b_{k}^{2}$, dann ist 
$S_{m} + S'_{m} = \Sum_{k=1}^{m}a_{k}^{2}+\Sum_{k=1}^{m}b_{k}^{2} =\Sum_{k=1}^{m} a_{k}^{2}+b_{k}^{2}$ 
und $\Limin m S_{m} = \Sum_{k=1}^{\infty} a_{k}^{2}$ konvergent, $\Limin n S'n =\Sum_{k=1}^{\infty}b_{n}^{2}$ konvergent,
und damit auch $\limin S_{m} + S'_{m} = \Sum_{k=1}^{\infty}a_{k}^{2}+b_{k}^{2}$ konvergent (linearität des Grenzwertes))

Es gilt aber $a^{2}_{k} + b^{2}_{k} \geq a_{k}b_{k} \F k \in\N \RA \Sum_{k=1}^{\infty}a_{k}^{2} + b_{k}^{2}$ ist majorante,
$\Sum_{k=1}^{\infty}a_{k}b_{k}$ konvergiert absolut, und damit konvergiert es auch
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


# Aufgabe 3

### a)
Sei $(a_{n})_{n \in \N}$ eine monoton fallende Folge mit $a_{n} \geq 0 \F n \in \N$

Z.z:
$\Sum_{k=1}^{\infty} a_{k}$ konvergent $\LRA \Sum_{k=0}^{\infty}3^{k}a_{3^{k}}$ konvergent

"$\RA$"

Sei $\Sum_{k=1}^{\infty} a_{k}$ konvergent

$(a_{n})$ monoton fallend $\RA a_{n} \geq a_{n+1} \F n \in\N$

$\Sum_{k=1}^{\infty} a_{k}$ konvergent und $a_{n} \geq 0\RA \exists N_{1} \in \N : a_{n} < \frac{1}{3} \F n \geq N_{1}$ (weil sonst das Cauchykriterium schon durch ein Glied überschritten wird.)

$\RA a_{n}^{k} \leq \frac{1}{3^{k}} \F n \geq N_{1}$

$\RA a_{3^{k}} \leq \frac{1}{3^{3^{k}}} = \frac{1}{3^{3k}} \F k \geq N_{1}$

$\RA 3^{k}a_{3^{k}} \leq 3^{k} \cdot \frac{1}{3^{3k}} = \frac{3^{k}}{3^{3k}} = \frac{1}{3^{2k}} \F k \geq N_{1}$

$\RA \Sum_{k=N_{1}}^{\infty}3^{k}a_{3^{k}}$ hat $\Sum_{k=N_{1}}^{\infty} \left( \frac{1}{3^{2}} \right)^{k}$ als Majorante, aber $\Sum_{k=0}^{\infty} \left( \frac{1}{3^{2}} \right)^{k}$ konvergiert als Geometrische Reihe, und damit nach Lemma Ü.8.0 auch $\Sum_{k=N_{1}}^{\infty} \left( \frac{1}{3^{2}} \right)^{k}$

Folglich konvergiert $\Sum_{k=N_{1}}^{\infty} 3^{k} a_{3^{k}}$ und damit nach Lemma Ü.8.0 auch $\Sum_{k=0}^{\infty} 3^{k}a_{3^{k}}$ 
$\checkmark$

"$\LA$"
Sei $\Sum_{k=0}^{\infty} 3^{k}a_{3^{k}}$ konvergent.
...

<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

### b)
Z.z:
$\Sum_{k=1}^{\infty} \frac{1}{k^{\alpha}}$ konvergiert für $\alpha >1$

$\stackrel{a)}\LRA \Sum_{k=0}^{\infty} 3^{k}\frac{1}{(3^{k})^{\alpha}}$ konvergent

$\Sum_{k=0}^{\infty}3^{k} \frac{1}{(3^{k})^{\alpha}} = \Sum_{k=0}^{\infty} \frac{3^{k}}{3^{k \alpha}} = \Sum_{k=0}^{\infty} \frac{3^{k}}{(3^{\alpha})^{k}} = \Sum_{k=0}^{\infty} \left( \frac{3}{3^{\alpha}} \right)^{k}$

$= \Sum_{k =0}^{\infty} \left( \frac{1}{3^{\alpha-1}} \right)^{k}$

$\alpha >1 \RA \alpha - 1 >0$
$\RA 3^{\alpha-1} > 1 \RA \frac{1}{3^{\alpha-1}} < 1 \RA |\frac{1}{3^{\alpha-1}}| <1$

$\RA \Sum_{k=0}^{\infty} \left( \frac{1}{3^{\alpha-1}} \right)^{k}$ konvergiert als Geometrische Reihe.
$\RA \Sum_{k=1}^{\infty} \frac{1}{k^{\alpha}}$ konvergiert
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


# Aufgabe 4
Sei $(a_{k})$ eine Folge mit $a_{k} \to 0$
Zu zeigen:
$\Limin k \frac{\exp(a_{k})-1}{a_{k}} = 1$

$\d\frac{\exp(a_{k}-1)}{a_{k}} = \frac{\Sum_{n=0}^{\infty} (\frac{a_{k}^{n}}{n!}) - 1}{a_{k}}$

$=\d \frac{\Sum_{n=1}^{\infty} (\frac{a_{k}^{n}}{n!}) + 1-1}{a_{k}}$

$\d= \frac{\Sum_{n=1}^{\infty} \frac{a_{k}^{n}}{n!}}{a_{k}}$

$= \Sum_{n=1}^{\infty} \frac{a_{k}^{n-1}}{n!}$

$= \Sum_{n=0}^{\infty} \frac{a_{k}^{n}}{(n+1)!}$

$\d= \frac{a_{k}^{0}}{(0+1)!} + \Sum_{n=1}^{\infty} \frac{a^{n}_{k}}{(n+1)!}$

$= 1 + \Sum_{n=1}^{\infty} \frac{a_{k}^{n}}{(n+1)!}$ ($0^{0} := 1$ wurde am Anfang so definiert, also gilt allgemein für alle $x \in \R$: $x^{0} = 1$)

$\RA \Limin k \frac{\exp(a_{k})-1}{a_{k}} =  \Limin k \left( 1+ \Sum_{n=1}^{\infty} \frac{a_{k}^{n}}{(n+1)!} \right)$

$= 1 + \Limin k \Sum_{n=1}^{\infty} \frac{a_{k}^{n}}{(n+1)!}$
## Korrektur
Hier wird vorausgesetzt, das $\Sum_{n=1}^{\infty} \frac{a^{n}}{(n+1)!}$ für alle a konvergiert, ein Beweis dafür folgt vielleicht noch.
$= 1 + \Lim_{k\to \infty} \left( a_{k} \Sum_{n=1}^{\infty} \frac{a_{k}^{n-1}}{(n+1)!} \right)$
$= 1+ \Lim_{k \to \infty} a_{k} \cdot \Lim_{k\to \infty} \Sum_{n=1}^{\infty} \frac{a_{k}^{n-1}}{(n+1)!}$ //immer noch konvergent
$= 1 + 0 \cdot \Lim_{k\to \infty} \Sum_{n=1}^{\infty} \frac{a_{k}^{n-1}}{(n+1)!}$
$= 1+ 0$
$=1$
$\bs$
#### Alte, Falsche Lösung
$= 1+ \Sum_{n=1}^{\infty} \Limin k \frac{a_{k}^{n}}{(n+1)!}$ 
$(a_{k}) \to 0$
$= 1+ \Sum_{n=1}^{\infty} \frac{0^{n}}{(n+1)!}$ 

$= 1 + \Sum_{k=1}^{\infty} 0$
$= 1$
$\bs$

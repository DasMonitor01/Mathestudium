#### Aufgabe 1
a)

Zu zeigen:
$\Sum_{k=0}^{n}{x^k} = \frac{1 - x^{n+1}}{1-x}$

Beweis durch Induktion:

Induktionsanfang:
n = 1:
$LS = \Sum_{k=0}^{n}x^k = \Sum_{k=0}^{1}x^k = x^0 + x^1 = x + 1$
$\d RS = \frac{1 - x^{n+1}}{1 - x}=\frac{1 - x^{1+1}}{1 - x} = \frac{1 - x ^2}{1 - x} = \frac{(1 + x)(1 - x)}{1-x} = x + 1$ 
$\Rightarrow LS = RS$

Induktionsschritt:
$(I)$ Wir wissen für ein $n \in \N$ gilt: $\Sum_{k=1}^{n}{x^k} = \frac{1 - x^{n+1}}{1-x}$ 
-> n+1:

$\Sum_{k=1}^{n+1}{x^k}$
$= \Sum_{k=1}^{n}{x^k}+ x^{n+1}$
$\d \stackrel{I}= \frac{1-x^{n+1}}{1-x} + x^{n+1}$
$\d = \frac{1 - x^{n+1}}{1-x} + \frac{(1-x)x^{n+1}}{1-x}$
$\d = \frac{1 - x^{n+1}}{1-x}+ \frac{x^{n+1} - x^{n+2}}{1 - x}$
$\d = \frac{1 - x^{n+1} + x^{n+1} - x^{n+2}}{1 - x}$
$\d \frac{1 - x^{n+2}}{1 - x}$
$\blacksquare$

b)
Lemma:
L1:
Sei $a \in \N$ und $b \in \Z$
Es gilt folgende Relation
$\binom{a}{b} = \binom{a - 1}{b - 1} + \binom{a - 1}{b}$
Beweis:
siehe Vorlesungsskript Lemma 1.5


Zu zeigen:
Seien $m, n \in \N_0$
$\Sum_{k=0}^{n}\binom{m + k}{k} = \binom{m + n + 1}{n}$

Beweis durch Induktion:
Sei $m \in \N_0$ beliebig

Induktionsanfang:
n = 0
$LS = \Sum_{k = 0}^{0} \binom{m + k}{k} = \binom{m}{0} = \frac{m!}{(m - 0)! \cdot 0!} = \frac{m!}{m!} = 1$
$\d RS = \binom{m + n + 1}{n} = \binom{m + 1}{0} = \frac{(m + 1)!}{(m + 1 - 0)! \cdot 0!} = \frac{(m+1)!}{(m + 1)!} = 1$
$\Rightarrow LS = RS$

Induktionsschritt:
$(I)$ Wir wissen für ein $n \in \N_0$ gilt: $\Sum_{k=0}^{n}\binom{m + k}{k} = \binom{m + n + 1}{n}$ 
-> n + 1:

$\Sum_{k=0}^{n + 1}\binom{m + k}{k}$
$= \Sum_{k=0}^{n}\binom{m + k}{k} + \binom{m + n + 1}{n + 1}$
$\d\stackrel{I}= \binom{m + n + 1}{n} + \binom{m + n + 1}{n + 1}$ -> $(II)$ Sei $a = m + n + 2$ und $b = n + 1$
$\stackrel{II}= \binom{a - 1}{b - 1} + \binom{a - 1}{b}$ 
$\stackrel{L1} = \binom{a}{b} \stackrel{II}= \binom{m + (n + 1) + 1}{n +1}$
$\blacksquare$


#### Aufgabe 2
Erinnerung: 
Körperaxiome:
a)
$x \cdot 0$
$\stackrel{A4}= x \cdot (1 - 1)$
$\stackrel{D}= (x\cdot 1)-(x \cdot 1)$
$\stackrel{M3}= (x)-(x)$
$\stackrel{A1}= x - x$
$\stackrel{A4}= 0$
$\blacksquare$

b)
Sei $x \in K: x \neq 0$
$\Rightarrow x \neq 0$
$\Leftrightarrow x \cdot 1 \neq x \cdot 0$
$\Leftrightarrow x \cdot 1 \cdot x^{-1} \neq x \cdot 0 \cdot x^{-1}$
$\Leftrightarrow x \cdot x^{-1} \cdot 1 \neq x \cdot x^{-1} \cdot 0$
$\Leftrightarrow 1 \neq 0$
$\blacksquare$

c)
Sei $x \in K: x \neq 0$

Hinweis:
$x^{-1} \cdot (x^{-1})^{-1} = 1$ (M4)

$x = x$
$x = x \cdot 1$ (M3)
$x = x \cdot x^{-1} \cdot (x^{-1})^{-1}$ (M4)
$x = 1 \cdot (x^{-1})^{-1}$ (M4)
$x = (x^{-1})^{-1}$  (M1)
$\blacksquare$

d)
$x \cdot (-y)$
$\stackrel{M2}= -y \cdot x$
$\stackrel{M1}= - (y \cdot x)$
$\stackrel{M2}= -(x \cdot y)$
$\blacksquare$

e)
Sei $x = 0$
Sei $y = -x$ (A4)
$x + y = 0$ (A4)
$0 + y = 0$ 
$y = 0$ 
$- x = 0$
$-0 = 0$
$\blacksquare$

f)
z.z: $-(-x) = x$
Anmerkung:
$-x + (-(-x)) = 0$ (A4)

Sei $x \in K$
$x = x$
$x = x + 0$ (A3)
$x = x (- x + (-(-x)))$ (A4)
$x = x - x + (-(-x))$ (A1)
$x = 0 + (-(-x))$ (A4)
$x = (-(-x))$ (A3)
$x = -(-x)$ (A1)
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

#### Aufgabe 3
Gegeben:
$(I)$ $A, B \subseteq \R$
$(II)$ $A, B \neq \es$
$(III)$ $A \cup B = \R$
$(IV)$ $\forall a \in A\F b \in B: a < b$ 

Vorarbeit:
Aus den Forderungen folgt, da ss A nach unten unbeschränkt und nach oben beschränkt und B nach oben unbeschränkt und nach unten beschränkt sein muss (da weder A noch B leer sein können, und alle Elemente aus A kleiner als alle Elemente aus B sein müssen, und alle Reellen Zahlen abgedeckt sein müssen. Für einen erweiterten Beweis siehe Anhang)
Somit muss gelten:
$(V)$ $\exists c : c = \sup A$
$\Rightarrow x \leq c \F x \in A$  
$(VI)$ $\exists d \in \R: d = \inf A$
$\Rightarrow d \leq y \F y \in B$
$(VII)$ $c \leq d$ (nach Ordnungsrelation $IV$)

Zu zeigen:
$c = d$

Beweis durch wiederlegung der Negation:
Angenommen $c < d$
$\stackrel{Kor.2.4}\Rightarrow \exists e \in \R: c < e < d$
$\stackrel{V}\Rightarrow e \notin A$
$\stackrel{VI}\Rightarrow e \notin B$
$\Rightarrow e \notin A \cup B$ aber $e \in \R$
$\Rightarrow A \cup B \neq \R \rightarrow \leftarrow (III)$
 
somit folgt das c = d gelten muss (und mit der Eindeutigkeit des Supremums, dass nur ein c existieren kann).
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

#### Aufgabe 4
a)
$\d M = \set{\frac{3+ (-1)^n}{2^{n+1}}\mid n \in \N}$ 
Merke: $M \subset \R$

$\sup M = \max M = \frac{1}{2}$

Beweis:
Z.z.:
$\d \frac{3 + (-1)^n}{2^{n+1}} \leq \frac{1}{2} \F n \in \N$

Merke:
$\d n = 1 \Rightarrow \frac{3 + (-1)^n}{2^{n+1}} = \frac{2}{4} = \frac{1}{2}$
$\d 3 + (-1)^n \leq 4$
$\d\Rightarrow \frac{3 + (-1)^n}{2^{n+1}} \leq \frac{4}{2^{n+1}}$
Für $n \geq 2$
$\d\Rightarrow \frac{3 + (-1)^n}{2^{n+1}} \leq \frac{4}{2^{n+1}} \leq \frac{4}{2^{2 + 1}}$
$\d\Rightarrow \frac{3 + (-1)^n}{2^{n+1}} \leq \frac{1}{2} \F n \geq 1$
$\d \Rightarrow\frac{3+ (-1)^n}{2^{n+1}} \leq \frac{1}{2} \F n \in \N$
$\blacksquare$

$\inf M = 0$

Beweis:

Z.z.:
$(I)$ $\d\frac{3 + (-1)^n}{2^{n+1}} \geq 0 \F n \in \N$
$(II)$ $(\exists t \in \R : x \geq t \F x \in M ) \Rightarrow t \leq 0$

$(I)$:

Merke: 
$3 + (-1)^n \geq 0 \F n \in \N$
$2^{n+1} \geq 0 \F n \in \N$
$\d\Rightarrow \frac{3 + (-1)^n}{2^{n+1}} \geq 0 \F n \in \N$

$(II)$:
Sei $t \in [0,\infi)$  (da unsere Menge nach $(I)$ größer gleich 0 ist)mit
$(III)$: $\d \frac{3 + (-1)^n}{2^{n+1}} \geq t \F n \in \N$ 
$\d\Rightarrow t - \frac{3 + (-1)^n}{2^{n+1}} \leq 0$
$\d\Rightarrow |t - \frac{3+ (-1)^n}{2^{n+1}}| \leq 0$
$\d \stackrel{\triangle ungl}\Rightarrow 0 \geq |t - \frac{3+ (-1)^n}{2^{n+1}}| \geq |t| + | - \frac{3 + (-1)^n}{2^{n+1}}|$
$\d\Rightarrow 0 \geq | t - \frac{3+(-1)^n}{2^{n+1}}| \geq |t| + \frac{3+(-1)^n}{2^{n+1}} \stackrel{III}\geq |t| + t$
$\stackrel{t \geq 0}\Rightarrow 0 \geq 2t$
$\stackrel{:2}\Rightarrow 0 \geq t$
$\blacksquare$

b)
$M = \set{\frac{x}{1 + x^2}| x \in \R}$

$\sup M = \max M = \frac{1}{2}$

Beweis:
Z.z.:
$\frac{x}{1+x^2} \leq \frac{1}{2} \F x \in \R$

Fallunterscheidung:
x  = 1:
$\frac{x}{1+x^2} = \frac{1}{1 + 1} = \frac{1}{2}$

x > 1:
$(I)$: $\Rightarrow |x^2| > |x|$
$\Rightarrow x = 1 + y: y > 0$
$\Rightarrow \frac{x}{1+x^2} = \frac{y + 1}{(1 + y)^2 +1} \stackrel{I}< \frac{1}{1 + 1}$
$\Rightarrow \frac{x}{1 + x^2} < \frac{1}{2}$

0 < x < 1:
$ $

x < 0:
$\Rightarrow \frac{x}{1 + x^2} < 0$

$\inf M = min M = -\frac{1}{2}$

Beweis:
Z.z.:
$\frac{x}{1+x^2} \geq - \frac{1}{2} \F x \in \R$

Fallunterscheidung:
x = -1:
$\frac{x}{1 + x^2} = \frac{-1}{1 + 1} = -\frac{1}{2}$

x < -1:
$(II)$: $\Rightarrow |x^2| > |x|$
$\Rightarrow x = -1 - y: y > 0$
$\Rightarrow \frac{x}{1+x^2} = \frac{-y - 1}{(-1 - y)^2 +1} \stackrel{II} > \frac{-1}{1 + (-1)^2}$
$\Rightarrow \frac{x}{1 + x^2} > - \frac{1}{2}$


-1 < x < 0:



x > 0:
$\Rightarrow \frac{x}{1 + x^2} > 0$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


# Anhang

#### Aufgabe 3:
Gegeben:
$(I)$ $A, B \subseteq \R$
$(II)$ $A, B \neq \es$
$(III)$ $A \cup B = \R$
$(IV)$ $\forall a \in A\F b \in B: a < b$ 

Es muss gelten, dass A nach unten unbeschränkt ist, d.h.
$(V)$ $A=(-\infi, c) \cup C : (C=\es \lor C = \set{c})$ 
(A ist entweder $(-\infi, c)$ oder $(-\infi, c]$)

Beweis:
Angenommen A ist nach unten beschränkt, d.h.
$(VI)$ $\exists s_1 \in \R: s_1 \leq a \F a \in A$

$\stackrel{II}\Rightarrow \exists x \in A$
$\stackrel{VI}\Rightarrow s_1 \leq x$ 
Außerdem gilt: 
$s_1-1 \in \R$
und
$(VII):$ $s_1 -1 < s_1$  

$\stackrel{VI,VII}\Rightarrow s_1 - 1 \notin A$ 
$\stackrel{VII}\Rightarrow s_1-1 < x$
$\Rightarrow s_1-1 \notin B$, da sonst gelten würde $\exists y \in B \E x \in A: y<x$ (wiederspruch zur Ordnungsforderung $a < b, \forall a \in A, b \in B$)
$\Rightarrow s_1 - 1 \notin A \land s_1 - 1 \notin B$
$\Rightarrow s_1 -1 \notin A \cup B$
$\Rightarrow s_1 -1 \in \R \land s_1 -1 \notin A \cup B$ 
$\Rightarrow A \cup B \neq \R \rightarrow \leftarrow A\cup B = \R$

Somit kann keine untere Schranke für A existieren


Außerdem muss gelten, dass B nach oben unbeschränkt ist, d.h.
$B = (d, \infi) \cup D : (D = \es \lor D = \set{d})$
(B ist entweder $(d,\infi)$ oder $[d, \infi)$)

Beweis:
Angenommen B ist nach oben beschränkt, d.h.
$(VIII)$ $\exists s_2 \in \R: s_2 \geq b \F b \in B$

$\stackrel{II}\Rightarrow \exists x \in B$
$\stackrel{VIII}\Rightarrow s_2 \geq x$
Außerdem gilt: 
$s_2+1 \in \R$
und
$(XI):$ $s_2 + 1 > s_2$  

$\stackrel{VIII,XI}\Rightarrow s_2 + 1 \notin A$ 
$\stackrel{VIII}\Rightarrow s_2+1 > x$
$\Rightarrow s_2+1 \notin A$, da sonst gelten würde $\exists y \in A \E x \in B: y>x$ (wiederspruch zur Ordnungsforderung $a < b, \forall a \in A, b \in B$)
$\Rightarrow s_2 1+1 \notin A \land s_2 + 1 \notin B$
$\Rightarrow s_2+1 \notin A \cup B$
$\Rightarrow s_2 +1 \in \R \land s_2 +1 \notin A \cup B$ 
$\Rightarrow A \cup B \neq \R \rightarrow \leftarrow A\cup B = \R$ 

Somit kann keine obere Schranke für B existieren
$\blacksquare$

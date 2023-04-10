Zur Erinnerung: (Aus Übungsblatt 1)
Seien A, B, und C Aussagen.
Es gelten folgende Relationen:
$(E.I)$ Assoziatvität
$A \land (B \land C) \Leftrightarrow (A \land B) \land C$
$A \lor (B \lor C) \Leftrightarrow (A \lor B) \lor C$

$(E.II)$ Kommutativität
$A \land B \Leftrightarrow B \land A$
$A \lor B \Leftrightarrow B \lor A$

$(E.III)$ Distributivität
$(A \land B) \lor C \Leftrightarrow (A \lor C) \land (B \lor C)$
$(A \lor B) \land C \Leftrightarrow (A \land C) \lor (B \land C)$

$(E.IV)$ Demorgensche Gesetze
$\lnot(A \land B) \Leftrightarrow \lnot A \lor \lnot B$
$\lnot(A \lor B) \Leftrightarrow \lnot A \land \lnot B$

#### Aufgabe 2.5 
a) 
$M \cap (N \cap L)$
$\Leftrightarrow x \in M \land (x \in N \land x \in L)$ 
$\stackrel{E.I} \Leftrightarrow (x \in M \land x \in N) \land x \in L$
$\Leftrightarrow (M \cap N) \cap L$

$M \cup (N \cup L)$
$\Leftrightarrow x \in M \lor (x \in N \lor x \in L)$
$\stackrel{E.I}\Leftrightarrow (x \in M \lor x \in N) \lor x \in L$
$\Leftrightarrow (M \cup N) \cup L$
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

b)
$M \cup (N \cap L)$
$\Leftrightarrow x \in M \lor (x \in N \land x \in L)$ 
$\stackrel{E.III} \Leftrightarrow (x \in M \lor x \in N) \land (x \in M \lor x \in L)$
$\Leftrightarrow (M \cup N) \cap (M \cup L)$

$M \cap (N \cup L)$
$\Leftrightarrow x \in M \land (x \in N \lor x \in L)$
$\stackrel{E.III}\Leftrightarrow (x \in M \land x \in N) \lor (x \in M \land x \in L)$ 
$\Leftrightarrow (M \cap N) \cup (M \cap L)$ 
$\blacksquare$ 

Lemma:
L1:
$M \cap M = M$
(Beweis siehe Anhang A2.5.L1)

c)
$M \without (N \cap L)$ 
$\Leftrightarrow x \in M \land \lnot (x \in N \land x \in L)$ 
$\stackrel{E.IV}\Leftrightarrow x \in M \land (x \notin N \lor x \notin L)$ 
$\stackrel{E.III}\Leftrightarrow (x \in M \land x \notin N) \lor (x \in M \land x \notin L)$
$\Leftrightarrow (M \without N) \cup (M \without L)$ 

$M \without (N \cup L)$
$\Leftrightarrow x \in M \land \lnot (x \in N \lor x \in L)$
$\stackrel{E.IV}\Leftrightarrow x \in M \land (x \notin N \land x \notin L)$
$\stackrel{L1}\Leftrightarrow x \in M \land x \in M \land (x \notin N \land x \notin L)$
$\stackrel{E.I; E.II} \Leftrightarrow (x \in M\land x \notin N) \land (x \in M \land x \notin L)$
$\Leftrightarrow (M \without N) \cap (M \without L)$
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

#### Aufgabe 2.6:
Notation:
$(N.I)$ a teilt b $:\Leftrightarrow a \mid b :\Leftrightarrow \E z \in \Z: a \cdot z = b$ (Definition der Teilbarkeit)
$(N.II)$ a teilt b nicht $: \Leftrightarrow a \not \mid b :\Leftrightarrow \lnot (a \mid b)$ (Entweder ist eine Zahl Teilbar oder nicht)

Lemma:
L1:
$(A \Rightarrow B) \Leftrightarrow (\lnot(A \land \lnot B))$
Beweis:
siehe Aufgabe 2.1 (falls Beweis gefordert siehe Anhang A2.6.L1)

L2:
$\lnot(\lnot A) \Leftrightarrow A$
(Beweis falls gefordert, siehe Anhang A2.6.L2)

L3:
Seien $a,b \in \Z$
$a \not \mid b \Rightarrow \frac{b}{a} \notin \Z$
(Wenn a nicht b teilt, dann ist der Quotient aus b mit a keine ganze Zahl.)
(Beweis falls gefordert, siehe Anhang A2.6.L3)

L4:
Seien $a,b \in \Z$
Es gilt auch:
$a \cdot b \in \Z$
(Das Produkt zweier ganzer Zahlen ist eine ganze Zahl)
(Beweis: Dieses Lemma ist so offensichtlich, dass es sich nach meiner Ansicht, auf Grund der Aufwändigkeit eines Beweises, außerhalb eines Numerikkurses nicht rentiert, hierzu einen Beweis aufzuschreiben (man könnte es Induktiv zeigen))
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

Seien $n,p \in \N$
### Zu zeigen:
p teilt nicht n $\Rightarrow$ $p^2$ teilt nicht n
$\stackrel{N.II}\Leftrightarrow (p \not \mid n \Rightarrow p^2 \not \mid n)$
$\stackrel{L1}\Leftrightarrow \lnot(p \not \mid n \land \lnot (p^2 \not \mid n))$

Negation:
$\lnot(\lnot(p \not \mid n \land \lnot (p^2 \not \mid n)))$
$\stackrel{L2}\Leftrightarrow p \not \mid n \land \lnot (p^2 \not \mid n)$
$\stackrel{N.II}\Leftrightarrow p\not \mid n \land p^2 \mid n$
(p teilt nicht n und $p^2$ teilt n)
$\Rightarrow$ Annahme: $p \not \mid n \land p \mid n^2$
$p \not \mid n$
$\stackrel{L3}\Rightarrow \frac{n}{p} \notin \Z$

$p^2 \mid n$
$\stackrel{N.I}\Leftrightarrow \exists z \in \Z: p^2 \cdot z = n$
$\Leftrightarrow p \cdot p \cdot z = n$
$\stackrel{:p}\Leftrightarrow p \cdot z = \frac{n}{p}$ $(I)$
Aber:
$\stackrel{L4}\Rightarrow p \cdot z \in \Z$ (da $p \in \N \land z \in \Z$)

$p \cdot z \in \Z$ aber $\frac{n}{p} \notin \Z$
$\Rightarrow p \cdot z \neq \frac{n}{p} \contra (I)$
$\Rightarrow (p \not \mid n) \land (p^2 \mid n)$ ist falsch .


Dementsprechend muss gelten:
$(p \not \mid n) \Rightarrow (p^2 \not \mid n)$ ist wahr.
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

#### Aufgabe 2.7:
Lemma:
L1:
Sei $x \in \Q: x \neq 0$
Dann ist auch $\frac{1}{x} \in \Q$
(Beweis falls gefordert siehe Anhang A2.7.L1)

L2:
Sei $x \in \R$
Dann ist $x^2 \geq 0$
(Beweis falls gefordert siehe Anhang A2.7.L2)

a)
$\forall x \in \Q\without\set{0} \E y \in \Q\without\set{0}: x \cdot y = 1$
Gesprochen:
Für jede rationale Zahl ungleich Null existiert eine zweite rationale Zahl ungleich Null, sodass das Produkt der Zahlen 1 ist

Beweis:
$x \in \Q\without\set{0}$
Wähle $y = \frac{1}{x}$
Es gilt $y \in \Q\without\set{0}$ (nach L1)
$\Rightarrow x \cdot y = x \cdot \frac{1}{x} = \frac{x}{x} = 1$
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

b)
$\exists x \in \Q\without\set{0} \F y \in \Q\without\set{0} : x \cdot y = 1$
Gesprochen:
Es gibt eine rationale Zahl ungleich Null, die mit allen rationalen Zahlen ungleich Null im Produkt 1 ergibt.

Negation:
$\forall x \in \Q \without\set{0} \E y \in \Q\without\set{0}:x \cdot y \neq 1$ 
Gesprochen:
Es gibt für alle rationalen Zahlen ungleich Null eine rationale Zahl ungleich Null, sodass das Produkt der zwei Zahlen nicht 1 ist.

Beweis:
Sei $x \in \Q\without\set{0}$
Wähle $y = 2 \cdot \frac{1}{x} = \frac{2}{x}$
Es gilt $y \in \Q\without\set{0}$ (nach L1)
$\Rightarrow x \cdot y = x \cdot \frac{2}{x} = \frac{2x}{x} = 2 \neq 1$
(wir haben eine Methode gefunden, um für jede rationale Zahl eine andere Zahl zu finden, bei der das Produkt ungleich 1 ist)
$\blacksquare$

c)
$\exists z \in \Z \F x \in \Z : x + z = x$
Gesprochen:
Es gibt eine ganze Zahl z für alle ganzen Zahlen sodass die Summe der Zahlen mit z die Zahlen selbst liefert.

Beweis:
Sei $x \in \Z$ beliebig
Wähle z = 0;
$\Rightarrow z \in \Z$
$\Rightarrow x + z = x + 0 = x$
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

d)
$\forall y \in \R \E x \in \R : y = x^2$
Gesprochen:
Für alle reellen Zahlen existiert eine rationale Zahl x so das das Quadrat von x die Zahl ist.

Negation:
$\exists y \in \R \F x \in \R: y \neq x^2$

Beweis:
wähle $y = -1$
Es gilt $y \in \R$ und $y < 0$
Sei $x \in \R$ beliebig
Es gilt $x^2 \geq  0$ (nach Lemma 2)
$\Rightarrow x^2 > y$
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

#### Aufgabe 2.8:
$M := \set{0, \es, \set{1,2}, \triangle, \unicode{9786}, x^2 + 1, 1}$ 
$|\mathcal P (M)| = 2^7 = 128$ 

wahr:
$\es \in \mathcal P (M)$
$\set{0} \in \mathcal P(M)$ 
$\set{\es} \in \mathcal P(M)$
$\set{1,\unicode{9786}} \in \mathcal P(M)$

falsch:
$\set{1,2} \in \mathcal P(M)$
$1 \in \mathcal P (M)$
$\set{1,2, \triangle} \in \mathcal P(M)$

$M \without \set{1,2} = \set{0, \es, \set{1,2},\triangle, \unicode{9786}, x^2+1}$
$M \cap \es = \es$
$M \cap \set{\es} = \set{\es}$
$M \cap \set{1,2,\triangle,\unicode{9786},x^2} = \set{1, \triangle, \unicode{9786}}$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

### Anhang
Anmerkung: Dies ist eine Sammlung von Beweisen zu verschiedenen Lemmata. Die Beweise sind dafür da, falls ein für ein Lemma ein Beweis gefordert sein sollte. Ist dies nicht der Fall können die Beweise auch unkorrigiert gelassen werden.


#### Aufgabe 2.5:
A2.5.L1:
Lemma:
Sei M eine Menge, dann gilt
$M \cap M = M$

Beweis:
$M \cap M$
$\Leftrightarrow x \in M \land x \in M$
Fallunterscheidung:
Gilt $x \in M$ dann gilt $x \in M \land x \in M$.
Gilt $x \in M$ nicht, dann gilt auch $x \in M \land x \in M$ nicht.
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

#### Aufgabe 2.6:
A2.6.L1:
Lemma:
Seien A und B Aussagen, dann gilt:
$(A \Rightarrow B) \Leftrightarrow (\lnot(A \land \lnot B))$
Beweis durch Wahrheitstafel:

 A | B | $\lnot B$ | $A \land \lnot B$ | $\lnot(A \land \lnot B)$ | $A \Rightarrow B$ 
 --- | --- | --- | --- | --- | --- 
 w | w | f | f | w | w 
 w | f | w | w | f | f 
 f | w | f | f | w | w 
 f | f | w | f | w | w 
$\blacksquare$


A2.6.L2:
Lemma:
Sei A eine Aussage, dann gilt:
$\lnot(\lnot A) \Leftrightarrow A$
Beweis durch Wahrheitstafel:

 A | $\lnot A$ | $\lnot(\lnot A)$ 
 --- | --- | --- 
 w | f | w 
 f | w | f 
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

A2.6.L3:
Lemma:
Seien $a,b \in \Z$, dann gilt:
$a \not \mid b \Rightarrow \frac{b}{a} \notin \Z$
Beweis durch Kontraposition:
z.z: $\frac{b}{a} \in \Z \Rightarrow a \mid b$ (Kontraposition)

Sei $\frac{b}{a} \in \Z$, d.h. $\exists c \in \Z: \frac{b}{a} = c$
$\frac{b}{a} = c$
$\stackrel{\cdot a}\Leftrightarrow b = c \cdot a$
$\Rightarrow \exists c \in \Z: b = c \cdot a$
$\Rightarrow a \mid b$ (nach der Definition der Teilbarkeit)
$\blacksquare$


#### Aufgabe 2.7
A2.7.L1:
Lemma:
Sei $x \in \Q: x \neq 0$
Dann ist auch $\frac{1}{x} \in \Q$
Beweis:
Sei $x \in \Q\without\set{0}$, d.h. $x = \frac{a}{b}: a \in \Z\without\set{0}, b \in \N$
$\stackrel{x \neq 0}\Rightarrow$ es gibt $\frac{b}{a}$ (auch wenn wir nicht wissen, ob es in $\Q$ liegt)
$\Rightarrow \frac{1}{x} = \frac{1}{\frac{a}{b}} = \frac{1}{\frac{a}{b}} \cdot \frac{\frac{b}{a}}{\frac{b}{a}} = \frac{\frac{b}{a}}{\frac{a}{b} \cdot \frac{b}{a}} = \frac{\frac{b}{a}}{\frac{ab}{ab}} = \frac{\frac{b}{a}}{1} = \frac{b}{a}$
Nun schauen wir uns an, was für unterschiedliche Fälle für a folgt:
Für $a > 0$ gilt direkt $a \in \N$ und damit $\frac{1}{x} = \frac{b}{a} \in \Q$

Für $a < 0$ folgt $a = -c: c \in \N$ und damit $\frac{1}{x} = \frac{b}{a} = \frac{b}{-c} = \frac{b}{-c} \cdot \frac{-1}{-1} = \frac{-b}{c}$
Da gilt $-b \in \Z$ und $c \in \N$ folgt $\frac{1}{x} = \frac{b}{a} = \frac{-b}{c} \in \Q$
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

A2.7.L2:
Lemma:
Sei $x \in \R$
Dann gilt $x^2 \geq 0$
Beweis:
Fallunterscheidung:
$(I)$
$x > 0$: 
$\Rightarrow x^2 = x \cdot x > 0$ 

x = 0:
$\Rightarrow x^2 = x \cdot x = 0 \cdot 0 = 0 \geq 0$

$x < 0$:
$\Rightarrow x = - y: y > 0, y \in \R$
$\Rightarrow x^2 = (-y)^2 = (-1 \cdot y)^2 = -1 \cdot (-1) \cdot y \cdot y = y^2 > 0$ (nach $(I)$) 
$\blacksquare$


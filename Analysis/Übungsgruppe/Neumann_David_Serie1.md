subset ## Aufgabe 1:
a)  Zu zeigen:
$\displaystyle\sum_{k = 1}^{n}{k^2} = \frac{n(n+1)(2n+1)}{6}; \forall n \in \mathbb N$

$(I)$ Induktionsanfang:
n = 1:
$\displaystyle\sum_{1}^{k=1}{k^2} = 1^2 = 1$
$\displaystyle\frac{1(1+1)(2 \cdot 1 + 1)}{6} = \frac{6}{6} = \displaystyle\sum_{1}^{k=1}{k^2}$ 

$(II)$ Induktionsschritt:
Wir wissen für ein n gilt:
$\displaystyle\sum_{k = 1}^{n}{k^2} = \frac{n(n+1)(2n+1)}{6}$
-> n+1

$\displaystyle (II.a)\sum_{k = 1}^{n+1}{k^2} = \displaystyle\sum_{k = 1}^{n}{k^2} + (n+1)^2$

$\displaystyle\frac{(n+1)(n+1+1)(2(n+1)+1)}{6}$
$\displaystyle= \frac{(n+1)(n+2)(2n+3)}{6}$
$\displaystyle= \frac{2n^3+9n^2+13n+6}{6}$
$\displaystyle= \frac{2n^3 + 3n^2 + n + 6n^2 + 12n + 6}{6}$
$\displaystyle= \frac{(2n+1)(n+1)n}{6} + (n+1)^2$
$\displaystyle\stackrel{(I)}= \displaystyle\sum_{k = 1}^{n}{k^2} + (n+1)^2$
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

b)
$\displaystyle\sum^{n}_{k=1}{(2k-1)^2}; n \in \mathbb N$
$\stackrel{a)}=\displaystyle\frac{(2k-1)(2k-1 + 1)(2(2k-1)+1)}{6}$
$\displaystyle=\frac{(2k-1)(2k)(4k-2)}{6}$
$\displaystyle=\frac{16k^3-12k^2+2k}{6}$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

c)

#### $\displaystyle (I)$ Lemma:
$\displaystyle 2n^2 > n^2 + 2n + 1, \forall(n \in \mathbb N : n \geq 5)$

Beweis:
$(I.0)$ Lemma:
$4n + 2 > 2n + 3,\forall n \geq 5$
Beweis:
Annahme:
$4n + 2 \leq 2n + 3, \forall n \geq 5$
$\displaystyle \stackrel{-(2n+2)}\Leftrightarrow$ 
$2n \leq 1$
$\displaystyle\stackrel{:2}\Leftrightarrow$
$\displaystyle n < \frac{1}{2} \rightarrow \leftarrow n \geq 5$
$\Rightarrow 4n+2 > 2n + 3, \forall n \geq 5$


$\displaystyle (I.1)\ 2n^2 > n^2 + 2n + 1$
$\displaystyle\stackrel{-n^2}\Leftrightarrow$ 
$\displaystyle n^2 > 2n + 1$

##### $\displaystyle(I.2)$ Induktionsanfang:
$n = 5$:
$\displaystyle 5^2 = 25$
$\displaystyle 2 \cdot 5 + 1 = 11$
$\displaystyle 25 > 11$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

##### $\displaystyle (I.3)$ Induktionsschritt
Wir wissen für ein n gilt:
$\displaystyle n^2 > 2n + 1$
$\displaystyle \stackrel{+(2n + 1)} \Leftrightarrow$
$\displaystyle n^2 + 2n + 1 > 4n + 2$

-> $n+1$:
$\displaystyle(n+1)^2 = n^2 + 2n + 1 \stackrel{(I.2)} \geq 4n + 2$
$(2(n+1)+1) = 2n + 3 \stackrel{(I.0)}\leq 4n + 2 \leq (n+1)^2$
$\displaystyle \blacksquare$

Zu zeigen:
$\displaystyle\forall n \in \mathbb N, n \geq 5 \Rightarrow 2^n>n^2$

#### $(II)$  Induktionsannahme:
$\displaystyle\forall n \in \mathbb N, n \geq 5 \Rightarrow 2^n>n^2$

#### $\displaystyle(III)$ Induktionsanfang:
$\displaystyle n = 5$:
$\displaystyle 2^5 = 32$
$\displaystyle 25 = 5^2$
$\displaystyle32 > 25$

#### $\displaystyle(IV)$ Induktionsschritt:
Wir wissen für ein n gilt:
$2^n > n^2$
-> n+1
$2^{n+1} = 2^{n} \cdot 2 \stackrel{(III)}\geq 2 n^2$

$(n+1)^2 = n^2 + 2n + 1 \stackrel{(I)}\leq 2n^2 \leq 2^{n+1}$
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

## Aufgabe 2:
A, B, C, M Mengen
$I$ Indexmenge
$A_i\ Menge\ \forall\ i \in I$

Lemma:
L1:
Sei X eine Menge und $\emptyset = \set{}$ die leere Menge , dann gilt:

1: $X \backslash \emptyset = X$ 
2: $X \cup \emptyset = X$
3: $X \backslash X = \emptyset$

Beweis:
1:
$X \backslash \emptyset = \set{x \mid x \in X \land x \notin \emptyset}$ 
Der rechte Teil des logischen und ist für jedes x erfüllt, da es nach der Definition kein x gibt, das Teil der leeren Menge ist.
$= \set{x \mid x \in X}$
$= X$ 
$\blacksquare$

2: $X \cup \emptyset = \set{x \mid x \in X \lor x \in \emptyset}$
Der rechte Teil des logischen oder ist nie erfüllt, da es nach der Definition kein x gibt, dass Teil der leeren Menge ist.
$= \set{x \mid x \in X}$
$= X$
$\blacksquare$

3: $X \backslash X = \set{x \mid x \in X \land x \notin X}$
Diese Aussage kann für kein x erfüllt sein (kein x kann gleichzeitig Teil und nicht Teil von X sein)
$= \set{}$
$= \emptyset$
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

a) Behauptung:
$(A\backslash B) \cup C= (A \cup C) \backslash (B \cup C)$

Wähle $(I):\ B = \emptyset = \set{}$ und $(II): A = C \neq \emptyset$

$(III)\Rightarrow A\backslash B \stackrel{I}= A \backslash \emptyset \stackrel{L1.1}= A$

$(IV)\Rightarrow B \cup C \stackrel{I}= \emptyset \cup C \stackrel{L1.2}= C$

$(V) \Rightarrow A\cup C \stackrel{II}= A \cup A = A$

$(VI)\Rightarrow (A\backslash B) \cup C \stackrel{III}= A \cup C \stackrel{V}= A$

$\Rightarrow (A \cup C)\backslash (B\cup C) \stackrel{IV}= (A\cup C)\backslash C \stackrel{V}= A \backslash C \stackrel{II}= A\backslash A \stackrel{L1.3}= \emptyset$

$\Rightarrow A = \emptyset \rightarrow \leftarrow (II): A \not = \emptyset$

$\Rightarrow$ Die Behauptung war falsch
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

Lemma:
L2: 
Seien A, B und C Mengen. Es gelten die Folgenden Relationen:

1: $A \cap (B \cup C) = (A \cap B)\cup(A\cap C)$

Beweis:
siehe Skript 1.2

2: $A \cup (B \cap C) = (A \cup B) \cap (A\cup C)$

Beweis:
$x \in (A \cup (B \cap C))$
$\Leftrightarrow x \in A \lor x \in B\cap C$
$\Leftrightarrow x\in A \lor (x \in B \land x \in C)$
$\Leftrightarrow (x \in A \lor x \in B) \land (x \in A \lor x \in C)$
$\Leftrightarrow x\in (A \cup B) \land x \in (A \cup C)$
$\Leftrightarrow x \in (A \cup B) \cap (A \cup C)$
$\blacksquare$

L3:
Seien A und B Mengen. Es gilt folgende Relation:
$A \subset A \cup B$ 

Beweis:
$A \subset A \cup B \Leftrightarrow (x \in A \Rightarrow x \in A \cup B)$
$\Leftrightarrow (x \in A \Rightarrow x \in A \lor x \in B)$
-> Fallunterscheidung:
gilt $x \notin A$ so ist die Implikation trivialer Weise wahr.
gilt $x \in A$ so ist $x \in A \lor x \in B \Leftrightarrow wahr \lor x \in B$ und somit ist die Implikation wahr.
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

b) Behauptung:
$(A \cup B) \cap C \subset A \cup (B \cap C)$

$(I) Sei\ D = (A\cup B) \cap C \stackrel{L2.1}= (A \cap C) \cup (B \cap C)$ 
$(II) Sei\ E=(A\cup B)$
$(III) A \cup (B \cap C)$
$\stackrel{L2.2}= (A \cup B) \cap (A \cup B)$
$\stackrel{II}= E \cap (A \cup C)$
$\stackrel{L2.1}= (E \cap A)\cup (E \cap C)$
$\stackrel{II}= ((A \cup B) \cap A) \cup ((A \cup B)\cap C)$
$\stackrel{L2.1}=(A\cap A)\cup (B\cap A) \cup (A \cap C) \cup (B \cap C)$
$= (A\cap C) \cup (B\cap C) \cup (A \cap A) \cup (B\cap A)$
$= ((A \cap C) \cup (B \cap C)) \cup (A \cap A) \cup (B \cap A)$
$\stackrel{I}= D \cup (A\cap A) \cup (B \cap A)$
$\stackrel{L3}\Rightarrow D \subset D \cup (A \cap A) \cup (B \cap A)$
$\Rightarrow D \subset A \cup (B\cap C)$
$\stackrel{I}\Rightarrow (A \cup B) \cap C \subset (A \cup (B\cap C))$
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

c) Behauptung:
$\displaystyle \bigcup_{i \in I}(M\backslash A_i) = M\backslash (\bigcap_{i \in I}A_i)$

Beweis:
$\displaystyle \bigcup_{i \in I}(M\backslash A_i)$
$\Leftrightarrow \set{x \mid \exists i \in I : x \in (M \backslash A_i)}$
$\Leftrightarrow \set{x \mid \exists i \in I: (x \in M \land x \not \in A_i)}$
Da i keinen Einfluss auf M hat können wir "$x \in M \land$" vor den Existenzquantor ziehen:
$\Leftrightarrow \set{x \mid x \in M \land x \in (\exists i \in I: x \not \in A_i)}$ nun negieren wir die Klammer
$\Leftrightarrow \set{x \mid x \in M \land x \in (\lnot (\forall i \in I: x \in A_i))}$ 
$\Leftrightarrow \set{x \mid x \in M \land x \notin (\forall i \in I : x \in A_i)}$
$\Leftrightarrow M\backslash {x \mid (\forall i \in I : x \in A_i)}$
$\displaystyle \Leftrightarrow M\backslash \bigcap_{i \in I}(A_i)$
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

## Aufgabe 3:
$f: \mathbb N \rightarrow \mathbb N, f(n) \leq n\ \forall n \in \mathbb N$
f bijektiv
$(I)\Rightarrow \not \exists n,n'\in  \mathbb N: f(n)= f(n') \land n \neq n'$ (Injektivität) 

Beweis durch starke Induktion:
$(II)$ Induktionsanfang:
n = 1:
$(f(1) \leq 1) \land (f(1) \in \mathbb N)$
$\Rightarrow f(1) = 1$

Induktionsschritt:
Wir wissen für alle $x \in \mathbb N: x \leq n$ bis
f(n) = n

-> n+1

$f(n+1) \leq n + 1$

$f(x) = x \forall x \in \mathbb N : x \leq n$ 
$(IV)\stackrel{I}\rightarrow f(n+1) > n$ da sonst $f(n+1) = f(x)\ für\ ein\ x\leq n$ und damit f nicht injektiv wäre
$\Rightarrow n < f(n+1) \leq n+1$
$\stackrel{-n}\Leftrightarrow 0 < f(n+1) - n \leq 1$ 
$f(n+1),n \in \mathbb N \land f(n+1) > n \Rightarrow f(n+1) - n \in \mathbb N$ 
$\Rightarrow f(n+1) - n  = 1$
$\stackrel{+n}\Rightarrow f(n+1) = n + 1$
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

#### Aufgabe 4:
a)

Notation: 
x ist durch Drei teilbar $\Leftrightarrow 3 \mid x$
(gesprochen 3 teilt x)
x ist nicht durch Drei teilbar $\Leftrightarrow 3 \not \mid x$
(gesprochen 3 teilt x nicht)

Es gelte folgende Relation (definition der Teilbarkeit):
$(I):3 \mid x :\Leftrightarrow \exists a \in \mathbb Z: 3 \cdot a = x$
Außerdem gelte:
$(II): 3 \not \mid 1 \land 3 \not \mid 2$ (für 1 wäre $a = \frac{1}{3} \notin \mathbb N$ und für 2 wäre $a = \frac{2}{3} \notin \mathbb N$)

Lemma:

L4:
$(3 \mid x) \land (3 \mid y) \Rightarrow (3 \mid x - y)$

Beweis:
$(3 \mid x) \stackrel{I}\Leftrightarrow x = 3a, a \in \mathbb Z$
$(3 \mid y) \stackrel{I} \Leftrightarrow y = 3b, b \in \mathbb Z$
$\Rightarrow x - y = 3 a - 3 b = 3 (a - b) \Rightarrow (3 \mid (x-y))$
$\blacksquare$


L5:

1: $3 \not\mid (3a + 1) \forall a \in \mathbb Z$ 

Beweis durch wiederlegung der Negation:
Annahme: Sei $a \in \mathbb Z: (3 \mid (3a + 1))$
Nach $(I)$ gilt außerdem $3 \mid 3a$
$\Rightarrow (3 \mid (3a + 1)) \land (3 \mid 3a)$ 
$\stackrel{L4}\Rightarrow 3 \mid (3a + 1 - 3a) \Leftrightarrow (3 \mid 1) \rightarrow \leftarrow II: (3 \not \mid 1)$
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

2: $3 \not \mid (3a + 2) \forall a \in \mathbb Z$ 

Beweis durch wiederlegung der Negation:
Annahme: Sei $a \in \mathbb Z: (3 \mid (3a + 2))$
Nach $(I)$ gilt außerdem $3 \mid 3a$
$\Rightarrow (3 \mid (3a + 2)) \land (3 \mid 3a)$ 
$\stackrel{L4}\Rightarrow 3 \mid (3a + 2 - 3a) \Leftrightarrow (3 \mid 2) \rightarrow \leftarrow II: (3 \not \mid 2)$
$\blacksquare$


Zu Zeigen:
$\forall n \in \mathbb N: (3 \mid n^2) \Rightarrow (3 \mid n)$
Kontraposition:
$\Leftrightarrow \forall n \in \mathbb N: (3 \not \mid n) \Rightarrow (3 \not \mid n^2)$ 
nach Lemma 5:
$\Leftrightarrow \forall n \in \mathbb N: (x = 3 a + 1 \Rightarrow (x^2 = 3 b + 1 \lor x^2 = 3b + 2)) \land$ 
$(x = 3 c + 2 \Rightarrow (x^2 = 3 d + 1 \lor x^2 = 3d + 2))),(a,b,c,d \in \mathbb Z)$ 

1: -> Sei $x = 3a +1$, $a \in \mathbb Z$
$\Rightarrow x^2 = (3a + 1)^2 = 9a^2 + 6a + 1 = 3(a^2 + 2a)$ -> wähle $b = 3a^2 + 2a$ 
$\Rightarrow x^2 = 3b + 1$

2: -> Sei x = 3c + 2, $c \in \mathbb Z$
$\Rightarrow x^2 = (3c + 2)^2 = 9c^2 + 12c + 4 = 3 (3c^2 + 4c + 1) + 1$ -> wähle $d = 3c^2 + 4c + 1$
$\Rightarrow x^2 = 3 d + 1$

$\Rightarrow [(x = 3a +1) \Rightarrow (x^2 = 3b +1) \land (x = 3c + 2) \Rightarrow (x^2 = 3d + 1), (a,b,c,d \in \mathbb Z)]$
$\Rightarrow [(3 \not \mid x) \Rightarrow (3 \not \mid x^2)]$
nach Kontrapostion
$\Leftrightarrow [(3 \mid x^2) \Rightarrow (3 \mid x)]$
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

b)
Zu zeigen:
$\sqrt3 \notin \mathbb Q$
$\Leftrightarrow \not \exists p \in \mathbb Z,q \in \mathbb N, (p,q) \ teilerfremd: \sqrt{3} = \frac{p}{q}$

Beweis durch wiederlegung der Negation:
Sei $p \in \mathbb Z$ und $q \in \mathbb N$, (p,q) teilerfremd: $\sqrt3 = \frac{p}{q}$
$\stackrel{()^2}\Leftrightarrow 3 = \frac{p^2}{q^2}$
$\stackrel{\cdot q^2}\Leftrightarrow 3 q^2 = p^2$
$\Rightarrow 3 \mid p^2$
$\stackrel{4.a} \Rightarrow 3 \mid p$ -> $p = 3a, a \in \mathbb Z$
$\Rightarrow 3q^2 = (3a)^2$ 
$\Leftrightarrow 3q^2 = 9 a^2$
$\stackrel{:3}\Leftrightarrow q^2 = 3a^2$ 
$\Rightarrow 3 \mid q^2$
$\stackrel{4.a}\Rightarrow 3 \mid q$
$\Rightarrow (3 \mid p) \land (3 \mid q) \rightarrow \leftarrow (p,q teilerfremd)$
$\Rightarrow \sqrt{3} \notin \mathbb Q$
$\blacksquare$


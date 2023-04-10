# Aufgabe 5.5
Z.z:
$(H, *)$ unteregruppe von $(G,*)$ 
$\Leftrightarrow$
1) $H \subseteq G$, $H \neq \es$
2) $\forall a,b \in H: a* b \in H$
3) $\forall a \in H: \inv a \in H$ 

Nach definition gilt:
$(H,*)$ untergruppe von $(G,*)$
$\Leftrightarrow$
$H \subseteq G$ und $(H,*)$ ist eine Gruppe.

"$\Rightarrow$"
Sei $(H, *)$ eine Untergruppe von $(G,*)$ 

Nach der Definition einer Untergruppe folgt direkt:
$H \subseteq G$ und nach der Definition einer Gruppe $H \neq \es$

Nach der Eigenschaft der wohldefiniertheit der Operation einer Gruppe folgt auch direkt:
$\forall a,b \in H: a*b\in H$ 

Und mit der Eigenschaft der existenz eines Inversen auch
$\forall a \in H: \inv a \in H$ 
$\checkmark$

"$\Leftarrow$"
Sei $(G,*)$ eine Gruppe und seien folgende Eigenschaften gegeben:
(Damit H eine Untergruppe ist, muss G eine Gruppe mit Stern bilden)
$(I)$ $H \subseteq G, H \neq  \es$
$(II)$ $\forall a,b \in H : a*b \in H$
$(III)$ $\forall a \in H: \inv a \in H$

Zu zeigen: 
$(H,*)$ ist eine Gruppe
$\Leftrightarrow$
- \* ist auf H wohldefiniert
- * ist Assoziativ auf H
- H beinhaltet das neutrale Element
- es existiert das Inverse in H

##### Wohldefiniertheit:
Folgt aus $(II)$ (bzw. ist das eigentlich genau die Definition von wohldefiniertheit)

#### Assoziativität:
Folgt daraus, das $(G,*)$ eine Gruppe bildet, und * in G und damit auch in $H \subseteq G$ ist.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

#### Existenz des neutralen Elements:
Nach $(I)$ existiert mindestens ein a in H.
Nach $(III)$ gilt:
$\inv a \in H$.
Nach $(II)$ gilt dann auch:
$a * \inv a \in H$ 
Nach der Definition des inversen gilt damit
$a*\inv a = e_* \in H$ wobei $e_*$ das neutrale Element auf * bezeichnet

Existenz des Inversen:
Folgt aus $(III)$ und der Existenz des neutralen Elements.

$\Rightarrow (H,*)$ ist eine Gruppe
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


# Aufgabe 5.6
a)

Zu zeigen:
$(G, *)$ mit $G := \set{x\in \R \mid x >1}$ , $*: G \x G \to G, (x,y) \onto xy - x - y + 2$ 
ist eine Gruppe
$\Leftrightarrow$
- $*$ ist Wohldefiniert auf G
- $*$ ist Assoziativ auf G
- $\exists e_* \in G: a * e_* = e_* * a = a \F a \in G$ (existenz des neutralen)
- $\forall a \in G \E \inv a \in G: a * \inv a = e_*$ 
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

#### Wohldefiniertheit:
Seien $a, b \in G$ beliebig. Zu zeigen:
$a * b \in G$
$\Leftrightarrow xy - x - y + 2 > 1 \F a,b \in G$ 

Wir wissen für $a,b \in G$ gilt nach der Definition von G:
$a > 1$, $b > 1$ 

$a > 1$
$\stackrel{b > 1}\Leftrightarrow ab > b$ 
$\Leftrightarrow ab - b > 0$
$\Leftrightarrow ab - b + 2 > 2$ 
$\Leftrightarrow ab - b - a + 2 > 2 - a$ 
// Mit $a > 1$ folgt $2-a > 2 - 1 = 1$
$\Leftrightarrow ab - a - b + 2 > 2- 1$
$\Leftrightarrow ab - a -b + 2 > 1$
$\Rightarrow ab - a - b + 2 \in G$ 
$\checkmark$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


#### Assoziativität:
Seien $a,b,c \in G$
Zu zeigen:
$(a*b)*c = a * (b * c)$

$(a*b)* c = (ab - a - b + 2) * c$ 
$= (ab - a - b + 2)c - (ab -a - b + 2) - c + 2$ 
$= abc - ac - bc +2c - ab + a +b -2 -c + 2$ 
$= abc - ab - ac - bc + a + b + c$ 

$a * (b *c) = a*(bc - b - c + 2)$
$= a(bc -b - c + 2) - a - (bc -b -c + 2) + 2$
$= abc - ab - ac + 2a - a -bc + b + c - 2 + 2$
$= abc - ab -ac - bc + a + b + c$ 
$= (a*b)*c$ 
$\checkmark$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

#### Existenz des neutralen Elements:
Beh.: 2 ist das neutrale Element
Beweis:
Sei $x \in G$ beliebig
$x * 2 = 2x - x - 2 + 2$
$=2x - x$
$= (2-1)x$
$= 1 x$
$= x$

$2* x = 2x - 2 - x + 2$
$= 2x -x$
$= x$
$\checkmark$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

#### Existenz des Inversen:
Wir wissen:
$2$ ist neutrales Element von G
Sei $a \in G$ beliebig so muss gelten:
$\Leftrightarrow 2 = a\inv a - a -\inv a + 2$
$\Leftrightarrow a \inv a - a - \inv a = 0$
$\Leftrightarrow \inv a (a - 1) = a$   // mit $1 < x \F x \in G$
$\Leftrightarrow \inv a = \frac{a}{a-1}$ 

Mit $a > 1$ folgt $\frac{a}{a-1} > \frac{a-1}{a-1}$
$\Rightarrow \frac{a}{a-1}> 1$
$\Rightarrow \frac{a}{a-1} \in G$ 
$\checkmark$

$\Rightarrow (G,*)$ ist eine Gruppe
$\blacksquare$ 
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

b)
Zu zeigen:
$(G,*): g = \inv g \F g \in G$ 
$\Rightarrow a * b = b * a \F a,b \in G$

Bew:
Sei $(G,*)$ eine Gruppe mit $g = \inv g \F g \in G$
Hinweis: $*$ ist assoziativ
Seien $a,b,c \in G : a*b = c$ und $e_*$ das neutrale Element von $(G, *)$
$a* b = c$
$\Leftrightarrow a * a * b = a * c$
$\Leftrightarrow b = a * c$ // ($a = \inv a$)
$\Leftrightarrow b * b = b* a * c$
$\Leftrightarrow e_* = b * a * c$
$\Leftrightarrow e_* = (b*a)*c$
$\Rightarrow (b*a) = \inv c$ 
Da das Inverse eindeutig ist folgt:
$b* a = c$ 
$\Rightarrow b*a = a*b$
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


# Aufgabe 5.7
Sei $U := \set{x \in \R \mid \E k \in \Z : x = 2^k}$ 

Zu zeigen:
$(U, \cdot)$ ist eine Untergruppe von $(\Q\without 0, \cdot)$ 
$\stackrel{A 5.5}\Leftrightarrow$ 
1.  $U \subseteq \Q, U \neq \es$
2. $\forall a,b \in U: a \cdot b \in U$ 
3. $\forall a \in U: \inv a \in U$

1.:
U ist die Menge aller ganzen Potenzen von 2.
Wir können $x \in U$ also auch schreiben als:
$x = 2^k, k \in \Z$ 
da gilt, $2^k \in \Z \F k \in \Z$ und $\Z \subseteq \Q$ folgt:
$U \subseteq \Q$ 

Da $x = 2^0 =1 \in U$ gilt folgt außerdem:
$U \neq \es$ 
$\checkmark$

2.:
Seien $a,b \in U$ also $a = 2^k, k \in \Z$ und $b = 2^j, j \in \Z$
$a \cdot b = 2^k \cdot 2^j$ //mit Potenzgesetzen:
$= 2^{k+j}$. //$k \in \Z, j \in \Z \Rightarrow k+j \in \Z$
$\Rightarrow a \cdot b \in U$ 
$\checkmark$ 

3.:
Sei $a \in U$ also $a = 2^k, k \in \Z$
$k \in \Z \Rightarrow -k \in \Z$ 
$\Rightarrow b = 2^{-k} \in U$ 
$a \cdot b = 2^k \cdot 2^{-k}, k \in \Z$
$= 2^{k-k}$ 
$= 2^{0} = 1$ 

Da $1$ das Ne.}utrale Element ist (neutrales Element der Multiplikation der rationalen Zahlen) 
folgt:
Für $a = 2^k \in U, k \in \Z: \inv a = 2^{-k} \in U$ 
$\checkmark$

Folglich ist $(U, \cdot)$ eine Untergruppe von $(\Q, \cdot)$ 
$\blacksquare$ 
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


# Aufgabe 5.8
Sei M eine Menge
und $X\triangle Y := (X \backslash Y) \cup (Y \backslash X)$ für alle Mengen X, Y
x
Zu zeigen:
$(\P(M), \triangle, \cap)$ ist ein kommutativer Ring mit Eins

Also:
1) $(\P(M), \triangle)$ ist eine kommutative Gruppe also:
	1) wohldefiniertheit
	2) assoziativität
	3) kommutativität
	4) neutralität
	5) inversivität
2) $\cap$ hat auf $\P(M)$ folgende Eigenschaften:
	1) wohldefiniertheit
	2) assoziativität
	3) neutralität
	4) kommutativität
3) Es gelten die Distributivgesetze
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

### 1: $\triangle$
#### Wohldefiniertheit:
$\triangle$ ist als Operation zwischen zwei Mengen für alle Mengen wohldefiniert.
Es gilt $X \triangle Y \subseteq X \land X \triangle Y \subseteq Y$, folglich ist $X \triangle Y$ für alle $X,Y \in \P(M)$ auch wieder in $\P(M)$

#### Assoziativität
Seien $X,Y,Z \in \P(M)$ 

Zu zeigen:
$(X \triangle Y) \triangle Z = X \triangle (Y \triangle Z)$ 

$(X \triangle Y) \triangle Z$
$= ((X\backslash Y) \cup (Y \backslash X)) \triangle Z$
$= (((X\backslash Y) \cup (Y \backslash X)) \backslash Z) \cup Z \backslash ((X\backslash Y) \cup (Y \backslash X))$ 
$\Leftrightarrow ((x \in X \land x \nin Y) \lor (x \in Y \land \x \nin X) \land x \nin Z)$
$\lor (x \in \Z \land \lnot((x \in X \land x \nin Y) \lor (x \in Y \land x \nin X)))$ 
...
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

#### Kommutativität:
Seien $X,Y \in \P(M)$
$X \triangle Y$
$= ((X \backslash Y) \cup (Y \backslash X))$ 
$= ((Y \backslash X) \cup (X \backslash Y))$ (kommutativität der Vereinigung)
$= Y \triangle X$
$\checkmark$

#### Neutralität:
Beh: Das neutrale Element auf $\triangle$ ist $\es$ 
Bew:
Sei $X \in \P(M)$
$\es \triangle X$
$= X \triangle \es$ (Kommutativität von $\triangle$)
$= (X \backslash \es \cup \es \backslash X)$
$= (X \cup \es)$
$= X$ 
$\checkmark$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

#### Inverses:
Beh: Das Inverse zu $X\in \P(M)$ ist X

Bew:
Sei $X \in \P(M)$
$X \triangle X$
$= (X \backslash X \cup X \backslash X)$
$= (\es \cup \es)$
$= \es$ 

### 2: $\cap$

#### Wohldefiniertheit
$\cap$ ist als vereinigung von zwei Mengen für alle Mengen definiert.
Es gitl $X \cap Y \subseteq X$ und $X \cap Y \subseteq Y$ folglich ist für alle $X,Y \in \P(M)$ 
$X \triangle Y$ auch wieder in $\P(M)$

#### Assoziativität:
Gilt nach der assoziativität der Schnittmenge (siehe Übung 2)

#### Kommutativität:
Gilt nach der Kommutativität der Schnittmenge (siehe Übung 2)
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

#### Neutralität:
Beh: $M$ ist das neutrale Element:
Bew:
Sei $X \in \P(M)$
$\Rightarrow X \subseteq M$ (die Potenzmenge ist die Menge aller Teilmengen von M)
$\Rightarrow x \in M \F x \in X$
$\Rightarrow M \cap X = X$ 

Nach der Kommutivität gilt somit auch
$X \cap M = X$
$\checkmark$


3: Distributivität
Seien $X,Y,Z \in \P(M)$
$(X \triangle Y) \cap Z$
$= Z \cap (X\triangle Y)$ (Kommuativität von $\cap$)
$= ((X \backslash Y) \cup (Y \backslash X)) \cap Z$
$= ((X \backslash Y) \cap Z)\cup(((Y \backslash X) \cap Z))$ 
...

$= (X \cap Z) \triangle (Y \cap Z)$ 
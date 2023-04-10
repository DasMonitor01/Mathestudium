# Aufgabe 6.5
$(R,+,*)$ ist ein Kommutativer Ring mit $1 \neq 0$ und $x,y \in R\without 0 \Rightarrow x * y \neq 0$ (keine nontrivialen Nullteiler)


## a)
$M = R \x R\without 0$
$(x,y) \tilde (u,v) :\LRA x*v = y *u$

Z.z:
$\tilde$ ist Äquivalent.

$(I)$: Reflexivität:
Es gilt $(a,b) \tilde (a,b)$
denn sei $(x,y) \in M$
$x * y = y * x$ (gilt weil * auf R kommutativ ist)
$\RA (x,y) \tilde (x,y)$
$\checkmark$

$(II)$: Symmetrie:
Es gilt $(x,y) \tilde (a,b) \LRA (a,b) \tilde (x,y)$
denn seien $(x,y),(a,b) \in M: (x,y) \tilde (a,b)$
$\RA x * b = y * a$
$\LRA b * x = a * y$
$\LRA a * y = b * x$
$\LRA (a,b) \tilde (x,y)$
$\checkmark$


$(III)$: Transitivität:
Es gilt $(x,y) \tilde (a,b) \land (a,b) \tilde (c,d) \Rightarrow (a,b) \tilde (c,d)$
denn seien $(x,y),(a,b),(c,d)\in M: (x,y)\tilde (a,b) \land (a,b) \tilde (c,d)$ 
$\RA x * b = y * a$ und $a * d = b * c$
$x * b = y * a$
$\LRA x * b * d = y * a * d$ (* ist kommutativ)
$\LRA x * b * d = y * b * c$ //($a * d = b * c$)
$\LRA x * d *b= y * c * b$ 
$\Rightarrow x*d = y * c$
$\Rightarrow (x,y) \tilde (c,d)$ 
$\checkmark$
$\RA$ $\tilde$ ist reflexiv,symmetrisch und transitiv, und somit Äquivalent
$\bs$

## b)
Im folgenden wird die Ringmultiplikation von R (also \*), kurz geschrieben mit :$a * b \LRA ab$

$[(x,y)]_{\tilde} \LRA \frac{x}{y}$
Z.z:

$\oplus: (M / \tilde) \x (M / \tilde) \to (M /\tilde), \frac{x}{y} \oplus \frac{u}{v} := \frac{xv+yu}{yv}$
ist wohldefiniert.
Also $\frac{xv+yu}{yv} \in (M / \tilde)$
$\Rightarrow$ $(xv+yu)\in R \land yv \in R\without 0$
(dann ist die Relation $\tilde$ und damit auch die Äquivalenzklasse definiert)

$(xv+yu)\in R$ gilt, da $x,v,y,u \in R$ 
($y,v \in R \without 0 \Rightarrow y,v \in R$)
und damit sind Ringmultiplikation und addition wohldefiniert.
$(yv \in R\without 0)$ gilt, da $y,v \in R\without 0$ und damit auch $y*v \in R\without 0$ weil R keine nontrivialen Nullteiler hat.
$\RA \oplus$ ist wohldefiniert.

Z.z: 
$\odot: (M / \tilde) \x (M / \tilde) \to (M / \tilde), \frac{x}{y} \odot \frac{u}{v} := \frac{xu}{vy}$
ist wohldefiniert.
Also
$xu \in R$, $vy \in R\without 0$
$xu \in R$, da $x,u \in R$ und somit ist die Ringmultiplikation wohldefiniert
$vy \in R\without 0$ weil siehe $\oplus$

$\RA \odot$ ist wohldefiniert

## c) 
Z.z:
$((M / \tilde), \oplus, \odot)$ ist ein Körper:

$\oplus$:
Wohldefiniert nach b)

Assoziativität:
Z.z: $\frac{x}{y} \oplus\left(  \frac{p}{q} \oplus \frac{r}{s} \right) = \left(  \frac{x}{y} \oplus \frac{p}{q} \right) \oplus \frac{r}{s}$

$\frac{x}{y} \oplus \left( \frac{p}{q} \oplus \frac{r}{s} \right)$
$= \frac{x}{y} \oplus$
# Aufgabe 1
a)
Z.z:
Sei $k \in \N$
Für a > 0 gilt:
$(I)$: Für $2 \mid k$ gilt:
$x^k = a$ hat zwei Lösungen:

#### Beweis:
Merke:
$a>0 \RA \sqrt[k]{a}$ existiert eindeutig (also $\sqrt[k]a$ ist die eindeutige nichtnegative Lösung der Gleichung)!
Sei $x_{1} = \sqrt[k]a$ 
$x_{1}^k = (\sqrt[k]a)^k = a \RA$ $\sqrt[k]a$ ist eine Lösung der Gleichung

außerdem gilt:
$x^k = (-x)^k \F k \in \N: 2 \mid k$
$\Rightarrow x^k = (-x)^k \F x \in \R$
Sei $x_{2} = - \sqrt[k]a$ 
$\Rightarrow x_{2}^{k} = (-\sqrt[k]a)^{k} = (\sqrt[k]a)^{k} = a$ 
$\RA -\sqrt[k]a$ ist eine Lösung der Gleichung 

Da die k-te Wurzel und auch das additive Inverse eindeutig sind, bilden diese zwei Lösungen die einzigen Lösungen von $x^{k} = a$ 

$(II)$: Für $2 \not \mid k$ gilt:
$x^{k} = a$ hat eine Lösung

#### Beweis:
Merke: $a > 0 \RA \sqrt[k]a$ existiert eindeutig (also $\sqrt[k] a$ ist die eindeutige nichtnegative Lösung der Gleichung)
Sei $x_{1} = \sqrt[k]a$
$\RA x_{1}^{k} = (\sqrt[k]a)^{k} = a$ 
$\RA$ $\sqrt[k]a$ ist eine Lösung der Gleichung.

außerdem gilt:
$(-x)^{k} = - (x)^{k} \F k \in \N: 2 \not \mid k$ 
$\RA$ es existiert keine negative Lösung, denn angenomen:
$x' < 0$ wäre eine Lösung der Gleichung also 
$(x')^{k} = a$ 

Aber sei y gegeben durch: $x' = - y : y > 0$ 
$a = (x')^{k} = (-y)^{k} = -(y)^{k} = -(-(y)^{k}) = -((-y)^{k}) = - (x')^{k} = - a$ $\contrana$ 
$\RA$ es existiert keine negative Lösung
$\RA$ $\sqrt[k]{a}$ ist die einzige Lösung der Gleichung
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

b)
Seien $x>0$, $r,s \in \Q$
$(I)$: 
Z.z: $x^{r}x^{s} = x^{r+s}$
Sei $r = \frac{p}{q}, p \in \Z, q \in\N$
und $s = \frac{v}{w}, v \in\Z, w \in \N$

$\d x^{r}x^{s}$ 
$= x^{\frac{p}{q}}x^{\frac{v}{w}}$ 
$= x^{\frac{pw}{qw}}x^{\frac{vq}{qw}}$ 
$= \sqrt[qw]{x^{pw}} \cdot \sqrt[qw]{x^{qw}}$ 
$= (x^{pw})^{\frac{1}{qw}} \cdot (x^{vq})^{\frac{1}{qw}}$ 
$\stackrel{L 4.3.I}= (x^{pw}\cdot x^{vq})^{\frac{1}{qw}}$ 
$= (x^{pw+vq})^{\frac{1}{qw}}$ *
$= \sqrt[qw]{x^{pw+vq}}$ 
$=(x)^{\frac{pw + vq}{qw}}$ 
$= (x)^{\frac{pw}{qw} + \frac{vq}{qw}}$ 
$= (x)^{\frac{p}{q} + \frac{v}{w}}$ 
$= (x)^{r+s}$ 
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

$(II):$
Z.z: $(x^{r})^{s} = x^{r \cdot s}$ 

$(x^{r})^{s}$
$= \sqrt[w]{(\sqrt[q]{x^{p}})^{v}}$
$= \sqrt[w]{((\sqrt[q]{x})^{p})^{v}}$
$= \sqrt[w]{(\sqrt[q]x)^{p \cdot v}}$
$= (\sqrt[q]{x})^{\frac{pv}{w}}$
$= (x)^{\frac{pv}{qw}}$
$= (x)^{\frac{p}{q} \cdot \frac{v}{w}}$
$= x^{r \cdot s}$
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


# Aufgabe 2
Seien a,b > 0

##### Lemma 2.1:
$(a+b)^{n} \geq a^{n} + b^{n} \F n \in \N$
##### Beweis:
$(a+b)^{n} = \Sum_{k=0}^{n} {\binom{n}{k} a^{k} b ^{n-k}}$ (Binomischer Lehrsatz)
$= \binom{n}{0} a^{0}b^{n-0} + \binom{n}{n} a^{n} b ^{n-n} + \Sum_{k=1}^{n-1} \binom{n}{k} a^{k} b^{n-k}$ 
$=b^{n} + a ^{n} + \Sum_{k=1}^{n-1} \binom{n}{k} a^{k}b^{n-k}$ 
Sei $\xi_{n} = \Sum_{k=1}^{n} \binom{n}{k} a^{k}b^{n-k}$
also $(a+b)^{n} = a^{n} + b^{n} + \xi_{n}$

Merke: $a, b >0 \RA \binom{n}{k} a^{k}b^{n-k} >0 \F n,k \in \N$ 
$\Rightarrow \xi_{n} >0$

$\xi_{n} >0$
$\Leftrightarrow \xi_{n} + a^{n} + b^{n} > a^{n} + b^{n}$
$\Leftrightarrow (a+b)^{n} > a^{n} + b^{n}$
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


#### $(I)$:
Z.z: $\sqrt[n]{a+b} \leq \sqrt[n] a + \sqrt[n] b$ 

Seien $x = \sqrt[n] a, y = \sqrt[n] b$ 

Nach Lemma 2.1 gilt:
$x^{n} + y ^{n} \leq (x+y)^{n}$
$\Rightarrow a + b \leq (x+y)^{n}$
$\LRA \sqrt[n]{a+b} \leq \sqrt[n]{(\sqrt[n] a + \sqrt[n]b)^{n}}$ 
($\uparrow$ geht weil a,b >0 also $a +b >0$ und $x + y > 0$, und somit auch $\sqrt[n]{a+b} >0$ und $\sqrt[n]{(x+y)^{n}} >0$ gilt, man kann also anwenden $u > v \LRA u^{n} > v^{n}$) 

$\RA \sqrt[n]{a+b} \leq \sqrt[n]{a} + \sqrt[n]{b}$ 
$\bs$

#### $(II)$:
Z.z:
$|\sqrt[n]a - \sqrt[n]b| \leq \sqrt[n]{|a-b|}$
...

<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

# Aufgabe 3
a)
Sei $(a_{n})_{n}$ eine Folge mit:
$a_{n}\geq 0 \F n \in \N$,
$\limin a_{n} = a$
$\Rightarrow \forall \varepsilon > 0 \E N \in \N : |a_{n} - a| < \varepsilon \F n \geq N$

Z.z: $\limin \sqrt[k]{a_{n}} = \sqrt[k] a$
$\LRA \forall \varepsilon > 0 \E N \in \N: |\sqrt[k]{a_{n}} - \sqrt[k]{a}|< \varepsilon \F n \geq N$

$a_{n} \geq 0 \F n \in \N \RA \sqrt[k]{a_{n}}$ existiert $\forall n \in \N$

Sei $\varepsilon >0$

Nach der Vorrausetzung gilt:
$\exists N_1 \in \N: |a_{n} - a|< \varepsilon^{k} \F n \geq N_{1}$

$|\sqrt[k]{a_{n}} - \sqrt[k]{a}| \stackrel{A_{2}}\leq \sqrt[k]{|a_{n}-a|}$

$|a_{n} - a| < \varepsilon^{ k} \Rightarrow \sqrt[k]{|a_{n}- a}< \sqrt[k]{\varepsilon^{k}} = \varepsilon$

$\Rightarrow |\sqrt[k]{a_{n}} - \sqrt[k]{a}|< \varepsilon \F n \geq N_{1}$ 
$\RA \limin \sqrt[k]{a_{n}} = \sqrt[k]{a}$
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


b)
Sei $a > 0$

Z.z:
$\limin \sqrt[n] a = 1$

$(I)$:
a = 1:
$\RA \sqrt[n] a = \sqrt[n] 1 = 1 \F n \in \N$
$\RA \limin \sqrt[n] a = 1$
$\checkmark$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

$(II)$:
$a > 1$:

Es gilt:
$\sqrt[n] a > \sqrt[n+1] a \F n \in \N$

Beweis durch Induktion:
Induktionsanfang:
$n = 0:$
$a > \sqrt{a}$ 

Induktionsschritt:
Wir wissen für ein $n \in N$ gilt:
$\sqrt[n] a > \sqrt[n+1] a$
$\RA n+1$

$\sqrt[n+1] a \geq \sqrt[n+1]{\sqrt[n+2]{a^{n+1}}}$
$\RA \sqrt[n+1]a \geq \sqrt[n+2]a$ 

-> die Folge $(a_{n})_{n} := \sqrt[n] a$ ist monoton fallend.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


Außerdem ist die Folge beschränkt durch dass Infimum
1:

Zu zeigen:
1.: $\sqrt[n] a > 1 \F n \in \N$

Angenommen $\sqrt[n] a \leq 1$ 
$\RA (\sqrt[n] a)^{n} \leq 1^{n}$
$\RA a \leq 1$ $\contrana$

2.: $(\exists t \in \R: x \geq t \F x \in (\sqrt[n] a)_{n}) \RA t \leq 1$
$\LRA (\exists t \in \R : \sqrt[n] a \geq t \F n \in \N) \RA t \leq 1$

Sei $t \in \R: \sqrt[n] a \geq t \F n \in \N$
$\RA \sqrt[n] a \geq t$
$\RA a \geq t^{n}$
$\RA a - t^{n} \geq 0$

Aber für $t > 1 \E n \in \N : t^{n} > a$ 
(genauer für $t^{n} > a \F n > \frac{\ln(a)}{\ln(t)} = \log_{t}(a)$)
und somit wäre $a - t^{n} < 0$ für ein n
$\RA t \leq 1$
$\RA 1 = \inf(a_{n})$

Folglich ist die Folge beschränkt und monoton fallend, also konvergiert sie gegen das Infimum 1
$\RA \limin \sqrt[n] a = 1$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


$(III)$:
$a < 1$
$\Rightarrow 0 < a < 1$
$\RA$ Sei $a':= \frac{1}{a} \LRA a = \frac{1}{a'}$ 
$\RA a' > 1$ 

$\RA\limin \sqrt[n]a = \limin \sqrt[n]{ \frac{1}{a'}}$
$= \limin \frac{\sqrt[n]{1}}{\sqrt[n]{a'}}$ 
$= \frac{\limin \sqrt[n]{1}}{\limin \sqrt[n] {a'}}$ (da beide Folgen konvergieren)
($\limin \sqrt[n]{a'}$ konvergiert weil $a' > 1$ oben behandelt wurde)
$= \frac{1}{1}$ 
$\Rightarrow \limin \sqrt[n] a = 1$
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

# Aufgabe 4
Seien $z,w \in \C$
$\Rightarrow z  = a + bi, w = c + di: a,b,c,d \in \R, i^{2} = -1$ 

Anm: 
Latex hatte bei mir Schwierigkeiten mit dem Horizontalen Balken der Komplexen Konjugation. Deshalb wird hier die Konjugation der Zahl z mit conj(z) (vom Englischen conjugate) bezeichnet werden. Ich bitte um Entschuldigung hierfür. Dafür gibt es einen $\unicode{128532}$-Smiley


a) Z.z: $conj(z + w) = conj(z) + conj(w)$ 
Beweis:
$conj(z+w)$
$=conj(a+c+bi+di)$
$=conj(a+c+(b+d)i)$
$= a+c - (b+d)i$
$= a + c - bi - di$
$= (a-bi) + (c - di)$
$= conj(a+bi) + conj(c+di)$
$= conj(z) + conj(w)$ 
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

b)
Z.z: $\conj(z \cdot w) = conj(z) \cdot conj(w)$
Beweis:
$conj(z \cdot w)$
$= conj((a+bi) \cdot (c+di))$
$= conj(ac - bd + adi + bci)$ 
$= conj(ac - bd + (ad + bc)i)$
$= ac - bd - (ad + bc) i$
$= ac - bd - adi - bci$
$= (a-bi) \cdot (c - di)$
$= conj(z) \cdot conj(w)$ 
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

c)
$x^{2} > 0$
$\RA 0 \leq (ad-bc)^{2}$
$\RA 0 \leq (ad)^{2}+(bc)^{2}-2acbd$
$\RA$ $2ac b d \leq (ad)^{2} + (bc)^{2}$
$\RA (ac)^{2} + (bd)^{2} + 2 ac b d \leq ac^{2}+ ad^{2}+bc^{2}+bd^{2}$
$\RA (ac + bd)^{2} \leq (a^{2} + b^{2}) \cdot (c^{2}+ d^{2})$
da alle Terme nichtnegativ und reell sind, können wir die eindeutig Definierte nichtnegative Wurzel anwenden
$\RA ac + bd \leq \sqrt{(a^{2}+b^{2})(c^{2}+d^{2})}$
Wir rekonstruiren nun einen größeren Term (und spalten die Wurzel auf):
$\RA a^{2} + c^{2} + 2ac + b^{2} + d^{2} + 2bd$ 
$\leq a^{2} + b^{2} + c^{2} + d^{2} + 2 \sqrt{a^{2}+b^{2}}\cdot \sqrt{c^{2}+d^{2}}$
$\Rightarrow (a+c)^{2} + (b+d)^{2} \leq (\sqrt{a^{2}+b^{2}} + \sqrt{c^{2}+d^{2}})^{2}$
erneut können wir die eindeutig definierte nichtnegative Wurzel ziehen und erhalten:
$\RA \sqrt{(a+c)^{2} + (b+d)^{2}} \leq \sqrt{a^{2} + b^{2}} + \sqrt{c^{2} + d^{2}}$
$\RA |a+c+(b+di)|\leq |a+bi| + |c+di|$
$\RA |z+w|\leq |z| + |w|$
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

d)
Z.z: $|z+w|^{2} + |z - w|^{2} = 2(|z|^{2} + |w|^{2})$
Beweis:
$|z+w|^{2} + |z - w|^{2}$
$= |a+bi + c +di|^{2} + |a + bi - (c + di)|^{2}$
$= |(a+c) + (b+d)i|^{2} + |(a -c) + (b-d)i|^{2}$
$= (a+c)^{2} + (b+d)^{2} + (a-c)^{2} + (b-d)^{2}$ //($|a+bi| := \sqrt{a^{2} + b^{2}}$)
$= a^{2} + c^{2} + 2ac + b ^{2} + d^{2} + 2bd + a^{2} + c ^{2} - 2ac + b^{2} + d^{2} -2bd$
$=2(a^{2}+b^{2}+c^{2}+d^{2})$
$=2((\sqrt{a^{2}+b^{2}})^{2} + (\sqrt{c^{2}+d^{2}})^{2})$
$=2(|a+bi|^{2} + |c+di|^{2})$
$=2(|z|^{2} + |w|^{2})$
$\bs$
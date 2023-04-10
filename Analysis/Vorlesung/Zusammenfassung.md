# Funktionen
Im Folgenden steht $\mathbb K$ für den Körper $\R$ oder $\C$ und $D \subset \K$ ist eine beliebige Teilmenge.

## Def:
Sei $f,g: D \to \K$ und $\lambda \in \K$.
Wir definieren $f+g, f \cdot g, \lambda f : D \to \K$ durch:
$(f+g)(x) := f(x) + g(x)$
$(f \cdot g)(x) := f(x) \cdot g(x)$
$(\lambda f)(x) := \lambda f(x)$

Für $D' := \{ x \in D : g(x) \neq 0 \}$ ist $\left( \frac{f}{g} \right): D' \to \C, x \onto \frac{f(x)}{g(x)}$.

## Def:
$f: D \to N$ mit $D \subseteq \K$ heißt reellwertig, falls $N \subseteq \R$, komplexwertig, falls: $N \backslash \R \neq 0$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

# Stetigkeit
## Def:
Eine Funktion $f: D \to \K$ heißt stetig in $x_{0} \in D,$ falls 
$\forall \varepsilon > 0 \E \delta > 0: (|x-x_{0}|< \delta, x \in D \RA |f(x)-f(x_{0})|< \varepsilon)$

f heißt stetig, falls stetig in jedem $x_{0} \in D$ 

Bsp: 
1)
$abs: \R \to \R, x \onto |x|$ ist stetig
Sei $x_{0} \in \R$ und $\varepsilon >0$ beliebig.
$||x|-|x_{0}|| \leq ||x-x_{0}|| = |x-x_{0}|<\varepsilon$
für alle x mit $|x-x_{0}|< \delta$ und $\delta = \varepsilon$
$\RA$ abs ist stetig

2)
$X_{[0,1]}:\R \to \R, x \onto\biggl \{ \begin{matrix} 0: x \not \in [0,1] \\ 1 : x\in [0,1]\end{matrix}$
ist nicht stetig in $x=0$ (und in x=1)

Bew:
sei z.B. $\varepsilon = \frac{1}{2}$
$\forall x < 0$ ist $|f(x) - f(0)| = |0-1|=1 > \varepsilon$
d.h. es gibt kein $\delta >0$, s.d.
$|x-0|< \delta \RA |f(x)-f(0)|< \varepsilon$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

#### Bem:
Für $A \subset\K$ heißt $X_{A}: \K \to \R, x \onto \biggl \{ \begin{matrix} 1: x \in A \\0 : x \not \in A\end{matrix}$
die charakteristische Funktion von A.

## Def:
$f: D \to \K$ heißt Lipschitzstetig, falls 
$\exists L > 0: |f(x)-f(y)|\leq L|x-y| \F x,y \in D$
(d.h. Betrag der Steigung jeder Sekante ist durch L beschränkt)
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

# Proposition 8.1
Jede Lipschitzstetige Funktion ist stetig.
### Bew: 
Sei $f: D \to \K$ Lipschitzstetig: 
Sei $\varepsilon > 0$, $x_{0} \in D$ beliebig.
$|f(x) - f(x_{0})|\leq L |x- x_{0}|$ $\forall x \in D$
$< \varepsilon$ falls $|x-x_{0}|< \frac{\varepsilon}{L}$
wähle also $\delta := \frac{\varepsilon}{2}$

Bsp.:
1)
$abs : \R \to \R$ ist Lip-stetig mit L=1,
weil $||x|-|y||\leq |x-y|$
2)
$f: (0, \infty) \to \R, x \onto \frac{1}{x}$ ist stetig, aber nicht Lip-stetig.

a) Stetigkeit:
Sei $\varepsilon >0$ und $x_{0} \in (0,\infty)$
$|\frac{1}{x}- \frac{1}{x_{0}}| = \frac{1}{|x||x_{0}|} \cdot |x_{0}-x|$

$\leq \frac{1}{|x_{0}-\delta||x_{0}|} \delta$, falls $\delta < x_{0}, |x-x_{0}|<\delta$
$= \frac{\delta}{(x_{0}-\delta)x_{0}}$
$= \frac{\delta}{x_{0}^{2}-\delta x_{0}}< \varepsilon$, falls $\delta < \varepsilon (x_{0}^{2}-\delta x_{0})$, dh.
$\delta (1+ \varepsilon x_{0})< \varepsilon x_{0}^{2}$, dh.
$\delta < \frac{\varepsilon x_{0}^{2}}{1+ \varepsilon x_{0}}$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

b) 
Lip-stetigkeit:
$\frac{1}{x} - \frac{1}{y_{k}} \to - \infty$ für beliebiges (festes) $x>0$ und $(y_{k}) \subset(0,\infty)$ mit $y_{k} \to 0$, aber $|x-y_{k}|$ bleibt beschränkt ($\to$ beliebig große Steigung der Sekanten)
Im Detail:
Angenommen $L >0$ ist s.d. $|\frac{1}{x} -\frac{1}{y}| \leq L |x-y| \F x,y \in (0,\infty)$

Sei $x > 0$ fest.
$|\frac{1}{x} - \frac{1}{y}| = \frac{1}{|x||y|}|x-y|$

Für $|y| < \frac{1}{L|x|}$ ist $\frac{1}{|x||y|}> L$ $\contrana$ 
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

# Propostion 8.2
$\exp: \C \to \C$ ist stetig.
### Bew: 
1) Stetigkeit in $z_{0}=0$

Für $|z- z_{0}| = |z|<\delta$ gilt:
$|\exp(z)-\exp(0)| = |\Sum_{k=0}^{\infty} \frac{z^{k}}{k!} - 1| = |\Sum_{k=1}^{\infty} \frac{z^{k}}{k!}|$
$\stackrel{S.6.14}\leq 2 \cdot \frac{|z|}{1} = 2|z| < 2 \delta$ $\F |z|\leq 1$
Sei $\varepsilon >0$. Dann ist $|\exp(z)-\exp(0)|<\varepsilon$, falls $|z|< \delta:= \left\{  \frac{\varepsilon}{2}, 1\right\}$

2) Stetigkeit in $z_{0} \in \C$ beliebig.
Sei $\varepsilon >0$
$|\exp(z) - \exp(z_{0}| = |\exp(z_{0})(\exp(z-z_{0} )-1)|$
$= |\exp(z_{0})| \cdot |\exp(z-z_{0}) - \exp(0)|$
$< |\exp(z_{0})| \cdot \frac{\varepsilon}{|\exp(z_{0})|}$ falls $|z-z_{0}|< \delta := \min \left\{  \frac{\varepsilon}{2|\exp(z_{0})|}, 1\right\}$
$= \varepsilon$
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

#### Bem:
Für $x \in \K$ und $\varepsilon >0$ sei $B_{\varepsilon}(x) := \{ y \in\K:|y-x|< \varepsilon \}$
d.h. der offene Ball mit Radius $\varepsilon$, Mittelpunkt x.

# Def:
Sei $A \subseteq \K$.
1) $x \in \K$ heißt Häufungspunkt von A, falls gilt:
$\forall \varepsilon>0$ hat die Menge $B_{\varepsilon}(x) \cap A$ unendlich viele Punkte.

2) $x \in A$ heißt isolierter Punkt, falls $\exists \varepsilon > 0$:
$B_{\varepsilon}(x) \cap A = \{ x \}$

z.B. 
$A=\{ 0 \} \cup (1,5)$
$x = 0$ ist isolierter Punkt
$x = 1,2$ sind Häufungspunkte.

#### Bem:
1) Für $x \in A \subset \K$ gilt:
$x$ ist HP von A $\LRA$ x ist kein isol. Punkt

2) Im isol. Punkt $x_{0} \in A$ ist $f: A \to \K$ immer stetig.
(da für $\delta$ klein genug die Bedingung $|x-x_0|< \delta, x \in A$ nur für $x= x_{0}$ gilt.)

# Def:
1) Sei $D \subset \K, f: D \to K$ und sei $x_{0}\in K$ ein HP von D

f konvergiert gegen $a \in \K$ für x gegen $x_{0}$, falls gilt:
$\forall \varepsilon >0 \E \delta>0: (|f(x)-a|<\varepsilon : |x-x_{0}|<\delta, x \in A)$

Notation:
- $f(x) \to a$, für $x \to x_{0}$
- $\Lim_{x\to x_{0}} =a$

2) Für $D \subset \K, f: D \to \R$ und einen HP $x_{0} \in \K$
heißt $\Lim_{x\to x_{0}}f(x) = \infty$
dass $\F M \in \R \E \delta >0: (x \in D, |x-x_{0}|< \delta \RA f(x)>M)$

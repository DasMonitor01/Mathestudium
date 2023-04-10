# Aufgabe 1
### a)
Sei $f: \R \to \R, x \onto \biggl \{ \begin{matrix} x: x \in \Q \\ 1-x : x \in \R\end{matrix}$

Beh:
f ist nicht stetig
f ist stetig auf $\frac{1}{2}$

Bew:
Sei $x_{0} = \frac{1}{2} \in \Q$

Z.z:
$\forall \varepsilon>0 \E \delta > 0: |x- x_{0}|< \delta \RA |f(x)-f(x_{0})|$
Sei $\varepsilon >0$
Zwei Fälle:
$x \in \Q$:
$f(x) = x$
$|x- \frac{1}{2}|< \delta \RA |x- \frac{1}{2}|< \varepsilon$
wenn $\delta = \varepsilon$ gewählt wird.

$x \in \R:$
$f(x) = 1- x$
$|x- \frac{1}{2}|< \delta$ 
$\RA|1 - x - \frac{1}{2}| = |x + \frac{1}{2} - 1| = |x- \frac{1}{2}|<\varepsilon$ für $\delta = \varepsilon$

$\RA \F \varepsilon$ wähle $\delta = \varepsilon$, damit gilt: $|x- \frac{1}{2}| < \delta \RA |f(x_{0}) - \frac{1}{2}| < \varepsilon$
$\checkmark$

Nicht stetig für $x_{0} \neq \frac{1}{2}$:
...

### b)
Sei $f: \N \to \R$ eine Funktion
Z.z:
f ist stetig
$\LRA \forall \varepsilon > 0\E \delta > 0: |x-x_{0}| < \delta \RA |f(x)-f(x_{0)}|<\varepsilon$

Beweis:
Sei $x_{0} \in \N$ beliebig
Sei $\varepsilon > 0$ beliebig
Betrachte $\d\delta =\frac{1}{2}$

$x_{0},x \in \N \RA x-x_{0}\in \Z \RA |x-x_{0}| \in \N$

$\RA |x-x_{0}| \neq 0 \RA |x-x_{0}| \geq 1$
$\RA x \neq x_{0} \RA |x-x_{0}| \geq 1$

$\RA |x-x_{0}|< \delta \LRA |x-x_{0}|< \frac{1}{2} \RA x = x_{0}$
$\RA |x-x_{0}|< \delta \RA |f(x) -f(x_{0})| = |f(x) - f(x)| = 0 < \varepsilon$
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

# Aufgabe 2
### a)
...

### b)
1) $(0,1)$
Sei $f: (0,1) \to (0,1),f(x) = 0.9 + 0.1 \cdot x$

$f$ ist stetig weil Lipschitz:
Seien $x,y \in (0,1)$
Z.z: $|x-y| \leq L|0.9+0,1x - (0.9 + 0.1y)|$
$\LRA |x-y| \leq L|0.1x - 0.1y|$
Sei L = 10
$|x-y| \leq 10 |0.1x-0.1y|$
$|x-y| \leq |x-y|$
$\checkmark$

Kein Fixpunkt:
Angenommen ein Fixpunkt existiert:
$f(x_{0}) = x_{0}$
$0.9 + 0.1 \cdot x_{0} = x_{0}$
$0.9 = 0.9x_{0}$
$x_{0} = 1$
Aber 1 liegt außerhalb des Definitionsbereichs, folglich hat f keinen Fipunkt
$\checkmark$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

2) $[0,\infty)$

Sei $f: [0,\infty) \to [0,\infty), x \onto 2x+1$

Stetig weil Lipschitzstetig:
Seien $x,y \in [0,\infty)$
Zu zeigen:
$\exists L:|x-y| \leq L |2x+1 - (2y+1)|$
$\LRA |x-y| \leq L |2x -2y|$
Wähle $L = \d \frac{1}{2}$
$\RA |x-y|  \leq |x-y|$
$\checkmark$

Kein Fixpunkt:
Angenommen ein Fixpunkt exisitiert:
$f(x_{0}) = x_{0}$
$x_{0} = 2x_{0} + 1$
$0 = x_{0}+1$
$x_{0} = -1$
aber $-1 \nin [0,\infty)$
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

# Aufgabe 3
Sei $f: [0, \infty) \to \R, x \onto \sqrt x$

### a)
z.z:
$\forall \varepsilon > 0 \E \delta >0: |x-x_{0}|< \delta \RA |f(x)-f(x_{0})|<\varepsilon$
$\LRA \forall \varepsilon >0 \E \delta > 0 : |x- x_{0}| \RA |\sqrt x - \sqrt{ x_{0}}|$

Sei $x_{0} \in [0,\infty)$, $\varepsilon>0$
$|\sqrt x - \sqrt{x_{0}}| \leq \sqrt{|x-x_{0}|} < \sqrt{\delta}$

Wähle $\delta = \varepsilon^{2}$
$\RA |\sqrt x - \sqrt{x_{0}}| < \varepsilon$
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

### b)
Angenommen: $\exists L > 0: |\sqrt{x}-\sqrt{y}| \leq L \cdot |x-y| \F x,y \in [0,\infty)$

Betrachte $x =0, y = \frac{1}{L^{2}}$

$\RA |0- \frac{1}{\sqrt{L^{2}}}| \leq L \cdot |0 - \frac{1}{L^{2}}|$
$\frac{1}{L} \leq L \cdot |\frac{-1}{L^{2}}|$
$\frac{1}{L} \leq \frac{1}{L}$
$\RA 1 \leq L$

Betrachte $x = 0, y = \frac{1}{L^{4}}$

$\RA |0- \frac{1}{L^{4}}| \leq L \cdot |0 - \frac{1}{L^{4}}|$

$\RA \frac{1}{L^{4}} \leq L \cdot \frac{1}{L^{4}}$
$\RA \frac{1}{L^{4}} \leq \frac{1}{L^{3}}$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

### c)
Z.z:
Sei $f_{\delta}: [\delta,\infty), x \onto \sqrt x$
Zu zeigen:

$\forall \delta >0 \E L > 0 \F x,y \in [\delta,\infty): |\sqrt x - \sqrt y| \leq L \cdot |x-y|$

$\RA L \geq \frac{|\sqrt x - \sqrt y|}{|x-y|}$

ObdA. sei $x > y \RA \sqrt x \geq \sqrt y$
$\RA \frac{\sqrt{x}-\sqrt{y}}{x-y} \leq L$

$\LRA \frac{\sqrt{x}-\sqrt y}{(\sqrt x - \sqrt y) \cdot (\sqrt x + \sqrt y)} \leq L$

$\stackrel{x > y}\LRA \frac{1}{\sqrt{x} + \sqrt{y}} \leq L$

Es gilt für $a,b > 0$:
$a > b \LRA a^{2} > b^{2}$
$\RA a = \sqrt x, b = \sqrt y$
$\RA (x > y \LRA \sqrt x > \sqrt y)$

$\RA y \in [\delta, \infty) \RA y \geq \delta$
$\RA \frac{1}{y} \leq \frac{1}{\delta}$
$\RA \frac{1}{\sqrt y} \leq \frac{1}{\sqrt{\delta}}$
$\RA \frac{1}{\sqrt{x}+ \sqrt y} \leq \frac{1}{\sqrt{x} + \sqrt{\delta}} \leq L$

Analog für x:
$\RA \frac{1}{\sqrt x} \leq \frac{1}{\sqrt\delta}$

Aber achtung: Es gilt $x > y$. Folglich gilt nur folgende ungleichung:
$\frac{1}{\sqrt x + \sqrt y} \leq \frac{1}{\sqrt x + \sqrt \delta} \leq \Lim_{x \to \delta} \frac{1}{\sqrt{x} + \sqrt \delta} \leq L$
$\RA L \geq \frac{1}{2\sqrt{\delta}}$
(das ist auch der kleinste mögliche L-Wert)
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

# Aufgabe 4
Erinnerung: 
$B_{\varepsilon} (x) := \{ y \in \K : |y-x| < \varepsilon\}$
d.h. die Menge aller $y$, die $\varepsilon-$nah an x liegen.

Häufungspunkt:
$\forall \varepsilon > 0: B_{\varepsilon}(x) \cap A$ hat unendlich viele Elemente, dass heißt, die Menge liegt unendlich Dicht um x

Isolationspunkt:
$\exists \varepsilon > 0: B_{\varepsilon}(x) \cap A = \{ x \}$, dass heißt, x liegt ab einem gewissen Intervall diskret.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

### a)
Sei $A \subseteq \K$, $x \in A$

Z.z:
$x\ HP \LRA x\ kein\ IP$

"$\RA$"
Sei x HP A:
$\RA \F \varepsilon >0$ hat $B_{\varepsilon}(x)\cap A$ unendlich viele Elemente
$\RA B_{\varepsilon}(x)\cap A \neq \{ x \} \F \varepsilon >0$
$\RA x$ ist kein IP

"$\LA$"
Sei x kein IP:
$\RA \forall\varepsilon>0 : B_{\varepsilon}(x) \cap A \neq \{ x \}$
aber $\{ x \} \subseteq B_{\varepsilon}(x) \cap A \F \varepsilon > 0$
$\RA \exists y : |y-x|< \varepsilon \F \varepsilon>0$
$\RA \E [-y;y]: |y-x|<\varepsilon$
$\RA B_{\varepsilon}(x) \cap A$ hat unendlich viele Elemente $\F\varepsilon >0$ (weil ein Intervall immer unendlich viele Elemente hat)
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

### b)
Sei $A := \left\{  \frac{1}{n} : n \in \N  \right\} \cup (1,3]$

Beh:
- $x_{0}: x_{0} \in (1,3]$ ist HP (das ist ja schon fast trivial)
- $x : x = \frac{1}{n} : n \in \N, n \geq 2$ ist IP
- 1 ist HP
- 0 ist HP

Beweise:

$x_{0} : x_{0} \in (1,3]$ HP:
Folgt trivialerweise aus der Defintion des Intervalls, oder allternativ auch aus Korrolar 2.4 folgt trivialerweise, dass unendlich viele Punkte dicht um $x_{0}$ liegen. ($\F \varepsilon >0 \E a_{n} := \biggl \{ \begin{matrix} \frac{\varepsilon + x_{0}}{2} : n=1 \\ \frac{a_{n-1}+x_{0}}{2} : sonst\end{matrix}$ wobei alle Glieder von $a_{n}$ in der $\varepsilon$-Region liegen, und $B_{\varepsilon}(x_{0})\cap A$ somit unendlich viele Elemente hat.)
$\checkmark$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

1 HP:
$\F \varepsilon >0$ definiere $a_{n} := \biggl \{ \begin{matrix}\frac{\varepsilon+1}{2}: n=1\\ \frac{a_{n-1} + 1}{2}: n > 1\end{matrix}$

$\RA |1-a_{n}|\leq |1 - \frac{\varepsilon+1}{2}| = | \frac{2}{2} - \frac{\varepsilon+1}{2}|$
$= | - \frac{\varepsilon-1}{2}| = | \frac{\varepsilon-1}{2}| = \frac{\varepsilon-1}{2} <\varepsilon$
$\RA$ Alle glieder von $a_{n}$ liegen in $B_{\varepsilon}(1)$
$\RA B_{\varepsilon}(x) \cap A$ hat unendlich viele Elemente
$\RA 1$ ist HP
$\checkmark$

$x: x = \frac{1}{n}: n \in\N, n\geq 2$ IP:
Wähle für $x_{0}= \frac{1}{n}$, $\varepsilon = \frac{1}{(n+1)^{2}}$
Es gilt:
$|1 - \frac{1}{n}| = \frac{n-1}{n} > \frac{n-1}{n^{2}+1} = \frac{1}{n+1} > \frac{1}{(n+1)^{2}} = \varepsilon$
$\RA 1$ liegt nicht in der $\varepsilon$-Region

Außerdem gilt:
$| \frac{1}{n} - \frac{1}{n-1}| = | -\frac{1}{n \cdot (n-1)}| > \frac{1}{(n+1)^{2}} = \varepsilon$
$\RA$ vorherige Glieder von $\frac{1}{n}$ liegen nicht in der $\varepsilon-$Region
und 
$| \frac{1}{n}- \frac{1}{n+1}| = \frac{1}{n(n+1)} > \frac{1}{(n+1)^{2}} = \varepsilon$
$\RA$ Folgeglieder liegen nicht mehr in der $\varepsilon$-Region
$\RA B_{\frac{1}{(n+1)^{2}}}(x_{0}) \cap A = \{ x_{0} \}$
$\checkmark$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

0 HP:
Es gilt $\limin \frac{1}{n} =0$
$\RA \F\varepsilon>0 \E N \in\N: |0- \frac{1}{n}|< \varepsilon \F n \geq N$

$\RA$ Es liegen alle $n \geq N$, also unendlich viele Glieder in $B_{\varepsilon}(0)$
$\RA B_{\varepsilon}(0) \cap A$ hat unendlich viele Glieder
$\RA 0$ ist HP
$\bs$

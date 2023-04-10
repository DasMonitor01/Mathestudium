## A1
### a)
$f: \R \to \R$ stetig mit $\Limin x f(x)= \Lim_{x \to -\infty}f(x) = 0$
Z.z:
f nimmt Minimum an oder f nimmt maximum an

Fallunterscheidung:
$\inf f(\R) = 0$:

gilt zusätzlich $\sup f(\R) = 0$
so folgt $f(x) = 0 \F x \in\R \RA \max(f(\R)) = \min(f(\R)) = 0$
(diese Aussagen sind sogar äquivalent, 
d.h. $f(x) = 0 \F x \in \R \RA \sup f(\R) = 0$)

gilt $s = \sup(f(\R)) > 0$:
Da f stetig in $\R$ ist und $\Limin x f(x) = 0 = \Lim_{x \to -\infty} f(x)$ folgt, dass $s \in \R$ gelten muss (sonst wäre f an einer Stelle nicht definiert)
Außerdem gilt nach oben: $\E x_{0} \in \R: f(x_{0}) > 0$, da sonst $\sup(f(\R)) = 0$ gelten müsste.

$\RA \E s \in \R: s \geq f(x) \F x \in \R$ (erster Teil der Definition des supremums)

Damit gilt aber $\E x_{s} \in \R: s \geq f(x_{s}) \geq f(x) \F x \in \R$,
denn sonst müsste gelten:
$\F x_{s} \in \R: s < f(x_{s}) \lor f(x_{s}) < f(x) \F x \in \R$
da aber $s \geq f(x) \F x \in \R$ gilt und $f(x_{s}) = f(x_{s})$, muss folgen, dass es mindestens ein größtes $x_{s}$ geben muss.
Da aber gilt $f(x_{s}) \geq f(x) \F x \in \R$ folgt $f(x_{s}) = \max(f(\R)) = \sup(f(\R)) = s$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

$\inf(f(\R)) < 0$:

Sei $i := \inf(f(\R))$
Da f stetig in $\R$ ist und $\Limin x f(x) = 0 = \Lim_{x\to -\infty} f(x)$ folgt auch, dass $i \in \R$ gelten muss (sonst hätte f erneut eine Lücke)

$\RA \E i \in \R: i \leq f(x) \F x \in \R$ (erster Teil der Definition des Infimum)

Damit gilt aber $\E x_{i}\in \R : i \leq f(x_{i}) \leq f(x) \F x \in \R$,
denn sonst müsste gelten $\F x \in \R: i \geq f(x_{i}) \lor f(x_{i}) > f(x)$,
da aber $i \leq f(x) \F x \in \R$ gilt und $f(x_{i}) = f(x_{i})$, muss folgen, dass es mindestens ein kleinstes $x_{i}$ geben muss.
Da aber gilt $f(x_{i}) \leq f(x) \F x \in \R$ folgt $f(x_{i}) = \min(f(\R)) = \inf(f(\R)) = i$

Folglich nimmt f entweder maximum oder minimum an
$\bs$

### b)

Z.z:
$\epta |x - y| < \delta \RA |f(x) - f(y)| < \varepsilon \F x, y \in \R$

<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


## A2
#### a)
$f: [0; \infty) \to f([0;\infty)), f(x) := \frac{1}{1+x^{2}}$

Z.z:
f ist bijektiv $\LRA$ f ist injektiv und surjektiv

surjektiv: 
Folgt direkt aus der Definition der Zielmenge der Funktion als Bild
(siehe Skript Seite 7 def. 2.)

injektiv:
z.z:
$\F x, x'\in [0,\infty): f(x') = f(x) \RA x = x'$

Seien $x,x' \in [0,\infty): f(x) = f(x')$
$\RA \frac{1}{1+x^{2}} = \frac{1}{1+(x')^{2}}$
$\LRA 1+ x^{2} = 1+ (x')^{2}$
$\LRA x^{2} = (x')^{2}$
// da $x \in [0,\infty)$, ist die Lösung dieser Gleichung die eindeutig bestimmte nichtnegative Wurzel
$\stackrel{\sqrt{\ }}\LRA x = x'$
$\checkmark$

$\RA$ f ist surjektiv und injektiv, und damit bijektiv

Umkehrfunktion:
Die Inverses zu f ist $\inv f : f([0,\infty)) \to [0,\infty), x \onto \sqrt{\frac{1}{x}-1}$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

Beweis:
Betrachte $f \circ \inv f (x)= \inv f\left( \frac{1}{1+x^{2}} \right) = \sqrt{\frac{1}{\frac{1}{1+x^{2}}}-1}$
$= \sqrt{1+x^{2}-1}$
$= \sqrt{x^{2}}$
$= x$
$= id(x)$

Betrachte $\d \inv f \circ f (x) = f\left( \sqrt{\frac{1}{x}-1} \right) = \frac{1}{1+ \left( \sqrt{\frac{1}{x} - 1} \right)^{2}}$
$= \frac{1}{1+ \frac{1}{x} - 1}$
$= \frac{1}{\frac{1}{x}}$
$= x$
$= id(x)$

// anm.: $\sqrt{\frac{1}{x}-1}$ ist in der inversen stehts definiert, da gilt $f([0,\infty)) = (0,1]$ und damit ist $\frac{1}{x} \geq 1$

### b)
...

<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

## Aufgabe 3

### Lemma 1:
Sei $f : \R \to \R$ eine Funktion, und sei $f_{x} : [x,\infty) \to \R, \alpha \in \R$ eine Einschränkung dieser Funktion
Gilt $f_{\beta} : \beta = \gamma + \delta$ gleichmäßig stetig$\F \delta > 0$ und $f_{\gamma}$ stetig in $\gamma$, so ist $f_{\gamma}$ gleichmäßig stetig

Beweis:
Z.z:$\F \varepsilon > 0 \E \delta >0: |x-y|< \delta \RA |f(x)-f(y)|< \varepsilon \F x,y \in [\gamma, \infty)$

ObdA sei $x \leq y$ (weil $|x-y| = |y-x|$)

Fallunterscheidung:
$x > \gamma$ (also auch $y > \gamma$):

$x > \gamma \LRA x - \gamma > 0$
Sei $\delta_{1} = x - \gamma \LRA x = \gamma + \delta_{1}, \delta_{1} > 0$
$\RA f_{x}$ ist nach vorraussetzung gleichmäßig stetig.
$\RA \F \varepsilon >0 \E \delta > 0 : |x-y| < \delta \RA |f(x) - f(y)|< \varepsilon \F x,y \in [\gamma + \delta_{1}, \infty)$

$x = \gamma$:

Z.z: $\F \varepsilon > 0 \E \delta > 0 : |\gamma - y| < \delta \RA |f(\gamma) - f(y)| < \varepsilon \F y \in [\gamma, \infty)$
Diese Vorrausetzung ist genau die Stetigkeit um $\gamma$, und ist somit auch nach vorraussetzung erfüllt.

$\RA$ $f_{\gamma}$ ist gleichmäßig stetig
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

### a)
Merke: $f:[0, \infty) \to \R, x \onto \sqrt{x}$ ist stetig (siehe Übung 9 Aufgabe 3 a) und damit auch stetig in $x_{0} = 0$.
Außerdem ist $f_{\delta}: [\delta, \infty) \to \R, x \onto \sqrt{x}$ Lipschitzstetig für alle $\delta > 0$, und damit auch gleichmäßig stetig für alle $\delta > 0$ (siehe Übung 9 Aufgabe 3 c)
Nach Lemma 3.1 ist f somit gleichmäßig stetig
$\bs$

### b)
Beh: $(f_{n})_{n \in \N}$ folge von Funktionen mit $f_{n} : [0,1] \to \R$ stetig $\F n \in \N$, $f: [0,1]$
$f(x) = \Lim_{n \to \infty} f_{n}(x) \F x \in [0,1] \RA f(x)$ stetig

Gegenbeispiel:
Betrachte $(f_{n})_{n \in \N}: f_{n}:= \Biggl \{ \begin{matrix} 0 : x \leq \frac{1}{2} \\ 1: x > \frac{1}{2}+\frac{1}{n} \\ n \cdot ( x - \frac{1}{2}): sonst \end{matrix}$

Offensichtlich ist $f_{n}$ stetig $\F n \in \N$:
Lipschitzstetig mit Lipschitzkonstante $L= n$


$\Lim_{n \to \infty}f_{n}(x) = f(x) = \biggl \{ \begin{matrix} 0: x \leq \frac{1}{2} \\ 1: x > \frac{1}{2}\end{matrix}$
($\limin \frac{1}{2} + \frac{1}{n} = \frac{1}{2}$, also fällt der dritte fall Weg)

Offensichtlich ist $f(x)$ nicht stetig, denn für $\varepsilon = \frac{1}{2}, x_{0}= \frac{1}{2}$ ist $|x+ \frac{\delta}{2} - x| < \delta$ aber $|f(x_{0}) - f\left( x + \frac{\delta}{2} \right)| = |0-1| = 1 > \frac{1}{2} \F \delta > 0$
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

## A4
### a)
Sei $f: (a,b) \to \R$ mit $x < y \RA f(x) \leq f(y)$ und $\Lim_{x \to x_{0}+} f(x) = \Lim_{x \to x_{0}-} f(x)$

Z.z.:
$\epta |x - x_{0}| < \delta \RA |f(x) - f(x_{0})| < \varepsilon \F x \in (a,b)$

Offensichtlich gilt $x_{0} \in \R$, denn sonst wäre entweder $\Lim_{x \to x_{0}-} f(x)$ nicht definiert ($x_{0} = -\infty$) oder $\Lim_{x \to x_{0}+}f (x)$ nicht definiert ($x_{0} = \infty$)

Außerdem folgt durch die monotonie, dass gelten muss
$\Lim_{x \to x_{0}+} f(x)= \Lim_{x \to x_{0}-} f(x) = L \in \R$:

Angenommen $L = \infty$:
Dann müsste nach der Monotonie für alle $x_{1}: x_{1} > x_{0}, x_{1} \in (a,b)$ gelten:
$f(x_{1}) \geq \Lim_{x \to x_{0}+} f(x) = \infty$ 
(weil $\Lim_{x \to x_{0}+} = \infty$ impliziert:
$\F M > 0 \E \delta > 0: |x-x_{0}| < \delta \RA |f(x) - f(x_{0})| > M \F x : x_{0} < x < b$
und damit muss f für ein $x > x_{0}$ definiert sein.
Folglich kann $\Lim_{x \to x_{0}+} f(x)$ nicht $\infty$ sein.
Analog für $-\infty$

Folglich muss gelten $L \in \R$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

$\RA$ Es gilt:
$\Lim_{x \to x_{0}+} f(x)= L$
$\LRA \epta |x - x_{0}|< \delta \RA |f(x) - L| < \varepsilon \F x: x_{0}< x < b$
und
$\Lim_{x \to x_{0}-} f(x) = L$
$\LRA \epta |x - x_{0}|< \delta \RA |f(x)- L|< \varepsilon \F x : a < x < x_{0}$

$\RA \epta |x-x_{0}|<\delta \RA |f(x)-L|<\varepsilon \F x \in (a,b)$

und mit $L \in \R$ folgt $\Lim_{x \to x_{0}+} f(x)= f(x_{0}) = \Lim_{x \to x_{0}-} f(x)$

$\RA \F \varepsilon > 0 \E \delta >0 : |x - x_{0}| < \delta \RA |f(x) - f(x_{0})|<\varepsilon \F x \in (a,b)$
$\bs$

### b)
Betrachte $f: \R\without \{ 0 \} \to \R, x \onto \frac{1}{x^{2}}$

Offensichtlich ist $\Lim_{x\to 0+} f(x) = \Lim_{x \to 0-} f(x) = \infty$
aber weil $f(0)$ nicht definiert ist, ist f nicht stetig in 0
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

### c)
Sei $I \subseteq \R$, $f: I \to \R$ stetig und $x < y \RA f(x) < f(y) \F x, y \in I$
Sei $\inv f: f(I) \to \R$ die Inversfunktion zu f (existenz bereits bewiesen in Satz 8.13)
Z.z: $\F x, y \in I': x < y \RA \inv f(x) < \inv f(y)$

Offensichtlich gilt: 
$(x < y \RA f(x) < f(y)) \RA (f(x) < f(y) \RA x  < y)$
denn:
Angenommen:
$f(x) < f(y)$ aber $x > y$
dann folgt $f(x) > f(y) \RA f(x) > f(x) \contrana$

Also gilt für größenrelionen von werten und streng monotonen Funktionen allgemein 
$x < y \LRA f(x) < f(y)$

Damit folgt aber:
Angenommen es gilt für $x, y \in f(I), x < y \LRA \inv f(x) \geq \inv f(y)$
$\RA f(x) < f(y) \LRA f(\inv f(x)) \geq f(\inv f (y))$
$\RA f(x) < f(y) \LRA x \geq y \contrana$

Folglich muss $\inv f$ streng monoton wachsend sein
$\bs$

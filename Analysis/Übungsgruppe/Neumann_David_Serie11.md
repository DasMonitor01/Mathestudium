# Aufgabe 1
Z.z:
$\Lim_{x \to 0, x\neq 0} \frac{1 - \cos (x)}{x^{2}} = \frac{1}{2}$

### Beweis:
$\d\frac{1-\cos(x)}{x^{2}}$
// Darstellung als Reihe
$\d = \frac{1-\Sum_{k = 0}^{\infty}(-1)^{k} \frac{x^{2k}}{(2k)!}}{x^{2}}$
// Aufspalten des Bruchs, kleine Anpassungen in der Reihe
$\d =\frac{1}{x^{2}} + \Sum_{k=0}^{\infty}(-1)^{k+1} \frac{x^{2k-2}}{(2k)!}$
// Herausziehen des ersten Terms der Reihe
$\d = \frac{1}{x^{2}} + (-1)^{0+1} \cdot \frac{x^{2 \cdot 0 - 2}}{(2 \cdot 0)!} + \Sum_{k=1}^{\infty}(-1)^{k+1} \cdot \frac{x^{2k-2}}{(2k)!}$
// Vereinfachung
$\d = \frac{1}{x^{2}}- \frac{1}{x^{2}} + \Sum_{k=1}^{\infty}(-1)^{k+1} \cdot \frac{x^{2k-2}}{(2k)!}$
// Kürzen der Terme, herausziehen des ersten Terms der Reihe
$\d = (-1)^{1+1} \cdot \frac{x^{0}}{(2\cdot 1)!} + \Sum_{k=2}^{\infty} (-1)^{k+1}\cdot \frac{x^{2k-2}}{(2k)!}$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

// Vereinfachung, substitution mit k = i+1
// Anm: $a^{0}$ wurde als 0 definiert, auch wenn $a = 0$ gilt.
$\d = \frac{1}{2} + \Sum_{i=1}^{\infty}(-1)^{i+2} \cdot \frac{x^{2(i+1)-2}}{(2i+2)!}$ 
$\d= \frac{1}{2} + \Sum_{i = 1}^{\infty}(-1)^{i+2} \cdot \frac{x^{2i}}{(2i+2)!}$
$\RA$
$\d\Lim_{x \to 0, x\neq 0} \frac{1-\cos(x)}{x^{2}}$
$\d= \Lim_{x \to 0, x \neq 0}(\frac{1}{2} + \Sum_{i = 1}^{\infty} (-1)^{i+2} \cdot \frac{x^{2i}}{(2i+2)!})$
$\d= \frac{1}{2} + \Sum_{i=1}^{\infty}(-1)^{i+2} \cdot \frac{0^{2i}}{(2i+2)!}$
// Anm. da $i \geq 1$ gilt, gilt $0^{2i} \neq 0^{0} \F i$ und somit $0^{2i} = 0$
$\d = \frac{1}{2} + \Sum_{i=1}^{\infty} 0$
$\d = \frac{1}{2}$
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

# Aufgabe 2
## a)
Z.z:
$\Sum_{k=2}^{\infty} \frac{1}{k \log(k)^{\alpha}}$ konvergent für $\alpha > 1$, divergent für $\alpha \leq 1$

### Beweis
// Blatt 8.3.a)
$\Sum_{k=2}^{\infty} \frac{1}{k \log(k)^{\alpha}}$ konvergent
$\LRA \Sum_{k=1}^{\infty} 3^{k} \frac{1}{3^{k} (\log(3^{k}))^{\alpha}}$ konvergent

$= \Sum_{k=1}^{\infty} \frac{1}{(\log(3^{k}))^{\alpha}}$

$= \Sum_{k=1}^{\infty} \frac{1}{(k \log(3))^{\alpha}}$
$= \Sum_{k = 1}^{\infty} \frac{1}{k^{\alpha} \log(3)^{\alpha}}$

$\d= \frac{1}{\log(3)^{\alpha}} \Sum_{k=1}^{\infty} \frac{1}{k^{\alpha}}$

//Blatt 8.3.b)
$\RA$ konvergent, genau dann, wenn $\alpha > 1$
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

## b)
Z.z:
$\log(1+x) \leq x \F x \geq 0$

### Beweis:
Sei $x \geq 0$
Es gilt 
$\exp(x) = 1+ x + \Sum_{k=2}^{\infty} \frac{x^{k}}{k!}$
und für $x \geq 0$ gilt $x^{k} \geq 0$
$\RA \Sum_{k=2}^{\infty} \frac{x^{k}}{k!} \geq 0$
$\RA 0 \geq - \Sum_{k=2}^{\infty} \frac{x^{k}}{k!}$
$\RA \exp(x) \geq 1 + x + \Sum_{k=2}^{\infty} \frac{x^{k}}{k!} - \Sum_{k=2}^{\infty} \frac{x^{k}}{k!}$
$\RA \exp(x) \geq 1 + x$
// wir können die Inversfunktion anwenden, und die Relation bleibt bestehen.
$\RA x \geq \log(1 + x)$
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

# Aufgabe 3
## a)
Z.z: 
$(1)$$\d\F |\alpha| \leq \pi : \cos\left( \frac{\alpha}{2} \right) = \sqrt{ \frac{1+\cos(\alpha)}{2}}$

$(2)$$\d\F |\alpha| \leq \frac{\pi}{2}: \sin\left( \frac{\alpha}{2} \right) = \frac{\sin(\alpha)}{2} \cdot \sqrt{\frac{2}{1+ \sqrt{1-\sin(\alpha)^{2}}}}$

### Beweis:
$(1)$
Sei $|\alpha| \leq \pi$

$\d\cos(\alpha) = \cos\left( \frac{\alpha}{2} + \frac{\alpha}{2} \right)$

// S.9.8
$\d\LRA \cos(\alpha) = \cos\left( \frac{\alpha}{2} \right)^{2} - \sin\left( \frac{\alpha}{2} \right)^{2}$ 

// $\sin(x)^{2} + \cos(x)^{2} = 1 \LRA -\sin(x)^{2} = \cos(x)^{2} - 1$ (S.9.6)

$\d\LRA \cos(\alpha) = \cos\left( \frac{\alpha}{2} \right)^{2} + \cos\left( \frac{\alpha}{2} \right)^{2} - 1$

// Umformen
$\d\LRA \cos\left( \frac{\alpha}{2} \right)^{2} = \frac{\cos(\alpha) + 1}{2}$

// anm: $\cos\left( \frac{\alpha}{2} \right) \geq 0 \F x \in [-\pi, \pi]$, deswegen gibt es hier keine Probleme mit den Vorzeichen
// da $\cos(\alpha) \leq 1$, können wir die Wurzel ziehen.
$\d\LRA \cos\left( \frac{\alpha}{2} \right) = \sqrt{\frac{\cos(\alpha)+1}{2}}$
$\checkmark$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

$(2)$
Sei $|\alpha| \leq \frac{\pi}{2}$

$\d\sin(\alpha) = \sin\left( \frac{\alpha}{2} + \frac{\alpha}{2} \right)$

// S.9.8
$\LRA\d \sin(\alpha) = 2 \sin\left( \frac{\alpha}{2} \right)\cos\left( \frac{\alpha}{2} \right)$

// Umformen, $\cos\left( \frac{\alpha}{2} \right)> 0 \F |\alpha| \leq \frac{\pi}{2}$

$\LRA\d\frac{\sin(\alpha)}{2} = \frac{\sin(\alpha)}{2} \cdot \frac{1}{\cos\left( \frac{\alpha}{2} \right)}$

// $|\alpha| \leq \frac{\pi}{2} \RA$ (1) auf $\cos\left( \frac{\alpha}{2} \right)$ anwenden.

$\d\LRA \sin\left( \frac{\alpha}{2} \right) = \frac{\sin(\alpha)}{2} \cdot \frac{1}{\sqrt{\frac{\cos(\alpha)+1}{2}}}$
// Umformen
$\d\LRA \sin\left( \frac{\alpha}{2} \right) = \frac{\sin(\alpha)}{2} \cdot \sqrt{\frac{1}{\frac{\cos(\alpha)+1}{2}}}$

$\d\LRA \sin\left( \frac{\alpha}{2} \right) = \frac{\sin(\alpha)}{2} \cdot \sqrt{\frac{2}{1+\cos(\alpha)}}$

// S.9.6: $\sin(x)^{2} + \cos(x)^{2} = 1 \LRA \cos(x) = \sqrt{1-\sin(x)^{2}}$

$\d\LRA \sin\left( \frac{\alpha}{2} \right) = \frac{\sin(\alpha)}{2} \cdot \sqrt{\frac{2}{1+\sqrt{1- \sin (\alpha)^{2}}}}$
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

## b)
#### a) $\cos\left( \frac{\pi}{3} \right) = \frac{1}{2}$: 

$\d \sin\left( \frac{\pi}{3} \right)$

$\d= \sin\left( \pi - \frac{2\pi}{3} \right)$

// S.9.8
$\d = \sin(\pi)\cos\left( -\frac{2\pi}{3} \right) + \sin\left( -\frac{2\pi}{3} \right)\cos(\pi)$

// $\sin(\pi) =0$, $\cos(\pi) = -1$

$\d = -\sin\left( -\frac{2\pi}{3} \right)$

// S.9.14 $\sin(x) = -\sin(-x)$

$\d= \sin\left( \frac{2\pi}{3} \right)$

// S.9.8 $\sin(2x) = 2 \sin(x) \cos(x)$

$\d= 2\sin\left( \frac{\pi}{3} \right)\cos\left( \frac{\pi}{3} \right)$

$\d\RA \sin\left( \frac{\pi}{3} \right) = 2 \sin\left( \frac{\pi}{3} \right)\cos\left( \frac{\pi}{3} \right)$

//$\sin\left( \frac{\pi}{3} \right) \neq 0$

$\d\LRA \frac{1}{2} = \cos\left( \frac{\pi}{3} \right)$
$\checkmark$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


#### b) $\d\cos\left( \frac{\pi}{4} \right) = \frac{1}{2}\sqrt{2}$:

// A3.a)
$\d\cos\left( \frac{\pi}{4} \right) = \sqrt{\frac{1+\cos\left( \frac{\pi}{2} \right)}{2}}$

// $\cos\left( \frac{\pi}{2} \right) = 0$

$\d= \sqrt{\frac{1}{2}} = \frac{1}{\sqrt 2} = \frac{\sqrt{2}}{2} = \frac{1}{2}\sqrt{2}$
$\checkmark$


#### c) $\d\cos\left( \frac{\pi}{6} \right) = \frac{1}{2}\sqrt{3}$:

// A3.a)
$\d\cos\left( \frac{\pi}{6} \right) = \sqrt{\frac{1+\cos\left( \frac{\pi}{3} \right)}{2}}$

// $\cos\left( \frac{\pi}{3} \right) = \frac{1}{2}$

$\d= \sqrt{\frac{1+ \frac{1}{2}}{2}}$

$\d=\sqrt{\frac{\frac{3}{2}}{2}}$

$=\d\sqrt{\frac{3}{4}}$

$=\d\frac{\sqrt{3}}{2}$

$\d= \frac{1}{2} \sqrt{3}$
$\checkmark$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

#### d) $\d\sin\left( \frac{\pi}{3} \right) = \frac{1}{2}\sqrt{3}$:

$\d \sin\left( \frac{\pi}{3} \right)$

// S.9.14 $\sin(x)= \cos\left( x -\frac{\pi}{2} \right)$

$\d= \cos\left( \frac{\pi}{3} - \frac{\pi}{2} \right)$

$= \d \cos\left( \frac{2\pi}{6} - \frac{3\pi}{6} \right)$

$\d = \cos\left( -\frac{\pi}{6} \right)$

// S.9.14 $\cos(x) = \cos(-x)$

$\d= \cos\left( \frac{\pi}{6} \right)$
//siehe c)

$\d= \frac{1}{2}\sqrt{3}$
$\checkmark$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

#### e) $\d\sin\left( \frac{\pi}{4} \right) = \frac{1}{2}\sqrt{2}$:

$\d\sin\left( \frac{\pi}{4} \right)$

// S.9.14 $\sin(x) = \cos\left( x - \frac{\pi}{2} \right)$

$\d= \cos\left( \frac{\pi}{4} - \frac{\pi}{2}\right)$

$\d= \cos\left( \frac{\pi}{4} -\frac{2\pi}{4}\right)$

$= \d \cos\left( -\frac{\pi}{4} \right)$

// S.9.14 $\cos(x) = \cos(-x)$

$= \d \cos\left( \frac{\pi}{4} \right)$
// siehe b)
$\d= \frac{1}{2}\sqrt{2}$
$\checkmark$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

#### f) $\d\sin\left( \frac{\pi}{6} \right) = \frac{1}{2}$

$\d \sin\left( \frac{\pi}{6} \right)$

// S.9.14 $\sin(x)= \cos\left( x - \frac{\pi}{2} \right)$

$=\d \cos\left( \frac{\pi}{6} - \frac{\pi}{2} \right)$

$\d = \cos\left( \frac{\pi}{6} - \frac{3\pi}{6} \right)$

$=\d \cos\left(  - \frac{2\pi}{6} \right)$

$=\d \cos\left( -\frac{\pi}{3} \right)$

// S.9.14 $\cos(x ) = \cos(-x)$
$\d = \cos\left( \frac{\pi}{3} \right)$
// siehe a)
$= \d \frac{1}{2}$
$\checkmark$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

#### g)

Merke: $e^{i \varphi} = \cos(\varphi)+ i \sin(\varphi)$
$\RA$
$\d e^{i \frac{\pi}{3}}$
$\d= \cos\left( \frac{\pi}{3} \right) + i \sin\left( \frac{\pi}{3} \right)$

//siehe a) und d)

$\d = \frac{1}{2} + i\frac{1}{2}\sqrt{3}$

$\d= \frac{1}{2}(1+ i\sqrt 3)$
$\checkmark$

$e^{i \frac{\pi}{4}}$
$=\d \cos\left( \frac{\pi}{4} \right) + i \sin\left( \frac{\pi}{4} \right)$

// siehe b) und e)

$\d= \frac{1}{2}\sqrt{2} + i \frac{1}{2}\sqrt{2}$

$\d = \frac{1}{2}\sqrt{2}(1+i)$
$\checkmark$

$e^{i \frac{\pi}{6}}$
$\d = \cos\left( \frac{\pi}{6} \right) + i \sin\left( \frac{\pi}{6} \right)$

// siehe c) und f)

$= \d \frac{1}{2}\sqrt{3} + i \frac{1}{2}$

$\d = \frac{1}{2}(\sqrt{3}+i)$
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

# Aufgabe 4
# a)
Sei $f: \R \to \R$ stetig, $\E t > 0: f(x +t) = f(x)$

Z.z:
f ist gleichmäßig stetig

### Beweis
Merke:

(1) $\F y \in f(\R) \E x_{0} \in [0,t]: f(x) = y$
Denn sei $y \in f(\R)$
$\RA \E x_{0} \in \R: f(x_{0}) = y$
$\RA f(x_{0} - t) = f(x_{0} - t + t) = f(x_{0})$
$\RA f(x_{0} - kt) = f(x_{0}), k \in \Z$
$\RA f(x_{0} \mod t) = f(x_{0})$
$\RA x_{0} \mod t \in [0,t]$


Z.z: $\F \varepsilon > 0 \E \delta > 0: |x - y|< \delta \RA |f(x)-f(y)| < \varepsilon \F x,y \in \R$

Seien $x,y \in \R$. 
// nach (1)
$\RA$ Es seien $x_{0} = x \mod t, y_{0} = y \mod t \in [0,t]$

$\RA$ $|x-y| < \delta \LRA |x_{0} - y_{0}|< \delta$
$\RA f(x_{0}) = f(x), f(y_{0}) = f(y)$
$\RA |f(x) - f(y)|< \varepsilon \LRA |f(x_{0}) - f(y_{0})|<\varepsilon$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

Sei $f*: [0,t] \to \R: f*(x) = f(x) \F x \in [0,t]$

// S.8.12
$f*$ ist gleichmäßig stetig.
$\RA \F \varepsilon* >0 \E \delta* >0: |x-y|< \delta* \RA |f(x)-f(y)|<\varepsilon* \F x,y \in [0,t]$

$\RA$ wähle $\delta = \delta*$. 
$\RA |x-y| <\delta \RA |f(x) - f(y)|< \varepsilon$
$\bs$

## b)
Sei $g: \R \to \R, x \onto f(x^{2})$
Z.z:
g gleichmäßig stetig $\LRA f(x) = c, c \in \R$

### Beweis
"$\RA$"
Sei $f(x) = c$
$\RA g(x) = f(x^{2}) = c = f(x) \F x \in \R$
$\RA$ g ist Lipschitzstetig, mit L=0;
$\RA$ g ist gleichmäßig stetig

"$\LA$"
Sei g gleichmäßig stetig
$\RA \epta |x-y|<\delta \RA |g(x)-g(y)|<\varepsilon \F x, y \in \R$
$\RA |x-y| <\delta \RA |f(x^{2})-f(y^{2})|<\varepsilon$
...
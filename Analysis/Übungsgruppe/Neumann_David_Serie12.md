

# Aufgabe 2
Seien $f,g: (-1,1)  \to \R$ stetig mit $f(x) \cdot g(x) = x \F x \in (-1,1)$

## a)
Seien f und g differenzierbar
Z.z:
$f(0) = 0 \RA g(0) \neq 0$
f,g diffbar $\RA f(x) \cdot g(x)$ ist differenzierbar mit $(f(x)\cdot g(x))' = f'(x)g(x)+ g'(x)f(x)$
Aber sei $h(x):= x = f(x) \cdot g(x)$
Es gilt $h'(x) = 1 = (f(x)\cdot g(x))'$
$\RA f'(x)g(x)+g'(x)f(x) = 1 \F x \in (-1,1)$
Sei nun $f(0) = 0$
$\RA (f(0)\cdot g(0))' = f'(0)g(0) + g'(0)f(0) = f'(0)g(0)+ g'(0)\cdot 0$
$= f'(0)g(0)$
$\RA 1 = f'(0)g(0)$

Angenommen $g(0) = 0$
$\RA f'(0)g(0)=f'(0)\cdot 0 = 0 \neq 1$
$\contrana$
$\RA g(0) \neq 0$
$\bs$

#### b)
Betrachte $f: (-1, 1) \to \R, x \onto \biggl \{ \begin{matrix} \sqrt{x}: x \geq 0 \\ - \sqrt{-x}: x < 0 \end{matrix}$
und $g: (-1,1) \to \R, x \onto \biggl \{ \begin{matrix} \sqrt{x}: x \geq 0 \\ \sqrt{-x}: x < 0\end{matrix}$

Offensichtlich gilt:
$f(x) \cdot g(x) = x \F x \in (-1,1)$, denn:
- ist $x \geq 0$, so ist $f(x) = \sqrt{x}$ und $g(x) = \sqrt{x}$
$\RA f(x) \cdot g(x) = \sqrt{x} \cdot \sqrt{x} = x$
- ist $x < 0$ so ist $f(x) = -\sqrt{-x}$ und $g(x) = \sqrt{-x}$, wobei $-x > 0$ gilt und somit $\sqrt{-x}$ existiert.
$\RA f(x) \cdot g(x) = - \sqrt{-x} \cdot \sqrt{-x}$
$= -(-x) = x$

Außerdem ist $f(0) = g(0) = \sqrt{0} = 0$

Zuletzt sind f und g stetig:
Z.z:
$\F x_{0} \in (-1,1) \F \varepsilon >0 \E \delta >0: |x-x_{0}|<\delta \RA |f(x)-f(x_{0})|<\varepsilon \F x \in (-1,1)$,
$\F x_{0} \in (-1,1) \F \varepsilon >0 \E \delta > 0 : |x-x_{0}| < \delta \RA |g(x)-g(x_{0})| < \varepsilon \F x \in (-1,1)$
Sei $\varepsilon > 0$:

Fallunterscheidung:

Fall 1:
$x_{0} > 0$:
Für $\delta < x_{0}$ folgt direkt $|x-x_{0}| < \delta \RA x \geq 0$
denn angenommen:
$|x-x_{0}| < \delta : 0 < \delta < x_{0}$
und $x < 0$
$\RA |x- x_{0}| = |x_{0}-x| < x_{0}$
Sei $x* = -x \RA x* >0$
$\RA |x_{0} - x| = |x_{0} + x*|$
$x_{0} > 0, x* > 0\RA x_{0} + x* > 0$
$\RA |x_{0} + x*| = |x_{0} - x| = x_{0} - x$
$\RA x_{0} - x < x_{0}$
$\RA -x < 0$
$\RA x > 0 \contrana x < 0$

$\delta < x_{0} \RA |f(x) - f(x_{0})| = |\sqrt{x} - \sqrt{x_{0}}|$

$\RA \F \varepsilon > 0 \E \delta > 0: |x-x_{0}| < \delta \RA |f(x)-f(x_{0})| < \varepsilon$, da wir wissen, dass $f*: [0,\infty) \to \R, x \onto\sqrt{x}$ stetig ist, und somit $\delta*$ existiert. Somit folgt mit $\delta = \min\left\{  \frac{x_{0}}{2}, \delta* \right\}$, dass $|f(x)-f(x_{0})| <\varepsilon$ gilt.
(Analoges auch für g für x > 0, da g(x) = f(x) für x > 0)

Fall 2:
$x_{0} < 0$

f:
Es gilt $f(x) = - f(-x) \F x <0$:
$f(x) = -\sqrt{-x}$
Für $x* := -x \RA x* >0$
existiert $\sqrt{x*}$
$\RA f(x) = -\sqrt{x*}$, $f(-x) = f(x*) = \sqrt{x*}$
$\RA f(x) = - f(-x)$
$\checkmark$

$\RA f(x)$ ist stetig für $x < 0$, da $f(x) = -f(-x) \F x < 0$ ist, und f stetig für alle $x >0$ ist
$\checkmark$

g:
Es gilt $g(x) = g(-x)\F x <0$:
$g(x) = \sqrt{-x}$
Für $x* := -x \RA x* > 0$
existiert $\sqrt{x*}$
$\RA g(x) = \sqrt{-x} = \sqrt{x*} = g(x*)$
$\checkmark$

$\RA g(x)$ ist stetig für $x < 0$, da $g(x) = g(-x) \F x < 0$ ist, und g stetig für alle x > 0 ist.
$\checkmark$

Fall 3:
$x_{0} = 0$:
$\RA f(x_{0}) = \sqrt{0} = 0$
$\RA$ Z.z: $\F \varepsilon > 0 \E \delta >0: |x|<\delta \RA |f(x)|<\varepsilon \F x \in (-1,1)$

Wähle $\d\delta = \frac{\varepsilon^{2}}{4}$

Fallunterscheidung:
Fall 3.1:
$x \geq 0$:
$\RA |x| < \delta \RA 0 < x < \delta$
$\d\RA |f(x)| = |\sqrt{x}| =\sqrt{x} < \sqrt{\delta} = \sqrt{\frac{\varepsilon^{2}}{4}} = \frac{\varepsilon}{2} < \varepsilon$
(Analog für g(x))
$\checkmark$

Fall 3.2:
$x < 0$:

$\RA |x| < \delta \RA 0 < -x < \delta$
f:
$\d\RA |f(x)| = |-\sqrt{-x}| = \sqrt{-x} < \sqrt{\delta} = \frac{\varepsilon}{2} < \varepsilon$
g:
$\RA |g(x)| = |\sqrt{-x}|=\sqrt{-x} < \sqrt{\delta} < \varepsilon$
$\bs$

# Aufgabe 3
Sei $x > 0$
## a)
Sei $\d f: (0,\infty), f(x) = \log\left( \frac{x^{3}}{(1+x^{2})^{5}} \right)$

Sei $g(x) := \log(x)$ und $\d h(x) := \frac{x^{3}}{(1+x^{2})^{5}}$

dann ist $f(x) = g(h(x))$, und weil g(x), h(x) diffbar für $x > 0$ (h(x) diffbar wird unten gezeigt) ist auch $g(h(x)) = f(x)$ diffbar 
und $(g(h(x)))' = f'(x) = g'(h(x)) \cdot h'(x)$

$g'(x) = \frac{1}{x}$

Sei $j(x) : = x^{3}$ und $k(x) := (1+x^{2})^{5}$
dann ist $\d h(x) = \frac{j(x)}{k(x)}$
und weil $k(x) > 0 \F x \geq 0, k(x)$, j(x) diffbar auf $(0,\infty)$ ist auch $\d \frac{j(x)}{k(x)}$ diffbar und $\d \left( \frac{j(x)}{k(x)} \right)' = h'(x) = \frac{j'(x)\cdot k(x) - j(x)\cdot k'(x)}{(k(x))^{2}}$

$j'(x) = 3x^{2}$

Sei $l(x) := x^{5}$ und $m(x) := 1+x^{2}$
dann ist $k(x) = l(m(x))$, und weil l(x), m(x) diffbar für $x \in (0,\infty)$ ist auch $l(m(x)) = k(x)$ diffbar und $(l(m(x)))' = k'(x) = l'(m(x)) \cdot m'(x)$

$l'(x) = 5x^{4}$, $m'(x) = 2x$
$\RA k'(x) = 5(1+x^{2})^{4} \cdot 2x$
$= 10x \cdot (1+x^{2})^{4}$

$\d \RA h'(x) = \frac{3x^{2}\cdot (1+x^{2})^{5} - x^{3} \cdot 10 x \cdot (1+x^{2})^{4}}{((1+x^{2})^{5})^{2}}$

$\d= \frac{3x^{2}(1+x^{2})^{5}- 10 x^{4} \cdot (1+x^{2})^{4}}{(1+x^{2})^{10}}$

$\d= \frac{3x^{2}\cdot (1+x^{2}) - 10x^{4}}{(1+x^{2})^{6}}$

$\d = \frac{3x^{2} + 3x^{4} - 10 x^{4}}{(1+x^{2})^{6}}$

$\d = \frac{-7x^{4} + 3x^{2}}{(1+x^{2})^{6}}$

$\d\RA (g(h(x)))' = f'(x) = \frac{1}{\left( \frac{x^{3}}{(1+x^{2})^{5}} \right)} \cdot \frac{-7x^{4}+3x^{2}}{(1+x^{2})^{6}}$

$\d = \frac{(1+x^{2})^{5}}{x^{3}} \cdot \frac{-7x^{4} + 3x^{2}}{(1+x^{2})^{6}}$

$\d = \frac{-7x^{4}+3x^{2}}{x^{3} \cdot (1+x^{2})^{6}}$
$\checkmark$

## b)

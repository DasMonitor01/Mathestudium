$f'_{b}(x) = -(x^{2}-1)^{-2} \cdot 2x + \frac{2}{b^{2}} \cdot x$
$f'_{b}(x) = 0$
$0 = -(x^{2}-1)^{-2} \cdot 2x + \frac{2}{b^{2}} \cdot x$
$\stackrel{x^{-n} := \frac{1}{x^{n}}}\Leftrightarrow 0 = - \frac{1}{(x^{2}-1)^{2}} \cdot 2x + 2 \cdot \frac{1}{b^{2}} \cdot x$
// da $(x^{2} - 1)^{2}$ sicher ungleich null ist (sonst wäre die funktion nicht definiert (geteilt durch 0)) können wir damit multiplizieren
$\stackrel{\cdot(x^{2}-1)^{2}}\Leftrightarrow 0 = -2x + 2 \cdot \frac{1}{b^{2}} \cdot x \cdot (x^{2}-1)^{2}$
$\stackrel{:2}\Leftrightarrow 0 = -x + \frac{1}{b^{2}} \cdot x \cdot (x^{2}-1)^{2}$
// $b^{2}$ ungleich null da siehe oben
$\stackrel{\cdot b^{2}} \Leftrightarrow 0 = -x \cdot b^{2} + x \cdot (x^{2}-1)^{2}$
$\stackrel{+ x \cdot b^{2}}\Leftrightarrow x \cdot b^{2} = x \cdot (x^{2}- 1)^{2}$
$\blacksquare$

Bonus:
$0 = x^{5} - 2x^{3} + x \cdot (1 - b^{2})$
$0 = x \cdot (x^{4} - 2 x^{2} + (1-b)\cdot (1+b))$
$\RA x_{1}= 0$
$0 = x^{4} - 2x^{2} + (1-b^{2})$
sei $z:= x^{2}$
$0 = z^{2} - 2 z + (1-b^{2})$
$z_{1,2} = 1 \plusminus \sqrt{1 - 1 +b^{2}}$
$= 1 \plusminus b$
$x_{1,2} = \plusminus \sqrt{1+b} \in \R \F b \geq -1$
$x_{3,4} = \plusminus \sqrt{1-b} \in \R\F b \leq 1$

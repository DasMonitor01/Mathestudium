## Lemma 2.a.1:
Anmerkung:
Im folgenden Sei $M := \{ b, b+1,\dots \}: b \in \Z$, dass heißt die Startglieder der Folge können auch im Negativen liegen.

Sei $(a_{n})_{n \in M}$ eine Folge mit $\limin a_{n} = 0$.
Dann konvergiert die Reihe $\Sum_{n=b}^{\infty}a_{n}^{2}$ für jedes $b \in M$.
### Beweis:
Merke: 
Es reicht zu zeigen, dass $\Sum_{n=b}^{\infty}a_{n}^{2}$ für ein $b \in M$ konvergiert, denn nach Satz $Ü.8.0$ gilt:
$\Sum_{n=b}^{\infty}a_{n}^{2}$ konvergent $\RA$ $\Sum_{n=c}^{\infty}a_{n}^{2}, c \in M$ konvergiert, weil gilt:
- Entweder $c = b$, trivial da die Reihe gleich ist.
- oder $c <b$, konvergent nach Ü.8.0.a)
- oder $c>b$, konvergent nach Ü.8.0.b)

Wir müssen also nur zeigen, für ein $b \in M$ gilt:
$\Sum_{n=b}^{\infty}a_{n}^{2}$ konvergiert.

Es gilt:
$\limin a_{n} = 0 \LRA \forall \varepsilon > 0 \E N\in M: |a_{n}-0|=|a_{n}|<\varepsilon \F n \geq N$ 
$\RA \exists N_{1} \in M: |a_{n}|< \frac{1}{2} \F n \geq N_{1}$

Betrachte:
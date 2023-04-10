# Satz 9.13
Jedes $z \in \C$ lässt sich schreiben als $z = r \cdot e^{i \varphi}$, wobei $r = |z| \in [0, \infty)$ und $\varphi \in \R$.
Für $z \neq 0$ ist $\varphi$ bis auf vielfache von $\tau$ eindeutig.

### Bew:
1) z = 0: $z = 0 \cdot e^{i\varphi} = 0 \F \varphi \in \R$
2) $z \neq 0$:
Sei $r = |z|$.
Dann ist $z = r \xi$ mit $\xi = \frac{z}{r}$
Sei $\mu = Re(\xi), \gamma = Im(\xi)$
$\alpha = \arccos(\mu)$ ($\in [0, \pi]$)
$\RA \cos \alpha = \gamma$
$\RA \sin \alpha = \plusminus \mu$

Wähle $\varphi = \alpha$ falls $\sin \alpha = \nu$
Wähle $\varphi = - \alpha$ falls $\sin \alpha = - \mu$

Dann $e^{ i \varphi} = \cos(\alpha) + i \cdot \sin(\alpha)$, falls $\sin(\alpha) = \mu$
$e^{i\varphi}= \cos(-\alpha) + i \sin(\alpha)$, falls $\sin(\alpha) = - \mu$
$= \mu + i \nu = \xi$

$z = r \xi = r \cdot e ^{i \varphi}$

3) Eindeutigkeit
Seien $\varphi$ und $\psi \in \R$ mit $e^{i \varphi} = e ^{i \psi} = \zeta$
...

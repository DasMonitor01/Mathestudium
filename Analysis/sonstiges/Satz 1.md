# Satz 1:
Sei $(a_{n})_{n \in \Z}$ eine Folge und $b,c,d \in \Z: b<c < d$. 
und $\Sum_{n=c}^{\infty} a_{n}$ konvergent.
Dann konvergieren auch
a) $\Sum_{n=b}^{\infty}a_{n}$ 
und 
b) $\Sum_{n=d}^{\infty} a_{n}$
und es gilt:
c) $\Sum_{n=b}^{\infty} a_{n} = \Sum_{n=c}^{\infty}a_{n} + \Sum_{n=b}^{c-1}a_{n}$
und
d) $\Sum_{n=d}^{\infty}a_{n} = \Sum_{n=c}^{\infty}a_{n} - \Sum_{n=c}^{d-1}a_{n}$

### Beweis:
Sei $S_{m} := \Sum_{n=c}^{m} a_{n}$.
Es gilt: $\Sum_{n=c}^{\infty} a_{n} = \Limin m S_{m}$

Betrachte: $S_{m} + \Sum_{n=b}^{c-1}a_{n}$
Es gilt: $\Limin m S_{m}$ existiert und $\Limin m \Sum_{n=b}^{c-1}a_{n} = \Sum_{n=b}^{c-1}a_{n}$
$\RA \Limin m S_{m} + \Limin m \Sum_{n=b}^{c-1}a_{n} = \Limin m (S_{m} + \Sum_{n=b}^{c-1}a_{n})$ 
$= \Limin m (\Sum_{n=c}^{m} a_{n} + \Sum_{n=b}^{m}a_{n}) = \Limin m \Sum_{n=b}^{m}a_{n} = \Sum_{n=b}^{\infty} a_{n}$ $\checkmark$

Betrachte: $S_{m} - \Sum_{n=c}^{d-1}a_{n}$

Es gilt: $\Limin m S_{m}$ existiert und $\Limin m \Sum_{n=c}^{d-1}a_{n} = \Sum_{n=c}^{d-1}a_{n}$
$\RA \Limin m S_{m} - \Limin m \Sum_{n=c}^{d-1} a_{n} = \Limin m (S_{m} - \Sum_{n=c}^{d-1} a_{n})$
$= \Limin m (\Sum_{n = c}^{m} a_{n} - \Sum_{n=c}^{d-1}a_{n})$ 
$= \Limin m (\Sum_{n= d}^{m}a_{n} + \Sum_{n=c}^{d-1}a_{n} - \Sum_{n=c}^{d-1}a_{n})$
$= \Limin m \Sum_{n=d}^{m} a_{n}$
$= \Sum_{n=d}^{\infty}a_{n}$ 
$\bs$
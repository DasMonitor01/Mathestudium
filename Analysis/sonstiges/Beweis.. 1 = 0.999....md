Beginn: 
Sei $a_{n \in \N} := \biggl\{ \begin{matrix} \frac{9}{10} : n= 1 \\ a_{n-1} + \frac{9}{10^{n}} : n > 1\end{matrix}$
-> $a_{n} = 0.99999\dots$ , mit n Neunen

Betrachte $b_{n \in \N} := \frac{1}{10^{n}}$

Merke:
Es gilt $a_{n} + b_{n} = 1 \F n \in \N$:

$(I)$ Beweis durch Induktion:
$(I.a)$ Induktionsstart:
n = 1:
$a_{1} + b_{1} = \frac{9}{10} + \frac{1}{10^{1}} = \frac{9}{ 10} + \frac{1}{10} = 1$

(I.b) Induktionsschritt:
Wir wissen für ein $n \in \N$ gilt:
$a_{n} + b_{n} = 1$

dann folgt für n+1:
$a_{n+1} + b_{n+1}$
$= a_{n} + \frac{9}{10^{n+1}} + \frac{1}{10^{n+1}}$
$= a_{n} + \frac{10}{10^{n+1}}$
$= a_{n} + \frac{1}{10^{n}}$
$= a_{n} + b_{n} \stackrel{I.a}= 1$
$\checkmark$
$\RA a_{n} = 1 - b_{n} \F n \in \N$

Merke: 
$\limin a_{n}$ existiert, da:

$a_{n}$ monton:

Es gilt $0 \leq \frac{9}{10^{n}} \F n \in \N$
$\RA a_{n-1} \leq a_{n-1} + \frac{9}{10} = a_{n}$
$\RA a_{n-1} \leq a_{n}$

$a_{n}$ beschränkt:
Es gilt $b_{n} = \frac{1}{10^{n}} \geq 0 \F n \in \N$
$\RA 0 \geq -b_{n}$
$\RA 1 \geq 1 - b_{n}$
$\RA 1 \geq a_{n} \F n \in \N$

$\RA a_{n}$ monoton wachsend und beschränkt,
$\RA \limin a_{n}$ existiert

Sei $0.\bar{9} := \limin a_{n}$

Es gilt $\limin b_{n} = \limin \frac{1}{10^{n}} = 0$:

$\RA 0.\bar{9} = \limin a_{n} = \limin (1-b_{n}) = \limin 1 - \limin  b_{n} = 1 - 0 = 1$
$\bs$

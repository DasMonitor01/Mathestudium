## Aufgabe 1
a)
gegeben:
$(a_n), (b_n), (c_n): a_n \leq b_n \leq c_n \F n \geq N\in \N$ 
$\limin a_n = a = \limin c_n$

z.z.:
$\limin b_n = a$
$\Leftrightarrow \F \epsilon > 0 \E N \in \N: |b_n - a| < \epsilon \F n \geq N$

$|b_n - a| \stackrel{\triangle-ungl}\leq |b_n - c_n| + |c_n - a|$
$a_n \leq b_n \Rightarrow |b_n - c_n| \leq |a_n - c_n|$
$\Rightarrow |b_n -a| \leq |a_n - c_n| + |c_n - a|$ 

$(c_n) \to a \Rightarrow \E N \in \N: |c_n - a| < \frac{\epsilon}{4} \F n \geq N$

$(a_n) \to a \Rightarrow \E N \in \N: |a_n - a| < \frac{\epsilon}{4} \F n \geq N$

$\Rightarrow |c_n - a_n| \stackrel{\triangle}\leq |c_n - a| + |a - a_n| < \frac{\epsilon}{2}$ 

$\Rightarrow |b_n -a| \leq |b_n - c_n| + |c_n - a| < \frac{\epsilon}{2} + \frac{\epsilon}{4} < \epsilon$
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

b)
geg:
$(a_n)$ beschränkt, $(b_n) \to 0$
$\Rightarrow \exists M \geq 0 \in \R: |a_n| \leq M \F n \in \N$

zu zeigen:
$\Lim_{n \to \infi}a_n \cdot b_n = 0$
$\Leftrightarrow \forall \epsilon >0 \E N \in \N: |a_nb_n| < \epsilon \F n \geq N$

Sei $\epsilon> 0$
$\Rightarrow |a_nb_n| \leq |M \cdot b_n| < |(M+1) \cdot b_n| \F n \in \N$

$(b_n) \to 0 \Rightarrow \E N: b_n < \frac{\epsilon}{M+1} \F n \geq N$
$\Rightarrow \E N : |a_n \cdot b_n| < |(M+1) \cdot \frac{\epsilon}{M+1}| = \epsilon \F n \geq N$ 
$\Rightarrow \E N: |a_n \cdot b_n| < \epsilon \F n \geq N$
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


## Aufgabe 2
gegeben:
$a_0 = \frac{3}{4}$
$a_{n+1} := \sqrt{a_n + \frac{3}{4}}$

a)
Beschränkt durch 2:
z.z:
$2 \geq a_n \F n \in \N$

Angenommen $2 \leq \sqrt{a_n + \frac{3}{4}}$  für ein $n \in \N$
$\Rightarrow 4 \leq a_n + \frac{3}{4}$
$\Rightarrow  a_n > 3$.
Da $a_0 < 3$ folgt, dass für alle $n \in \N$ gelten muss:
$2 > a_n$
$\blacksquare$

Monoton wachsend:
z.z.:
$a_{n+1} \geq a_n \F n \in \N$
Angenommen:
$a_n > a_{n+1}$ für ein $n \in \N$ 

$\Rightarrow a_n > \sqrt{a_n + \frac{3}{4}}$
...
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

b)
Nach a) ist $a_n$ monoton wachsend, und nach oben beschränkt, folglich konvergiert $a_n$ nach Satz 3.9

Sei $\limin a_n = a$

Es gilt:
$\limin a_n = \limin a_{n+1}$ 

$\Rightarrow 0 = \limin a_n - \limin a_{n+1}$ 
$= \limin a_n - a_{n+1}$
$0= \limin a_n - \sqrt{a_n + \frac{3}{4}}$ 
$0 = a - \sqrt{a + \frac{3}{4}}$
$a = \sqrt{a+\frac{3}{4}}$  (Achtung, hier schleicht sich eine zusätzliche Lösung ein)
$a^2 = a + \frac{3}{4}$
$0 = a^2 - a - \frac{3}{4}$
$a_{1,2} = \frac{1}{2} \plusminus \sqrt{(\frac{-1}{2})^2 + \frac{3}{4}}$
$a_1 = \frac{3}{2}$
$a_2 = - \frac{1}{2}$
von den berechneten werten ist nur der erste Sinnig, der andere ist eine fremde Lösung, die sich beim Quadrieren eingeschlichen hat.
$\Rightarrow \limin a_n = \frac{3}{2}$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


## Aufgabe 3
Gegeben:
$a_n := \biggl(1+ \Frac{1}{n}\biggl)^n$ 

$b_n := \biggl(1+ \Frac{1}{n}\biggl)^{n+1}$ 


z.z.:
$a_n$ monoton wachsend
$\Leftrightarrow$ 
$a_m < a_{m+1} \F m \in \N$
$\Leftrightarrow a_{n-1} < a_n\F n \in \N: n \geq 2$ ($m = n-1$)
$\Leftrightarrow (1 + \frac{1}{n-1})^{n-1} < (1 + \frac{1}{n})^n \F n \geq 2$

Beweis:
Startpunkt:
Nach der Bernoulli-Ungleichung gilt:
$(1+ (\frac{-1}{n^2}))^n > 1+ (\frac{-1}{n^2} \cdot n) \F n \geq 1$ 
$\Leftrightarrow (1 - \frac{1}{n^2})^n > 1 - \frac{1}{n}$ 
$\Leftrightarrow (\frac{n^2 -1}{n^2})^n > \frac{n-1}{n}$ 
$\Leftrightarrow (\frac{(n+1)(n-1)}{n \cdot n})^n > \frac{n-1}{n}$ 
$\Leftrightarrow (\frac{n+1}{n} \frac{n-1}{n})^n > \frac{n-1}{n}$ 

$\Leftrightarrow \Biggl(\Frac{(\frac{n+1}{n})}{(\frac{n}{n-1})}\Biggl)^n > \Frac{1}{\frac{n}{n-1}}$ 

$\Leftrightarrow \Frac{(\frac{n+1}{n})^n}{(\frac{n}{n-1})^n} > (\frac{n}{n-1})^{-1}$ | $\cdot (\frac{n}{n-1})^n$   //$(\frac{n}{n-1})^n > 0$

$\Leftrightarrow (\frac{n+1}{n})^n > (\frac{n}{n-1})^{n-1}$ 
$\blacksquare$

z.z.:
$b_n$ monoton fallend:
$\Leftrightarrow a_m > a_{m+1} \F m \in \N$
$\Leftrightarrow a_{n-1} > a_n \F n \in \N: n\geq 2$ ($m = n-1$)
$\Leftrightarrow (1+\frac{1}{n-1})^n > (1 + \frac{1}{n})^{n+1} \F n \geq 2$

Beweis:
Startpunkt:
Es gilt:
$n^2 > n^2 -1 \F n \geq 2$
$\Rightarrow \frac{n}{n^2 -1} > \frac{n}{n^2} = \frac{1}{n} \F n \geq 2$ 

Nach der Bernoulli-Ungleichung gilt auch:
$(1+ \frac{1}{n^2-1})^n > 1 + \frac{n}{n^2 -1} \F n \geq 2$

$\Rightarrow (1 + \frac{1}{n^2 -1})^n > 1 + \frac{1}{n}$ 

$\Leftrightarrow (\frac{n^2 - 1 + 1}{n^2-1})^n > \frac{n+1}{n}$ 
$\Leftrightarrow (\frac{n \cdot n}{(n+1)(n-1)})^n > \frac{n+1}{n}$ 

$\Leftrightarrow \Biggl(\Frac{\frac{n}{n-1}}{\frac{n+1}{n}}\Biggl)^n > \frac{n+1}{n}$ 

$\Leftrightarrow \Frac{(\frac{n}{n-1})^n}{(\frac{n+1}{n})^n} > \frac{n+1}{n}$ | $\cdot (\frac{n+1}{n})^n$  //$(\frac{n+1}{n})^n > 0$

$\Leftrightarrow (\frac{n}{n-1})^n > (\frac{n+1}{n})^{n+1}$
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

z.z.:
$\Lim_{n \to \infi} a_n = \Lim_{n \to \infi} b_n$

Wir wissen, dass $a_n$ monoton Wachsend, und $b_n$ monoton Fallend ist.

Es gilt außerdem offensichtlich $a_n \leq b_n \F n \in \N$ 

Da demnach aber $a_n$ offensichtlich nach unten, und $b_n$ offensichtlich nach oben beschränkt sind (jeweils $n = 1$ nach Definition der Monotonie), folgt dass $a_n$ und $b_n$ beschränkt sind. 
Nach Satz 3.9 konvergieren $a_n$ und $b_n$ demnach
Folglich existieren $\limnin a_n$ und $\limnin b_n$ 
$\Rightarrow \limnin a_n$
$= \limnin\ (1 + \frac{1}{n})^n$
$= 1 \cdot \limnin (1 + \frac{1}{n})^n$
$= \limnin (1 + 0) \cdot \limnin (1 + \frac{1}{n})^n$ 
$= \limnin (1 + \frac{1}{n}) \cdot \limnin (1 + \frac{1}{n})^n$ 
$= \limnin (1 + \frac{1}{n}) \cdot (1 + \frac{1}{n})^n$
$= \limnin (1+\frac{1}{n})^{n+1}$
$= \limnin b_n$ 
$\blacksquare$ 
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


## Aufgabe 4:
gegeben:
$0 < q < 1: q \in \R, C >0, (a_n): |a_{n+1} - a_n| \leq C q^n \F n \in \N$ 

$\Rightarrow Cq^n  \geq |a_{n+1} - a_n| \geq ||a_{n+1}| - |a_n||$
$\Rightarrow Cq^{n+1} \geq |a_{n+2} - a_{n+1}| \geq ||a_{n+2}| - |a_{n+1}||$ 
$\Rightarrow Cq^{n+1} + Cq^n \geq ||a_{n+1}|- |a_n|| + ||a_{n+2}| - |a_{n+1}||$ 
$\geq |a_{n+2} - a_{n+1} + a_{n+1} - a_n| = |a_{n+2} - a_n|$ 

$\Rightarrow C\cdot \Sum_{k=1}^{n+1}q^k \geq |a_{n+2} - a_n|$ 

Allgemeiner lässt sich folgern:

$C \cdot \Sum_{k=1}^{n+m} q^k \geq |a_{n + m} - a_n|$ 
$\Leftrightarrow C \cdot \frac{1 - q^{n+m}}{1-q} \geq |a_{n+m} - a_n|$ 
...
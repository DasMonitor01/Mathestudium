A1)
a)
z.z.: $||x| - |y|| \leq |x - y|$

Wir wissen:
$|a+b| \leq |a|+|b|$
$\Rightarrow |a + b| - |b| \leq |a|$

Sei $b:= -y$ und $a:= x+y$
$\Rightarrow |x + y - y| - |-y| \leq |x + y|$
$\Rightarrow |x| - |y| \leq |x + y - y + y|$
$\Rightarrow |x| - |y| \leq |x + y| \leq |x - y| + 2 |y|$
...


b)
aus a): $||x| -|y|| \leq |x - y|$

Gegeben:
$\Lim_{n \to \infi} a_n = a$
$\Rightarrow \forall \epsilon > 0 \E N \in \N: |a_n -a| < \epsilon \F n \geq N$

Beh.:
$\Lim_{n \to \infi}|a_n| = |a|$

z.z.: 
$\forall \epsilon > 0 \E N \in \N : ||a_n| - |a||< \epsilon \F n \geq N$

$\Rightarrow ||a_n|-|a||\leq |a_n-a| < \epsilon \F n \geq N$ (aus der Voraussetzung erfüllt)

$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


c)
Gegeben:
$\lim a_n = a$ 

Beh.: 
$\lim \sqrt{|a_n|} = \sqrt{|a_n|}$

Beweis:
z.z.:
$\forall \epsilon > 0 \E N \in \N : |\sqrt{|a_n|}- \sqrt{|a|}|< \epsilon \F n \geq N$

$\Rightarrow |\sqrt{|a_n|}-\sqrt{|a|}|$

$= \Frac{|(\sqrt{|a_n|} - \sqrt{|a|})| \cdot |(\sqrt{|a_n} + \sqrt{|a|})|}{|\sqrt{|a_n|} + \sqrt{|a|}|}$

$=\Frac{|a_n - a|}{|\sqrt{|a_n}+ \sqrt{|a|}|} \leq \frac{||a_n| - |a||}{|\sqrt{|a_n|} + \sqrt{|a|}|} \leq \frac{\epsilon}{|\sqrt{|a_n|} + \sqrt{|a|}|}$  
....
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


A2)
a)
$(a_n) \to 0$, $a_n > 0 \F n \geq N$, $N \in \N$ 
$\Rightarrow \forall \epsilon > 0 \E N: |a_n|< \epsilon \F n \geq N$

$b_n := \frac{1}{a_n}$
Beh.:
$\Lim b_n = \infi$

z.z.:
$\F K \in \R \E N \in \N : K < b_n \F n \geq N$ 

Für $K \leq 0$ ist diese Aussage trivial, da $a_n > 0 \Rightarrow \frac{1}{b_n} > 0$

Sei $K \in \R >0$ 
$\Rightarrow K < b_n \Leftrightarrow \frac{1}{b_n} < \frac{1}{K}$

$\Rightarrow a_n < \frac{1}{K}$

alternativ z.z.:
$\F K \in \R^+ \E N\in \N :a_n < \frac{1}{K} \F n \geq N$

Sei $\epsilon = \frac{1}{K}$ 
$\Rightarrow \forall \epsilon >0 \E N \in \N: a_n < \epsilon \F n \geq N$
(ist als Voraussetzung wahr)
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

b)
Gegeben:
$a_n := \frac{n}{2^n}$

z.z.:
$\Lim a_n = 0$
$\Leftrightarrow \forall \epsilon > 0 \E N \in \N: |a_n -0|< \epsilon \F n \geq N$

Sei $\epsilon >0$
Nach Blatt 1 wissen wir: $2^n \geq n^2 \F n \geq 5 \Rightarrow \Frac{1}{n^2} \geq \frac{1}{2^n} \F n \geq 5$
$\Rightarrow |\Frac{n}{2^n}| \leq |\frac{n}{n^2}| \F n \geq 5$

$\Rightarrow |\Frac{n}{2^n}| \leq |\frac{1}{n}| \F n \geq 5$

$\Rightarrow$ Nach Korr. 2.4 $\exists N \geq 5 \in \N: 0 < |\Frac{n}{2^n}| \leq |\frac{1}{n}| < \epsilon$ 
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


c)
Lemma:
$n^n > (n+1)! \F n \geq 3$
Beweis:

Induktionsanfang:
n = 3:
$3^3 = 27 > 24 = 4!$

Induktionsschritt:
Wir wissen für ein $n\geq 3 \in \N$ gilt: $n^n > (n+1)!$

-> n+1

$(n+2)! = (n+1)! \cdot (n+2) < (n+2) n^n = n^{n+1} + 2n^n < 2n^{n+1} \leq (n+1)^{n+1}$ 
...

Gegeben:
Sei $a_n := \frac{n!}{n^n}$
$\forall \epsilon > 0  \E N \in \N: |a_n -0| < \epsilon \F n\geq N$

$\Rightarrow |a_n| = |\frac{n!}{n^n}|\stackrel{Lemma}< |\frac{n!}{(n+1)!}| = |\frac{1}{n}|$

Nach Korr.2.4 folgt: $\E N \in \N: 0 <  |\frac{1}{N}|< \epsilon$
$\Rightarrow |a_n| = \frac{n!}{n^n} < |\frac{1}{n}| \leq |\frac{1}{N}| < \epsilon$
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

A3)
a)
$a_n := \Frac{1}{\sqrt[3]{n+1}}$

Beh. :$\Lim a_n = 0$
Bew:

Sei $\epsilon > 0$

Wir wissen:
$\exists N: 0 < \Frac{1}{\sqrt[3]{N+1}}< \epsilon$ (Kor.2.4)

$\Rightarrow |a_n - 0| = |a_n| = \frac{1}{\sqrt[3]{n+1}} \leq \frac{1}{\sqrt[3]{N+1}} < \epsilon \F n \geq N$ 
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


b)
$b_n := \Frac{2n^2-7n+9}{n \cdot (n+2)}$

Durch Polynomdivision kann man diesen Bruch übersetzen:
$(2n^2-7n+9):(n^2+2n)= 2 + \frac{-11n +9}{n^2+2n}$
$(-2n^2 -4n)$
-----------
$-11n + 9$

$\Rightarrow b_n= 2 + \Frac{-11n+9}{n^2+2n}$ (dieses Ergebniss kann man leicht durch Rückrechnen überprüfen)

Nun kann man eine Partialbruchzerlegung durchführen:
$\Frac{-11n + 9}{n(n+2)} = \frac{A}{n} + \frac{B}{n+2}$

$\stackrel{\cdot n(n+2)}\Leftrightarrow-11n + 9 = A(n+2) + Bn$
n = -2:
$22 + 9 = -2B$
$B = \Frac{-31}{2}$

n = 0:
$9 = 2A$
$A = \Frac{9}{2}$

$\Rightarrow b_n = 2+ \Frac{9}{2n} - \frac{31}{2n +4}$ (erneut kann das Ergebniss schnell durch Rückrechnung überprüft werden)
$\Rightarrow \Lim b_n$ 
$= \Lim(2 + \frac{9}{2n}- \frac{31}{2n +4})$
$= \Lim 2 + \Lim \frac{9}{2n} - \Lim \frac{31}{2(n +2)}$
$= 2 + \Lim \frac{9}{2} \cdot \Lim \frac{1}{n} - \Lim \frac{31}{2} \cdot \Lim \frac{1}{n+2}$
$= 2 + \frac{9}{2} \cdot 0 - \frac{31}{2} \cdot 0$
$= 2$
$\blacksquare$


c)
$c_n := \Frac{(-1)^n n^2 - n^2 -1}{n+3}$

Divergent:
1.:
Wenn n = 2m, $m \in \N$:
$c_{2m} = \frac{(-1)^{2m}(2m)^2-(2m)^2 - 1}{n+3}$
$= \frac{-1}{n + 3}$

-> n = 2m +1
$c_{2m + 1} = \frac{-(2m+1)^2 - (2m+1)^2 -1}{n +3}$
$=\frac{-2(2m+1)^2 - 1}{n + 3} < c_{2m}$

aber $c_{2m+2} = \frac{-1}{n + 3} > c_{2m + 1}$

$\Rightarrow$ Die Folge ist gegen unendlich unbeschränkt und somit nicht konvergent


d)
$d_n := \sqrt{n^2 +1}-n$
$= \Frac{(\sqrt{n^2 +1} - n)(\sqrt{n^2 +1} + n)}{\sqrt{n^2+1}+n}$

$= \Frac{n^2 + 1 - n^2}{\sqrt{n^2 + 1} + n}$ 

$= \Frac{1}{\sqrt{n^2+1}+n}$

Beh.:
$\Lim d_n = 0$
Beweis:

z.z.: 
$\forall \epsilon > 0 \E N \in \N: |\frac{1}{\sqrt{n^2+1}+n}| < \epsilon \F n \geq N$

Wir wissen:
$\E N: 0 < |\frac{1}{\sqrt{n^2 +1}+n}| < \epsilon$ (Kor.2.4)
$\Rightarrow |\frac{1}{\sqrt{n^2+1}+n}| \leq |\frac{1}{\sqrt{N^2+1}+N}|< \epsilon$ 
$\blacksquare$


A4)
Gegeben:
$M \neq \es$, $M\subseteq (0, \infi)$, $M':= \set{x \mid x = \frac{1}{y}:y \in M}$

Merke: 
M1:
$x > 0 \F x \in M$    $(I)$
$\Rightarrow \frac{1}{x} > 0 \F x \in M$    $(II)$
$\Rightarrow y > 0 \F y \in M'$     $(III)$


M2:
$x \in M \Leftrightarrow \frac{1}{x} \in M'$
$\Rightarrow (x \in M' \Leftrightarrow \frac{1}{x} \in M)$


z.z.:
M' beschränkt nach Oben $\Leftrightarrow$ $\inf M > 0$

1)
z.z.: $\inf M > 0 \Rightarrow$ M' beschränkt nach Oben:


Sei $M \subseteq (0, \infi): m = \inf M > 0$
$\Rightarrow \lnot \exists a \in M: a < m$    $(I)$

Annahme:
M' ist nicht nach oben beschränkt.
$\Rightarrow \forall b \in \R \E x \in M': x > c$
$\Rightarrow \exists x_1 \in M': x_1 > \frac{1}{m}$
$\stackrel{m, x_1 > 0}\Leftrightarrow m > \frac{1}{x_1}$
$\Rightarrow \frac{1}{x_1} \in M : \frac{1}{x_1} < m \contrana (I)$
$\Rightarrow$
M' muss nach oben beschränkt sein
$\checkmark$


2)
z.z.: M' nach oben beschränkt $\Rightarrow \inf M > 0$

Sei M' nach oben beschränkt.
$\Rightarrow \exists a \in \R: x \leq a \F x \in M' \Leftrightarrow \sup M' = a$ (es existiert ein supremum für M')

Annahme:
$\inf M \leq 0$

Fallunterscheidung:
a) $\inf M < 0$
$\Rightarrow \inf M \leq \min M \leq 0$
$\Rightarrow \exists y \in M: y \leq 0 \contrana M1.I$

$\inf M = 0$
$\stackrel{M1.I}\Rightarrow$ $\min M$ existiert nicht
Beh. $\forall z \in \R^+ \E m \in M: m < z$ ($m\in M$ kann beliebig nahe zu 0 werden)
{Bew: 
Angenommen: $\exists z \in \R^+ \F m \in M: z \leq m$
$\Rightarrow 0 < z \leq m \F m \in M$
$\Rightarrow \inf M < z \leq m \F m \in M$ $\contrana$}

$\Rightarrow  \forall z \in \R^+ \E m \in M: z > m$
$\stackrel{M1.I}\Leftrightarrow \frac{1}{m} > \frac{1}{z}$

Wähle $z = \frac{1}{a} \Rightarrow a = \frac{1}{z}$

$\Rightarrow \E m \in M: \frac{1}{m} > a$
$\Rightarrow \frac{1}{m} \in M'$
$\Rightarrow \exists \frac{1}{m} \in M': \frac{1}{m} > \sup M' \contrana$

$\Rightarrow \inf M > 0$
$\blacksquare$

z.z: $\inf M > 0 \Rightarrow (\inf M)^{-1} = \sup M'$

Sei $\inf M = a > 0$
$\Rightarrow \exists \sup M' = b$ (vorher bewiesen)

z.z.:
$\frac{1}{a} = \sup M'$
$\Leftrightarrow 
a) $(\frac{1}{a} \geq x \F x \in M') \land$ 
b) $((\exists t \in \R: x \leq t \F x \in M') \Rightarrow \frac{1}{a} \leq t)$

a) 
$a = \inf M \Rightarrow y \geq a \F y \in M$
$\Rightarrow \frac{1}{a} \geq \frac{1}{y} \F y \in M$
$\Rightarrow \frac{1}{a} \geq x \F x \in M'$

b)
$a = \inf M \Rightarrow ((\exists t \in \R: x \geq t \F x \in M) \Rightarrow a \geq t)$ 
$\Rightarrow ((\exists \frac{1}{t} \in \R : \frac{1}{t} \geq \frac{1}{x} \F x \in M)\Rightarrow \frac{1}{t} \geq \frac{1}{a})$
$\stackrel{t' = \frac{1}{t}}\Rightarrow ((\exists t' \in \R: t' \geq y \F y \in M') \Rightarrow t' \geq \frac{1}{a})$
$\Rightarrow \frac{1}{a} = \sup M'$ 
$\Rightarrow (\inf M)^{-1} = \sup M'$
$\blacksquare$



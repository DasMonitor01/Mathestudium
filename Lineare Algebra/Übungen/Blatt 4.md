## Aufgabe 4.5
Sei $M_n := \set{a_1, a_2, ... a_n}$ eine Menge
und $I_n : \set{1, 2 , ... , n}$
und $F_n := \set{f | f\ bijektion\ von\ M_n\ nach\ I_n}$


Induktionsanfang:
$M_1 = \set{a_1}$ 
$I_1 = \set{1}$

Es gibt folglich genau eine (paarweise verschiedene) Bijektion
$f_1 : M_1 \to I_1, a_1 \onto 1$
$\Rightarrow F_1 = \set{f_1}$
$|F_1| = 1 = 1!$


Induktionsschritt:
Wir wissen, für ein $n \in \N$ gibt es n! bijektionen zwischen $M_n$ und $I_n$. Dann folgt für n+1:

$M_{n+1} = M_n \cup \set{a_{n+1}} = \set{a_1, a_2, ..., a_n, a_{n+1}}$ 
$I_{n+1} = \set{1, 2, ..., n, n+1}$

Die $n!$ bijektionen aus $F_n$ können nun auf $M_{n+1}$ und $I_{n+1}$ erweitert werden, indem sie zusätzlich $a_{n+1}$ auf ein $m \leq n+1$ abbilden, und das Element das f an diese Stelle ursprünglich abgebildet hat auf n+1 abbilden. 
So entstehen zu jeder bijektion aus $F_n$ (n+1) verschiedene Sub-Bijektionen, die $a_{n+1}$ mit einem Element vertauschen.
Folglich existieren nun $n! \cdot (n+1) = n!$ bijektionen zwischen $M_{n+1}$ und $I_{n+1}$
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

## Aufgabe 4.6

a)
z.z.: $\Sum_{k=1}^{n}k^3 = \biggl(\Frac{n \cdot (n+1)}{2}\biggl)^2 \F n \in \N$ 

Beweis durch Induktion:

Induktionsanfang:
$n = 1$:

$\Sum_{k=1}^1 k^3 = 1^3 = 1$ 

$\biggl(\Frac{1 \cdot (1 + 1)}{2}\biggl)^2 = \biggl(\Frac{2}{2}\biggl)^2 = 1^2 = 1 = \Sum_{k=1}^{1}k^3$ 


Induktionsschritt:
Wir wissen für ein $n \in \N$ gilt:
$(I)$: $\Sum_{k=1}^{n} k^3 = \biggl(\Frac{n \cdot (n+1)}{2}\biggl)^2$ 
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

Dann folgt für n+1:

$\Sum_{k=1}^{n+1}k^3$
$= \Sum_{k=1}^n + (n+1)^3$
$\stackrel{I}= \biggl(\Frac{n \cdot (n+1)}{2}\biggl)^2 + \Frac{4\cdot (n+1)^3}{4}$ 
$= \Frac{(n \cdot (n+1))^2}{4} + \Frac{4\cdot(n+1) \cdot (n+1)^2}{4}$ 
$= \Frac{n^2 \cdot (n+1)^2 + (4n + 4) \cdot (n+1)^2}{4}$
$= \Frac{(n+1)^2 \cdot (n^2 + 4n + 4)}{4}$ 
$= \Frac{(n+1)^2 \cdot (n+2)^2}{2^2}$ 
$= \Frac{((n+1)\cdot (n+2))^2}{2^2}$
$=\biggl( \Frac{(n+1) \cdot (n+2)}{2}\biggl)^2$
$= \biggl(\Frac{(n+1) \cdot ((n+1)+1)}{2}\biggl)^2$
$\blacksquare$ 
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


b)
z.z.:
$\forall n \in \N: 23 \mid 5^{2n}-2^n$
$\Leftrightarrow \forall n \in \N \E k \in \Z: 23 \cdot k = 5^{2n}-2^n$ 

Beweis durch Induktion

Induktionsanfang:
n = 1:

$5^{2 \cdot 1} - 2^1 = 5^2 - 2^1 = 25 - 2 = 23$
$\Rightarrow 23 \mid 5^{2\cdot 1} - 2^1$

Induktionsschritt:
Wir wissen für ein $n \in \N$ gilt:
$23 \mid 5^{2n}-2^n$ $(I)$
$\Leftrightarrow \exists k \in \N: 23 \cdot k = 5^{2n}-2^n$ $(II)$

Dann folgt für n+1:
$5^{2(n+1)}-2^{n+1}$
$= 5^{2n+2}-2^{n+1}$
$=5^2 \cdot 5^{2n} - 2 \cdot 2^n$
$= 25 \cdot 5^{2n} - 2 \cdot 2^n$
$= (23 + 2) \cdot 5^{2n} - 2 \cdot 2^n$
$= 23 \cdot 5^{2n} + 2 \cdot 5^{2n} - 2 \cdot 2^n$
$= 23 \cdot 5^{2n} + 2 \cdot (5^{2n}- 2^n)$ 
$\stackrel{II}= 23 \cdot 5^{2n} + 2 \cdot 23 \cdot k, k \in \N$ 
$= 23 \cdot (5^{2n} + 2 \cdot k), k \in \N$ 
$\Rightarrow 23 \mid 5^{2(n+1)}-2^{n + 1}$ 
$\blacksquare$ 
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


## Aufgabe 4.7
Gegeben:
$R \subseteq (\N_0 \x \N_0) \x (\N_0 \x \N_0)$ mit
$\forall a,b,c,d \in \N_0: (a,b) \tilde (c,d) \Leftrightarrow a+d = b+c$

a) 
Sei $x := (1,3)$ und $y := (6, 8)$
$\Rightarrow 1 + 8 = 3 + 6$
$\Rightarrow x \tilde y$


b)
R äquivalenzrelation $\Leftrightarrow$ R reflexiv $\land$ R symmetrisch $\land$ R transitiv

Reflexivität:
Sei $x := (a,b) \in \N_0 \x \N_0$ 

$a + b$
$= b + a$  (Kommutativität der Addition der natürlichen Zahlen)

$\Rightarrow x \tilde x$ 
$\checkmark$ 

Symmetrie:
Seien $x := (a,b), y := (c+d) \in N_0 \x N_0$ 
mit $x \tilde y$
$\Rightarrow a + d = b + c$ 
$\Leftrightarrow c + b = d + a$ (Kommutativität der Addition der natürlichen Zahlen)
$\Rightarrow y \tilde x$ 
$\checkmark$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

Transitivität:
Seien $x:=(a,b), y:=(c,d), z:=(e,f) \in \N_0 \x \N_0$
mit $(I)$ $x \tilde y$ und $(II)$ $y \tilde z$ 
$\stackrel{I}\Rightarrow a + d = b + c$
$\Leftrightarrow d = b + c - a$ $(III)$

$(II) \Rightarrow c + f = d + e$ 
$\stackrel{III}\Rightarrow c + f = b + c - a + e$ 
$\Leftrightarrow a + f = b + e$ 
$\Rightarrow x \tilde z$ 
$\checkmark$ 

$\Rightarrow$ R ist äquivalent
$\blacksquare$

## Aufgabe 4.8:
Gegeben:
$R := \set{(A,B) \in \P(\N) \x \P(\N) \mid A \cap B = \es}$ 
$\Rightarrow A \tilde B \Leftrightarrow A \cap B = \es$ 

- $X := (\set{1}, \set{2}) \in R$ (da $\set{1} \cap \set{2} = \es$)
- $Y := (\set{1}, \set{2,3})\in R$ (da $\set{1} \cap \set{2,3} = \es$)
- $Z := (\set{4,5}, \set{3,8,20000})\in R$ (da $\set{4,5} \cap \set{3, 8, 20000} = \es$) 


$(I)$ R ist nicht Reflexiv:
Denn sei $A \in \P(\N) : A \neq \es$ 
$\Rightarrow A \cap A = A \neq \es$
$\Rightarrow (A, A) \nin R$ 
$\blacksquare$ 
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


$(II)$ R ist symmetrisch:
Seien $A, B \in \P(\N): A \tilde B$ 
$\Rightarrow A \cap B = \es$ 
$\Rightarrow B \cap A = \es$ (Die Schnittmenge ist kommutativ)
$\Rightarrow B \tilde A$ 
$\blacksquare$ 


R ist nicht Transitiv:
Denn seien $A, B, C \in \P(\N): A \tilde B \land B \tilde C$ 
$\stackrel{II}\Rightarrow B \tilde A$ $(III)$
Angenommen R transitiv:
$A \tilde B \land B \tilde C \Rightarrow A \tilde C$
Wähle $C = A$
$\Rightarrow (A \tilde B \land B \tilde A \Rightarrow A \tilde A)$ ($A \tilde B$ ist nach Annahme erfüllt und nach $III$ auch $B \tilde A$)
$\Rightarrow A \tilde A$ $\contrana I$  (Wir wissen nach $I$ das nicht $A \tilde A$ für alle $A \in \P(\N)$ gilt)
$\Rightarrow$ R ist nicht transitiv
$\blacksquare$ 


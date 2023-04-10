# Aufgabe 1
Gesucht: $(b_{n}) : \frac{1}{5} = \Sum_{k=0}^{\infty} b_{k} 7^{-k}$

Betrachte die Division von $1 : 5$ im 7-adischen System:
1:5 = 0,12541254...
10 : 5 // $10_{7} = 7_{10}$
	20:5 // $20_{7} = 14_{10}$
		40:5 // $40_{7} = 28_{10}$
			30 : 5 // $30_{7} = 21_{10}$
				10 : 5 ...

Beh: 
$b_{n} := \Biggl \{ \begin{matrix} 0: n=0 \\ 1 : n \mod 4 = 1 \\ 2: n \mod 4 = 2 \\ 5: n \mod 4 = 3 \\4: n \mod 4 = 0, n >0\end{matrix}$

Hat die Eigenschaft $\Sum_{n=0}^{\infty}b_{n}7^{-n} = \frac{1}{5} = 0.2_{10}$
Also die 7-adische Entwicklung von 
$\frac{1}{5} = 0,125412541254\dots_{7}$
...
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

# Aufgabe 2
### a)
$(I)$
$\Sum_{n=1}^{\infty} \frac{1}{n \cdot \sqrt{n^{2}+1}}$

Merke: $n > 0$ und $\sqrt{n^{2} + 1} \geq \sqrt{n^{2}}$
$\RA n \cdot \sqrt{n^{2} + 1} \geq n \cdot \sqrt{n^{2}} = n^{2}$
$\RA \frac{1}{n^{2}} \geq \frac{1}{n \cdot \sqrt{n^{2} + 1}}$
und $\RA 0 \leq \frac{1}{n \cdot \sqrt{n^{2} + 1}}$
$\RA |\frac{1}{n \cdot \sqrt{n^{2} + 1}}| = \frac{1}{n \cdot \sqrt{n^{2} + 1}}$
$\RA \Sum_{n=1}^{\infty} |\frac{1}{n \cdot \sqrt{n^{2} + 1}}| \leq \Sum_{n=1}^{\infty} \frac{1}{n^{2}}$

aber $\Sum_{n=1}^{\infty} \frac{1}{n^{2}}$ konvergiert, und somit konvergiert $\Sum_{n=0}^{\infty} \frac{1}{n \cdot \sqrt{n^{2} + 1}}$ absolut
$\bs$

$(II)$
Fehlend :(
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

### b)
Sei $(a_{n})_{n \in \N}$ mit
$a_{n} := \biggl\{\begin{matrix} \frac{1}{4k}: n=2k-1, k\geq 1 \\ \frac{1}{2k}:n=2k, k \geq 1 \end{matrix}$
(es wird hier mal davon ausgegangen das $k \in \N$ und nicht z.B. in $\Q$ gelten soll, sonst ergibt die Folgendefinition keinen Sinn)

$n = 2k - 1 \LRA k = \frac{n+1}{2}$
$n = 2k -1, k \in  \N \RA 2 \not \mid n$

$n = 2k \LRA k = \frac{2}{n}$
$n = 2k, k\in \N \RA 2 \mid n$

Damit können wir $a_{n}$ umschreiben zu:
$a_{n} = \biggl \{ \begin{matrix} \frac{1}{4 \cdot \frac{n+1}{2}} : 2 \not \mid n \\ \frac{1}{2 \cdot \frac{n}{2}} : 2 \mid n\end{matrix}$

$a_{n} = \biggl \{ \begin{matrix} \frac{1}{2n+2} : 2 \not \mid n \\ \frac{1}{n} : 2 \mid n \end{matrix}$

Sei $b_{n} := \frac{1}{2(2n-1)+2} = \frac{1}{4n}$

und $c_{n} := \frac{1}{2n}$

wir können nun $a_{n}$ mit diesen Folgen ausdrücken:
$a_{n} = \biggl \{ \begin{matrix} b_{\frac{n+1}{2}} : 2 \not \mid n \\ c_{\frac{n}{2}}: 2 \mid n\end{matrix}$

Betrachte nun $S_{m} = \Sum_{n=1}^{m} (-1)^{n} a_{n}$.

Für $m = 2k$ folgt:
$S_{2k} = \Sum_{n=1}^{2k}(-1)^{n}a_{n} = \Sum_{n=1}^{k} c_{n} - b_{n}$
weil $a_{n}$ abwechselnd durch die Glieder von $b_{n}$ und $c_{n}$
läuft, und $b_{n}$ alle ungeraden Glieder beschreibt, also die, die ein negatives Vorzeichen in der Reihe besitzen

$\RA S_{2k} = \Sum_{n=1}^{k} \frac{1}{2n} - \frac{1}{4n} = \Sum_{n=1}^{k} \frac{2-1}{4n}$
$= \Sum_{n=1}^{k} \frac{1}{4} \cdot \frac{1}{n} = \frac{1}{4} \cdot \Sum_{n=1}^{k} \frac{1}{n}$

Damit folgt sofern die Reihe konvergiert $\Sum_{n=1}^{\infty} (-1)^{n} a_{n} = \limin \frac{1}{4} \cdot \Sum_{n=1}^{k} \frac{1}{n}$
$= \frac{1}{4} \cdot \limin \Sum_{n=1}^{k} \frac{1}{n}$
$= \frac{1}{4} \cdot \Sum_{n=1}^{\infty} \frac{1}{n}$ $\contrana \Sum_{n=1}^{\infty} \frac{1}{n} \to \infty$

Dies steht nicht im Wiederspruch zum Leibnizkriterium, da $a_{n}$ nicht monoton ist:
Betrachte für ein beliebiges $m_{1} \in \N: 2 \not \mid m_{1}$
$a_{m_{1}} = \frac{1}{2m_{1}+2} < \frac{1}{2m_{1}+1} = a_{m_{1}+1} > \frac{1}{2m_{1} +6} =\frac{1}{2(m_{1}+2)+2} = a_{m_{1}+2}$
also $a_{m_{1}} < a_{m_{1}+1} > a_{m_{1}+2}$
und somit kann $a_{n}$ nicht monoton sein.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>


# Aufgabe 3
### a)
Sei $z \in \C : z^{2} = i$, $z = a + bi: a,b \in\R$
$\RA (a+bi)^{2} = 0 + i$
$\RA a^{2} - b ^{2} + 2abi = 0 + i$
Es gilt $Re((a+bi)^{2} = Re(0+i)) \RA a^{2} - b^{2} = 0$
und $Im((a+bi)^{2}) = Im(0+i) \RA 2ab = 1$
$\RA \begin{matrix}(I)\ a^{2}-b^{2} = 0 \\ (II)\ \ \ \ \ \ 2ab = 1\end{matrix}$
$\RA b = \frac{1}{2a}$
$\RA a^{2} - \left( \frac{1}{2a} \right)^{2} = 0$
$\RA a^{2} - \frac{1}{4a^{2}} = 0$
da defintiv gelten muss, $a \neq 0$ (weil division durch a), können wir mit $a^{2}$ multiplizieren
$\RA a^{4} - \frac{1}{4} = 0$
$\RA a^{4} = \frac{1}{4}$
da $\frac{1}{4} > 0$, können wir die eindeutig definierte nichtnegative Wurzel ziehen:
$\RA a^{2} = \sqrt\frac{1}{4} = \frac{1}{2}$
$\RA a = \sqrt \frac{1}{2} = \frac{1}{\sqrt{2}} = \frac{{\sqrt 2}}{2}$
$b = \frac{1}{2a} \RA b = \frac{1}{2 \cdot \frac{\sqrt{2}}{2}} = \frac{1}{\sqrt 2} = {\frac{\sqrt{2}}{2}}$
$\RA z_1 = \frac{\sqrt 2}{2} + \frac{\sqrt 2}{2} i$ löst die Gleichung $z^{2} = i$

Aber:
$i^{2} = (-i)^{2}$
$\RA z_{2} = \frac{\sqrt 2}{2} - \frac{\sqrt 2}{2} i$ löst auch die Gleichung $z^{2} = i$
$\bs$

### b)
$z = \frac{{10+i}}{2-3i} = \frac{(10+i) \cdot (2+3i)}{(2-3i) \cdot (2+3i)} = \frac{{17+5i}}{4 + 9} = \frac{17}{13} + \frac{5}{13} i$

### c)
$z = \Sum_{k=0}^{\infty}2^{-k} i^{k} = \Sum_{k=0}^{\infty} \frac{1}{2^{k}} \cdot i^{k}$
$= \Sum_{k = 0}^{\infty} \frac{i^{k}}{2^{k}}$
$= \Sum_{k=0}^{\infty} \left( \frac{i}{2} \right)^{k}$
Aber $|\frac{i}{2}| = \sqrt{\left( \frac{1}{2} \right)^{2}} = \frac{1}{2} < 1$

Sei $S_{n} := \Sum_{k=0}^{n}\left( \frac{i}{2} \right)^{k}$
nach der Geometrischen Summe (beweis vom reellen ist trivial auf komplexe Zahlen erweiterbar, siehe Anhang A3.c) gilt:

$S_{n} = \frac{1 + \left( \frac{i}{2} \right)^{n}}{1-\left( \frac{i}{2} \right)}$

$\Sum_{n=0}^{\infty} 2^{-k} i^{k} = \limin S_{n}$
$=\limin \frac{1+\left( \frac{i}{2} \right)^{n}}{1-\left( \frac{i}{2} \right)}$
$= \frac{\limin 1+ \left( \frac{i}{2} \right)^{n}}{\limin 1 - \frac{i}{2}}$
$\d= \frac{1 + \limin \left( \frac{i}{2} \right)^{n}}{1- \frac{i}{2}}$

Beh: $\limin \left( \frac{i}{2} \right)^{n} =0$
Beweis:
Betrachte $|\left( \frac{i}{2} \right)^{n} - 0| = |(\frac{i}{2})^{n}|$
$= \sqrt{\left( \left( \frac{1}{2} \right)^{n} \right)^{2}} \F n \in \N$
$= \left( \frac{1}{2} \right)^{n}$
$= \frac{1}{2^{n}}$
Da aber $\limin \frac{1}{2^{n}} = 0$ gilt, folgt direkt:
$\F \varepsilon > 0 \E N \in \N: | \frac{1}{2^{n}}| < \varepsilon \F n \geq N$
und da $\frac{1}{2^{n}} > 0 \F n \in \N$ gilt folgt damit auch direkt
$\frac{1}{2^{n}} < \varepsilon \F n \geq N$
$\RA |\left( \frac{i}{2} \right)^{n}| < \varepsilon$

$\RA \limin \left( \frac{i}{2} \right)^{n} = 0$

$\d\RA \frac{1+ \limin \left( \frac{i}{2} \right)^{n}}{1 - \frac{i}{2}} =\frac{1+0}{1 - \frac{i}{2}}$

$= \frac{1 \cdot \left( 1+\frac{i}{2} \right)}{\left( 1-\frac{i}{2} \right)\left( 1+ \frac{i}{2} \right)}$
$= \frac{1+ \frac{i}{2}}{1 + \frac{1}{4}}$
$= \frac{1+ \frac{i}{2}}{\frac{5}{4}}$
$= 4 \cdot \frac{1+\frac{i}{2}}{5}$
$= \frac{4}{5} + \frac{2}{5} i$
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

# Aufgabe 4
### a)
Im folgenden meint $\limsup a_{n}$ immer $\d\limsup_{n \to \infty} a_{n}$
Zu zeigen:
$\exists \theta \in (0,1) \E n_{0} \in \N:\F n \geq n_{0}: a_{n} \leq \theta \LRA \limsup a_{n }< 1$

"$\RA$":
Sei $(a_{n}) \subset \R$ mit $\exists \theta \in (0,1) \E n_{0} \in \N:\F n \geq n_{0}: a_{n} \leq \theta$ 
$\RA \sup \{ a_{k} : k\geq N \} \leq \theta \F N \geq n_{0}$ (weil alle Elemente in der Menge kleiner gleich $\theta$ sind.)
$\RA \limsup a_{n} \leq \theta < 1$ 
$\checkmark$

"$\LA$":
Sei $(a_{n}) \subset \R$ mit $\limsup a_{n} < 1$
$\RA \limin (sup \{ a_{k} : k \geq n \}) < 1$, d.h. für N groß genug liegen alle $a_{n}$ nach N unterhalb der Schranke 1

$\RA \E N \in \N: a_{k} < 1 \F k \in N$
$\RA \E \theta \in (0,1) \E N \in \N: a_{k} \leq \theta < 1 \F k \geq N$
$\RA \E \theta \in (0,1) \E n_0 \in \N: \F n \geq n_{0}: a_{n} \leq \theta$
$\bs$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

### b)
Z.z:
$\Sum_{n=0}^{\infty} \frac{1}{(n+2)(n+3)} = \frac{1}{2}$ (das ist der Grenzwert, den ich berechnet habe.)

Konvergenz:
$\Sum_{n=0}^{\infty} \frac{1}{(n+2)(n+3)} = \Sum_{n=0}^{\infty}\frac{1}{n^{2} + 5n + 6}$
Aber:
$5n + 6 > 0 \F n \in \N_{0}$
$\RA n^{2} + 5n + 6 > n^{2}$
$\RA \frac{1}{n^{2}} > \frac{1}{n^{2}+5n+6} \F n \in \N_{0}$ 
und weil $n^{2} >0$ und $5n+6 >0 \F n \in \N_{0}$
$\RA \frac{1}{n^{2}+5n+6} > 0 \F n \in \N_{0}$
$\RA |\frac{1}{n^{2} + 5n + 6}| = \frac{1}{n^{2} + 5n + 6} \F n \in \N_{0}$
$\RA \Sum_{n=0}^{\infty} |\frac{1}{(n+2)(n+3)}| \leq \Sum_{n=0}^{\infty} \frac{1}{n^{2}}$
$\RA$ $\Sum_{n=0}^{\infty} \frac{1}{n^{2}}$ ist Majorante, aber nach der Vorlesung konvergiert dies, daher ist $\Sum_{n=0}^{\infty} \frac{1}{(n+2)(n+3)}$ absolut konvergent.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

Grenzwert $\frac{1}{2}$: 
Wir wenden eine Partialbruchzerlegung auf den Term in der Summe an:
$\frac{1}{(n+2)(n+3)} = \frac{A}{(n+2)} + \frac{B}{(n+3)}$
$\RA 1 = A(n+3) + B(n+2)$
$\RA 1 = A(-3+3) + B(-3+2)$
$\RA 1 = -B$
$\RA -1 = B$
$\RA 1 = A(-2 + 3)$
$\RA 1 = A$
$\RA \frac{1}{(n+2)(n+3)} = \frac{1}{(n+2)}-\frac{1}{(n+3)}$

$\RA \Sum_{n=0}^{\infty} \frac{1}{(n+2)(n+3)} = \Sum_{n=0}^{\infty}\left( \frac{1}{(n+2)}-\frac{1}{(n+3)} \right)$

Betrachte $S_{m} := \Sum_{n=0}^{m} \left( \frac{1}{(n+2)}- \frac{1}{(n+3)} \right)$
$= \left( \frac{1}{2} - \frac{1}{3} \right) + \left( \frac{1}{3} - \frac{1}{4} \right) + \dots + \left( \frac{1}{m+1} - \frac{1}{m+2}\right) + \left( \frac{1}{m+2} - \frac{1}{m+3} \right)$ 
(Das ist die Teleskopreihendarstellung).
Man erkennt hierbei:
$S_{m} = \frac{1}{2} + \left( -\frac{1}{3} + \frac{1}{3} \right) + \left( -\frac{1}{4} + \frac{1}{4} \right) + \dots + \left( -\frac{1}{m+2} + \frac{1}{m+2} \right) - \frac{1}{m+3}$
$= \frac{1}{2} - \frac{1}{m+3}$
$\RA \Sum_{n=0}^{\infty} \frac{1}{(n+2)(n+3)} = \Limin m S_{m}$
$= \Limin m \left( \frac{1}{2} - \frac{1}{m+3}\right)$
$= \Limin m \frac{1}{2} - \Limin , \frac{1}{m+3}$
$= \frac{1}{2} - 0$
$= \frac{1}{2}$
$\bs$

# Anhang:

### A 3.c)
Zu zeigen:
Sei $x \in \C, n \in \N$
$\Sum_{k=0}^{n}{x^k} = \frac{1 - x^{n+1}}{1-x}$

Beweis durch Induktion:

Induktionsanfang:
n = 1:
$LS = \Sum_{k=0}^{n}x^k = \Sum_{k=0}^{1}x^k = x^0 + x^1 = x + 1$
$\d RS = \frac{1 - x^{n+1}}{1 - x}=\frac{1 - x^{1+1}}{1 - x} = \frac{1 - x ^2}{1 - x} = \frac{(1 + x)(1 - x)}{1-x} = x + 1$ 
$\Rightarrow LS = RS$

Induktionsschritt:
$(I)$ Wir wissen für ein $n \in \N$ gilt: $\Sum_{k=1}^{n}{x^k} = \frac{1 - x^{n+1}}{1-x}$ 
-> n+1:

$\Sum_{k=1}^{n+1}{x^k}$
$= \Sum_{k=1}^{n}{x^k}+ x^{n+1}$
$\d \stackrel{I}= \frac{1-x^{n+1}}{1-x} + x^{n+1}$
$\d = \frac{1 - x^{n+1}}{1-x} + \frac{(1-x)x^{n+1}}{1-x}$
$\d = \frac{1 - x^{n+1}}{1-x}+ \frac{x^{n+1} - x^{n+2}}{1 - x}$
$\d = \frac{1 - x^{n+1} + x^{n+1} - x^{n+2}}{1 - x}$
$\d \frac{1 - x^{n+2}}{1 - x}$
$\blacksquare$
(ja, dass ist genau der selbe Beweis, wie in der 2. Übungsserie, nur das nun $x \in \C$ statt in $\R$ gilt :)
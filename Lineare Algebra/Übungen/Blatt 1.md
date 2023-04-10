### Aufgabe 1.5:
Es gelten folgende Wichtigkeiten:
$(I): w_1 = w_2$
$(II): w_2 = \frac{1}{2} w_1 + \frac{1}{2} w_3$ 
$(III):w_3 = \frac{1}{2} w_1 + w_4$
$(IV):w_4 = w_5$
$(V):w_5 = \frac{1}{2} w_3$ 

$w_2 \stackrel{I} = \frac{1}{2} w_2 + \frac{1}{2} w_3$ 
$\stackrel{- \frac{1}{2} w_2} \Leftrightarrow \frac{1}{2} w_2 = \frac{1}{2} w_3$ 
$\stackrel{\cdot 2} \Leftrightarrow w_2 = w_3$
$\Rightarrow (VI): w_1 \stackrel{I} = w_2 = w_3$ 

$w_3 \stackrel{VI} = \frac{1}{2} w_3 + w_4$
$\stackrel{-\frac{1}{2} w_3} \Leftrightarrow \frac{1}{2} w_3 = w_4$ 
$\stackrel{\cdot 2} \Leftrightarrow (VII): w_3 = 2w_4 \stackrel{IV}= 2 w_5$ 

$w_5 \stackrel{VII} = w_5$ 

$\Rightarrow$ Das Gleichungssystem liefert keine Eindeutige Lösung, die Menge aller Lösungen ergibt sich wie folgt $\mathbb L = \set{l \mid l = a \cdot (2,2,2,1,1): a \in \mathbb R}$ , also alle Tupel, die ein Vielfaches der Tupels $(2,2,2,1,1)$ dastellen, wobei $a \cdot (x_1,x_2,x_3,x_4,x_5) := (a \cdot x_1, a \cdot x_2, a \cdot x_3, a \cdot x_4, a \cdot x_5)$ und eine Lösung das Format $l = (x_1, x_2, x_3, x_4, x_5) :\Leftrightarrow (w_1 = x_1, w_2 = x_2, w_3 = x_3, w_4 = x_4, w_5 = x_5)$ meint
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

### Aufgabe 1.6
a)
z.z.: 
$(I.a):(A \land B) \land C \Leftrightarrow A \land (B \land C)$

Beweis durch Wahrheitstafel:

 A | B | C | $A \land B$ | $B \land C$ | $(A \land B) \land C$ | $A \land (B \land C)$ 
 --- | --- | --- | --- | --- | --- | --- 
 w | w | w | w | w | w | w 
 w | w | f | w | f | f | f 
 w | f | w | f | f | f | f 
 w | f | f | f | f | f | f 
 f | w | w | f | w | f | f 
 f | w | f | f | f | f | f 
 f | f | w | f | f | f | f 
 f | f | f | f | f | f | f 
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

z.z.:
$(I.b):(A \lor B) \lor C \Leftrightarrow A \lor (B \lor C)$

Beweis durch Wahrheitstafel:

 A | B | C | $A \lor B$ | $B \lor C$ | $(A \lor B) \lor C$ | $A \lor (B \lor C)$ 
 --- | --- | --- | --- | --- | --- | --- 
 w | w | w | w | w | w | w 
 w | w | f | w | w | w | w 
 w | f | w | w | w | w | w 
 w | f | f | w | f | w | w 
 f | w | w | w | w | w | w 
 f | w | f | w | w | w | w 
 f | f | w | f | w | w | w 
 f | f | f | f | f | f | f 
$\blacksquare$ 
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

b)
z.z.: 
$(II.a):A \land B \Leftrightarrow B \land A$

Beweis durch Wahrheitstafel:

 A | B | $A \land B$ | $B \land A$ 
 --- | --- | --- | --- 
 w | w | w | w 
 w | f | f | f 
 f | w | f | f 
 f | f | f | f 
$\blacksquare$

z.z.:
$(II.b)A \lor B \Leftrightarrow B \lor A$ 

Beweis durch Wahrheitstafel:

 A | B | $A \lor B$ | $B \lor A$ 
 --- | --- | --- | --- 
 w | w | w | w 
 w | f | w | w 
 f | w | w | w 
 f | f | f | f 
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

c)
$(III.a)$: z.z.:
$(A \land B) \lor C \Leftrightarrow (A \lor C) \land (B \lor C)$ 

Beweis durch Wahrheitstafel:

 A | B | C | $A \land B$ | $A \lor C$ | $B \lor C$ | $(A \land B) \lor C$ | $(A \lor C) \land (B \lor C)$ 
 --- | --- | --- | --- | --- | --- | --- | --- 
 w | w | w | w | w | w | w | w 
 w | w | f | w | w | w | w | w 
 w | f | w | f | w | w | w | w 
 w | f | f | f | w | f | f | f 
 f | w | w | f | w | w | w | w 
 f | w | f | f | f | w | f | f 
 f | f | w | f | w | w | w | w 
 f | f | f | f | f | f | f | f 
 $\blacksquare$

$(III.b)$: z.z.:
$(A \lor B) \land C \Leftrightarrow (A \land C) \lor (B \land C)$ 

Beweis durch Wahrheitstafel:

 A | B | C | $A \lor B$ | $A \land C$ | $B \land C$ | $(A \lor B) \land C$ | $(A \land C) \lor (B \land C)$ 
 --- | --- | --- | --- | --- | --- | --- | --- 
 w | w | w | w | w | w | w | w 
 w | w | f | w | f | f | f | f 
 w | f | w | w | w | f | w | w 
 w | f | f | w | f | f | f | f 
 f | w | w | w | f | w | w | w 
 f | w | f | w | f | f | f | f 
 f | f | w | f | f | f | f | f 
 f | f | f | f | f | f | f | f 

$\blacksquare$ 

### Aufgabe 1.7:
a)
"Entweder ist Aussage A wahr oder es ist Aussage B wahr, aber nicht beides gleichzeitig"
$\Leftrightarrow (A \land \lnot B) \lor (\lnot A \land B)$ 

$(IV.a)$: Beweis durch Wahrheitstafel:

 A | B | $\lnot A$ | $\lnot B$ | $A \land \lnot B$ | $\lnot A \land B$ | $(A \land \lnot B) \lor (\lnot A \land B)$ 
 --- | --- | --- | --- | --- | --- | --- 
 w | w | f | f | f | f | f 
 w | f | f | w | w | f | w 
 f | w | w | f | f | w | w 
 f | f | w | w | f | f | f 

Negation: 

$\lnot ((A \land \lnot B) \lor (\lnot A \land B))$
$\Leftrightarrow (A \land B) \lor (\lnot A \land \lnot B)$ 

$C :\Leftrightarrow (A \land \lnot B) \lor (\lnot A \land B)$ (um Platz zu sparen)

 -> z.z.:
 $\lnot C \Leftrightarrow (A \land B) \lor (\lnot A \land \lnot B)$ 

Beweis durch Wahrheitstafel (C aus $IV.a$ entnommen):

 A | B | $\lnot A$ | $\lnot B$ | C | $(A \land B)$ | $(\lnot A \land \lnot B)$ | $\lnot C$ | $(A \land B) \lor (\lnot A \land \lnot B)$ 
 --- | --- | --- | --- | --- | --- | --- | --- | --- 
 w | w | f | f | f | w | f | w | w 
 w | f | f | w | w | f | f | f | f 
 f | w | w | f | w | f | f | f | f 
 f | f | w | w | f | f | w | w | w 
$\blacksquare$

Ausformuliert:
Entweder sind A und B beide wahr, oder A und B sind beide falsch, aber nicht nur eine von beiden.

b)
Aussage A ist genau dann wahr, wenn aus der Aussage B die Aussage C folgt.
$\Leftrightarrow (A \Leftrightarrow (B \Rightarrow C))$ 
$\Leftrightarrow (A \Rightarrow (B \Rightarrow C)) \land ((B \Rightarrow C) \Rightarrow A)$ 
$(IV.b)$: Beweis durch Wahrheitstafel:

 A | B | C | $B \Rightarrow C$ | $A \Rightarrow (B \Rightarrow C)$ | $(B \Rightarrow C) \Rightarrow A$ | $(A \Rightarrow (B \Rightarrow C)) \land ((B \Rightarrow C) \Rightarrow A)$ 
 --- | --- | --- | --- | --- | --- | --- 
 w | w | w | w | w | w | w 
 w | w | f | f | f | w | f 
 w | f | w | w | w | w | w 
 w | f | f | w | w | w | w 
 f | w | w | w | w | f | f 
 f | w | f | f | w | w | w 
 f | f | w | w | w | f | f 
 f | f | f | f | w | w | w 
 
Zur errinerung: Die letzte Spalte muss immer dann wahr sein, wenn A und $(B \Rightarrow C)$ gleich sind, und falsch, wenn nicht.

Negation:
$\lnot (A \Leftrightarrow (B \Rightarrow C))$ 
$\Leftrightarrow (\lnot A \Leftrightarrow (B \Rightarrow C))$

Ausgesprochen:
Aussage A ist genau dann falsch, wenn aus Aussage B Aussage C folgt.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

### Aufgabe 1.8:
Erinnerung:
$(I.b)$: $(A \lor B) \lor C \Leftrightarrow A \lor (B \lor C)$
$(II.b)$: $A \lor B \Leftrightarrow B \lor C$
$(III.a)$: $(A \land B) \lor C \Leftrightarrow (A \lor C) \land (B \lor C)$ 
(Beweise siehe oben: \[$(I.b)$ in 1.6 a); $(II.b)$ in 1.6 b); $(III.a)$ in 1.6 c)\])

Lemma:
L1:
$(A \lor \lnot A) \Leftrightarrow wahr$ 

Beweis durch Wahrheitstafel:

 A | $\lnot A$ | $A \lor \lnot A$ 
 --- | --- | --- 
 w | f | w 
 f | w | w 
$\blacksquare$
L2:
$(wahr \land A) \Leftrightarrow A$
Beweis durch Wahrheitstafel:

 A | wahr | $A \land wahr$ 
 --- | --- | --- 
 w | w | w 
 f | w | f 
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

L3:
$A \Rightarrow B \Leftrightarrow \lnot A \lor B$ 

Beweis durch Wahrheittafel:

 A | B | $\lnot A$ | $A \Rightarrow B$ | $\lnot A \lor B$ 
 --- | --- | --- | --- | --- 
 w | w | f | w | w 
 w | f | f | f | f 
 f | w | w | w | w 
 f | w | w | w | w 

L4:
$A \land A \Leftrightarrow A$

Beweis durch Wahrheitstafel:

 A | $A \land A$ 
 --- | --- 
 w | w 
 f | f  
$\blacksquare$

L5:
$\lnot(A \land B) \Leftrightarrow (\lnot A \lor \lnot B)$ 

Beweis durch Wahrheitstafel:

 A | B | $\lnot A$ | $\lnot B$ | $A \land B$ | $\lnot(A \land B)$ | $\lnot A \lor \lnot B$ 
 --- | --- | --- | --- | --- | --- | --- 
 w | w | f | f | w | f | f 
 w | f | f | w | f | w | w 
 f | w | w | f | f | w | w 
 f | f | w | w | f | w | w 
$\blacksquare$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

L6:
$\lnot(\lnot A) \Leftrightarrow A$

Beweis durch Wahrheitstafel: 

 A | $\lnot A$ | $\lnot(\lnot A)$ 
 --- | --- | --- 
 w | f | w 
 f | w | f 
$\blacksquare$

a)
$(A \land B) \lor \lnot A$ 
$\stackrel{III.a}\Leftrightarrow (A \lor \lnot A) \land (B \lor \lnot A)$ 
$\stackrel{L1, L2}\Leftrightarrow B \lor \lnot A$ 
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

b)
$(A \barwedge B) :\Leftrightarrow \lnot(A \land B)$
Wahrheitstabbelle:

 A | B | $A \land B$ | $A \barwedge B$ 
 --- | --- | --- | --- 
 w | w | w | f 
 w | f | f | w 
 f | w | f | w 
 f | f | f | w 

Behauptung:
$(A \Rightarrow B) \Leftrightarrow (A \barwedge (B \barwedge B))$ 

Beweis:
$A \barwedge (B \barwedge B)$
$\Leftrightarrow A \barwedge (\lnot (B \land B))$ 
$\Leftrightarrow \lnot (A \land \lnot(B \land B)$ 
$\stackrel{L4}\Leftrightarrow \lnot(A \land \lnot B)$ 
$\stackrel{L5} \Leftrightarrow \lnot A \lor \lnot(\lnot B)$
$\stackrel{L6}\Leftrightarrow \lnot A \lor B$
$\stackrel{L3} \Leftrightarrow (A \Rightarrow B)$ 
$\blacksquare$

c)
Behauptung: 
$(\lnot A \land B \Rightarrow C) \Leftrightarrow (\lnot C \Rightarrow A \lor \lnot B)$

Beweis:
$\lnot A \land B \Rightarrow C$
$\stackrel{L3} \Leftrightarrow \lnot(\lnot A \land B) \lor C$
$\stackrel{L5}\Leftrightarrow (A \lor \lnot B) \lor C$
$\stackrel{I.b, II.b}\Leftrightarrow C \lor (A \lor \lnot B)$
$\stackrel{L6}\Leftrightarrow \lnot(\lnot C) \lor (A \lor \lnot B)$
$\stackrel{L3}\Leftrightarrow (\lnot C \Rightarrow A \lor \lnot B)$
$\blacksquare$

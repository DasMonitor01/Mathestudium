In diesem Abschnitt betrachten wir Matrizen ausschließlich über einem Körper K. Zudem lassen wir das Multiplikationszeichen * nun oft weg, d.h. $A* B = AB$

Ziel des Abschnintts:
Zu einer gegebenen Matrix $A \in K^{n,m}$ Konstruiere ein $S \in Gl_{n}(K),$ so dass $SA = C$ eine quasi-obere Dreiecksmatrix ist.
Hierbei ist S das Produkt von Elementarmatrizen der Form (1), (2), (3)
Die Matrix $C \in K^{n,m}$ soll am Ende die folgende Gestalt haben:

# Defintion 5.2
Wir sagen dass eine Matrix $C \in K^{n,m}$ in Treppennormalform ist, falls 
"insert image here"

Formaler: C ist entweder die Nullmatrix oder es gibt eine Folge $(j_n) = (j_{1},j_{2}, j_{3}, j_{4},\dots,j_{r})$ mit $r \in \{ 1,\dots,min(n,m) \}$
und $j_{n}$ monoton steigend, $1 \leq j_{1} < j_{r}\leq m$, so dass
1) $[C]_{i,j} = 0$ für $1 \leq i \leq r$ und $1 \leq j  < j_{i}$
2) $[C]_{i,j} = 0$ für $r < i \leq n$ und $1 < j \leq m$
3) $[C]_{i,j_{n}} = 1$ für $1 \leq i \leq r$ und alle Einträge in Spalte $j_{n}$ sind identisch 0.


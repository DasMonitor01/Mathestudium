# Aufgabe 1
#### zum Programm aus 2):
Beim Vergleich der Gleichheit der Instanzen im Testprogram wird auf die Instanzen der Klasse Person ein Aufruf der equals-methode der Klasse ausgeführt.
Da in der Klasse Person aber keine equals-methode definiert wurde, wird die equals-methode aus der Elternklasse Object (Object ist die oberste Elternklasse aller Klassen oder auch die Mutter aller Klassen) verwendet. 
Diese ist jedoch sehr primitiv und vergleicht nur, ob es sich bei dem aufrufenden Objekt und dem übergebnene Objekt um das selbe Objekt (also die gleiche Referenz) handelt. 
Da alle Instanzen der Klasse Person seperat erstellt werden(also keine zwei variablen die selbe Referenz enthalten), ist dies für keine zwei Instanzen der Fall, und der vergleich ist immer falsch. 
Um dies zu beheben, muss die equals-methode von Object durch eine equals-methode der Klasse person überladen werden, die die gewünschten Gleichheitsanforderungen überprüft.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

#### zum Programm aus 3):
Beim Ausgeben der Instanzen im Testprogram wird auf die Instanzen der Klasse Planet ein Aufruf der toString-methode der Klasse ausgeführt (Dies wird von java in teilen auch automatisch gemacht, z.B. im Kontext von String concatination oder in der System.out.print-methode).
Da in der Klasse Planet aber keine toString-methode definiert wurde, wird die toString-methode der Elternklasse Object (Object ist die oberste Elternklasse aller Klassen oder auch die Mutter aller Klassen) verwendet. 
Diese ist jedoch sehr primitiv und liefert nur den Namen der Klasse des Objekts, gefolgt von einem @ und dann dem hash des Objekts in hexadezimaler Form 
(und nein, ich erkläre jetzt nicht nochmal im Detail was ein Hash ist, und wie der Hash für Object zu Stande kommt, oder was die hexadezimale Form ist, kurzgefasst ist es eine eindeutige (aber nicht unbedingt eineindeutige (also bijektive)) Identifizierung eines Objekts mit einer (in diesem Fall hexadezimalen) Zahl),
was defnitiv nicht dem entspricht, was hier als Ausgabe gewünscht ist. Um diesen Fehlverhalten zu beheben, muss in Planet eine toString-methode implementiert werden, die eine Instanz von Planet in die gewünschte Stringrepresentation übersetzt.
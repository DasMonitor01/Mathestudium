# Einleitung

Bei diesem Kurs handelt es sich um einen groben Einstieg in das Programmieren und die Programmiersprache Java.

Aufgrund der angepeilten Länge werden tiefere Konzepte wie etwa die Objektorientierung nur sehr oberflächlich angeschnitten werden. Die Konzepte, die hier vermittelt werden sollen, sind lediglich die Grundstrukturen die für das Arbeiten mit Java nötig sind.

Aufbau:

1. Was ist ein Programm/ Algorithmus
2. Einführung und Installation einer IDE
3. Standardaufbau eines Java Programms
4. "Hello World" oder auch das erste Programm
5. Variablen und simple Datentypen 
6. if- und else-statements, Vergleichsoperatoren
	1. *switches*
7. for und while
8. Methoden
	1. Parameter
	2. Rückgabewerte
	3. Überladung
	4. *Recursion*
9. Scoping
10. Arrays (listen)
	1. *Arraylists*
11. Strings (Das Textdingsda)
12. Klassen und Objekte
	1. Methoden
	2. __Vererbung
	3. __static und final
	4. __public, private und protected

### Zusatz
13. *ENUMs (Enumerations)
14. *Funktionale Programmierung
15. *Nachwort
16. *Anhang

Hinweis:

Das sieht nach viel aus, aber viele dieser Konzepte lassen sich sehr intuitiv verstehen, und bedürfen vor allem von der Sprachlichen Konstruktion (Syntax) Übung. Ein Verständnis für diese Konzepte zu haben reicht als Vorteil für Objektorientierte Programmierung definitiv aus. Zusätzlich sind vor allem nur die Punkte 1 - 12 wirklich wichtig, der Rest wird noch in der Vorlesung zu genüge behandelt.

Legende:
__Fette Themen kommen noch, sobald ich die Zeit dafür gefunden habe__
*Kursive Themen stellen zusätzliche Informationen da, und kommen dementsprechend nur vielleicht, wenn ich die Zeit dazu finde*
<br />

---
_Autor: David Neumann_
_Kontakt für Fehler und Fragen: davidneumann2155@gmail.com_

# 1: Was ist ein Programm/ Algorithmus

Formal definiert ist das etwas kompliziert, deshalb hier eine kurze Erklärung:

Ein Programm ist eine Abfolge von Schritten, die ausgeführt werden sollen.

Beispielsweise kann ein Programm eine Zusammenfassung verschiedener Algorithmen zum Lösen eines Zauberwürfels, oder auch ein System zum Berechnen von verschiedenen Mathematischen Operationen (z.B. Addition, Multiplikation, Taylorreihe, Newton-Methode etc.) sein.

Allgemein folgt ein Programm einer logischen Abfolge von teilschritten, um eine gewünschte Operation durchzuführen

Falls trotzdem jemand die offizielle Definition hören will, bitte sehr:
Ein **Computerprogramm** oder kurz **Programm** ist eine den Regeln einer bestimmten Programmiersprache genügende Folge von Anweisungen (bestehend aus Deklarationen und Instruktionen), um bestimmte Funktionen bzw. Aufgaben oder Probleme mithilfe eines Computers zu bearbeiten oder zu lösen. (Danke [Wikipedia](https://de.wikipedia.org/wiki/Computerprogramm))
<br />

---
_Autor: David Neumann_
_Kontakt für Fehler und Fragen: davidneumann2155@gmail.com_

# 2: Einführung und Installation einer IDE

## Hinweis! Dieser Schritt ist durch die Yapex-Entwicklungsumgebung der Uni-Halle freiwillig geworden. Sie können ihm trotzdem folgen, aber dies ist rein freiwillig. Ich werde weiterhin Hinweise zu IDE-Dingen geben, diese können Sie ignorieren, falls Sie Yapex nutzen.

## 1. Was ist eine IDE:

Bei einer IDE einer sogenannten "integrated develop enviroment" handelt es sich um ein Programm, das einem Funktionalitäten zum einfacheren Entwickeln von Programmen bietet. (z.B. Syntaxkontrolle, Auto Vervollständigung etc.)

Grundsätzlich kann man ein Programm in jedem Texteditor erstellen, es ist aber trotzdem empfehlenswert, eine IDE zu verwenden, um sich einiges an Arbeit zu sparen.

Es gibt verschiedene IDEs für verschiedene Sprachen. Für Java gibt es zwei große IDEs:

Eclipse und IntelliJ IDEA. Diese Installationserklärung wird sich auf die InteliJ Community Edition beziehen, da es die IDE ist, die ich empfehlen würde, zu Eclipse findet man aber auch mehr als genug Tutorials im Internet.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

## 2. Installation und Einrichtung

Den Download von IntelliJ IDEA Community Edition finden Sie unter

https://www.jetbrains.com/idea/download/#section=windows

hier:

![[Download.png]]

Laden Sie die Datei herunter, und führen Sie sie aus. Sie werden in ihrem Betriebssystem der Installation zustimmen müssen. 
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
Anschließend öffnet sich das Installationsfenster. Klicken Sie in diesem auf Next >

![[installer1.png]]

Nun können Sie den Installationsort auswählen. Falls Sie das gemacht haben, oder ihn nicht ändern wollen, gehen Sie wieder auf next >

![[installer2.png]]

Nun haben Sie verschiedene Optionen. Ich würde es empfehlen hierbei eine Assoziation mit .java Dateien zu erstellen, dies ist aber nicht nötig. Auch einen Desktopshortcut können Sie hier erstellen. Durch Add "Open Folder as Project" können Sie in Windows mit rechtsclick Ordner als IntelliJ Projekt in IntelliJ öffnen. Alle diese Dinge sind nicht nötig. Falls Sie sie trotzdem wollen, können Sie sie auswählen. Sie brauchen ihre PATH-Variablen nicht zu Updaten. Wählen Sie aus was Sie wollen, und klicken Sie dann auf next >

![[installer3.png]]

Nun können Sie eine Startmenüordner auswählen. Ich würde empfehlen, diesen beim Standard zu belassen. Klicken Sie auf Install, um die Installation zu starten.

![[installer4.png]]

Die Installation wird eine Weile brauchen. Klicken Sie anschließend Run IntelliJ IDEA Community Edition und dann auf finish.

![[installer5.png]]

Warten Sie, bis IntelliJ gestartet ist. Was Sie nun sehen, ist die Öffnungsseite von IntelliJ.

Wir werden nun ein Projekt erstellen. Klicken Sie auf New Project

![[IntelliJ CE 1.png]]

In dem jetzigen Fenster haben Sie eine Menge Optionen. Geben Sie bei Namen einen Namen für das Projekt ein. Der hier verwendete Name wird TestProjekt (Achtung auf die Groß- und Kleinschreibung!!!) sein. Entfernen Sie den Haken bei "Add sample code"!

Sie werden eine JDK spezifizieren müssen. Dabei handelt es sich um eine Datei, die Werkzeuge für das Programmieren von Java bereitstellt. Klicken Sie dafür auf JDK.

![[ProjektSetup1.png]]

Bei Ihnen werden vermutlich keinerlei JDK bereit liegen, bei mir sind bereits einige vorinstalliert. Wir werden so oder so nun die neueste JDK (aktuell Version 19) installieren. Klicken Sie dafür auf "Download JDK..."

![[JDKInstallation1.png]]

Das neue Fenster sollte wie folgt aussehen

![[JDK2.png]]

Falls dem so ist, gehen Sie auf Download

Nun öffnet sich ein Ladevorgang. Warten Sie, bis dieser abgeschlossen ist.

Die JDK sollte nun automatisch als JDK ausgewählt worden sein.

![[ProjektSetup2.png]]

Falls dem nicht so ist, wählen Sie sie einfach in dem JDK-Fenster aus.

Klicken Sie nun auf Create

Ich werde Ihnen nur einen kurzen Überblick über das allerwichtigste geben, vieles werden Sie im Laufe der Zeit kennen lernen.

Hier sehen Sie die Dateien ihres Projektes:

![[projektDateien.png]]

Hier ist die Konfiguration des Projektes, dazu später mehr.

![[config.png]]

Und hier sind einige wichtige Utility Tools, auch hierzu später mehr.

![[utility.png]]

Fahren Sie nun mit Abschnitt 3 fort.
<br />

---
_Autor: David Neumann_
_Kontakt für Fehler und Fragen: davidneumann2155@gmail.com_

# 3: Aufbau eines Java Programms

## Erste Schritte

Rechtsclicken Sie auf den Ordner namens „src“ bei den Dateien

![[src.png]]

gehen Sie ganz oben auf den Reiter New,

![[New.png]]

und wählen Sie dann „java class“ aus, um eine neue Datei zu erstellen.

![[java class.png]]

Was das genau ist, wird erneut später erklärt werden. Geben Sie in das Namensfeld einen Namen (am besten einfach "Main") ein.

![[Main.png]]

Diese Klasse wird ihre Hauptklasse, die auch die main-Methode enthalten wird (siehe unten). Erneut ergibt dies viel mehr Sinn, wenn man die späteren Konzepte versteht.

Im Hauptbereich sollte sich nun ein Fenster geöffnet haben, dies ist "ihr Programm" (Technisch gesehen handelt es sich hierbei um den Code der Hauptklasse ihres Programms, aber naja close enough IMO).

Ihr Programm sollte bisher so aussehen:

```java
public class Main {  
    ...  
}
```

Die geschwungenen Klammern beschreiben hierbei den Body der Klasse, alles, was darin steht, steht innerhalb der Klasse.

Nun werden wir die main-Methode implementieren.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
<br />

## main-Methode:

Die main-Methode ist der Teil des Programms, der beim Start des Programms einmal ausgeführt wird. Diese wird immer gleich konstruiert. Es empfiehlt sich ihren Aufbau auswendig zu lernen.

Erstellen Sie einen neuen Abschnitt (Enter) im inneren des Bereichs der geschwungen Klammern (Body), und schreiben Sie das folgende in den Body der Main-Klasse:

```java
public static void main(String[] args){  
    ...  
}
```

Bemerkungen:

1. IntelliJ vervollständigt automatisch einiges, z.B. klammern für Sie
2. Hierbei dienen die Einrückungen zum Behalten des Überblicks zum Body, in dem man sich befindet. IntelliJ nimmt Ihnen die Einrückarbeit größten Teils ab. Einrückungen können auch mit Tab erzeugt werden.

Ihr Code sollte nun wie folgt aussehen:

```java
public class Main {  
    public static void main(String[] args) {  
      ...  
    }  
}
```

Was diese Keywords genau bedeuten, wird später noch genauer erläutert werden.

Java Code wird normalerweise in mehre eigene Dateien aufgeteilt, dazu mehr bei Klassen

Die main-methode kommt innerhalb eines Projektes allerdings nur einmal vor, und stellt quasi das Herz des Programms da. Ihr Inhalt wird dabei durch die geschwungenen {} Klammern (ihren Body) begrenzt. Alles innerhalb dieser Klammern steht in der Methode, alles außerhalb steht außerhalb der Methode!

Außerhalb und innerhalb der main-methode können Variablen, Klassen, sowie weitere Methoden definiert werden. Dazu aber bei den einzelnen Bereichen mehr. Der Hauptunterschied ergibt sich hierbei durch das sog. Scoping (dazu mehr in Scoping)
<br />

## Libraries

Häufig benötigt man in java sog. Libraries. Das sind quasi Sammlungen, in denen von anderen Programmierern bereits Funktionalitäten umgesetzt wurden (zum Beispiel das Berechnen des Logarithmus oder so). Diese werden mit dem import Keyword in das Programm geladen. Aus Stilgründen werden imports immer ganz am Anfang des Programms geschrieben.

Bsp. (bitte nicht mitcoden):

```java
import Fisch;  
import xyz;  
  
  
public class Main{  
    public static void main(String[] args){  
      ...  
    }  
}
```

Dies sind die größten Dinge über den Aufbau von java-code, näheres wird dann in den einzelnen Kapiteln erklärt.

Als nächstes werden wir unser erstes Programm schreiben.
<br />

---

_Autor: David Neumann_
_Kontakt für Fehler und Fragen: davidneumann2155@gmail.com_

# 4: "Hello World" oder auch das erste Programm

Nun soll das erste Java-Programm geschrieben werden. Das Erste, was man eigentlich in jeder Programmiersprache macht, ist ein Programm zu schreiben, das "Hello World" ausgibt.

Dies werden Sie nun ebenfalls machen.

Ihr code sollte bislang wie folgt aussehen:

```java
public class Main{
	public static void main(String[] args){
		...
	}
}
```

Geben Sie nun in den Body der main-methode folgendes ein:

```java
System.out.println("Hello World");
```

Ein besonderer Hinweis hierbei auf das Semikolon am Ende des Befehls. Dieses dient in Java immer zur Signalisierung eines beendeten Teilschritts, und muss zwangsweise nach fast allen Dingen verwendet werden. (Nach jeder Deklaration oder Manipulation von Variablen, sowie nach Aufruf einer Methode)

Ihr code sollte nun wie folgt aussehen:

```java
public class Main{  
    public static void main(String[] args){  
        System.out.println("Hello World");  
    }
}
```

Nun führen wir das Projekt aus. 
Clicken sie dafür auf den grünen Pfeil neben der main-Methode
![[greenarrow.png]]

und anschließend auf Run 'Main.main()'
![[runmain.png]]

In Zukunft können Sie das Programm nun auch mit dem grünen Pfeil in der Oberen Rechten Ecke ausführen.

![[run.png]]

Es wird etwas brauchen, dann sollte ein Fenster im unteren Bereich aufpoppen, das wie folgt aussieht.

![[fenster.png]]

Im Folgenden wird dieser Teil als Konsole bezeichnet werden. Sie können sehen, dass darin Hello World geschrieben wurde.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
<br />

## Kommentare:

Um code übersichtlicher zu gestalten, ist es häufig sinnvoll, Kommentare zur Funktionalität von Dingen im Code selbst zu verfassen. Dies kann in Java auf zwei Arten erfolgen:

### 1: //

ein Kommentar mit zwei // Strichen blendet alles auf derselben Zeile rechts der Striche beim Ausführen aus, das heißt, hiermit kann man Bemerkungen zu einer Zeile schreiben

### 2: /\*Inhalt\*/

Will man mehrzeilige Kommentare verfassen, so kann man /\*...\*/ verwenden. Alles, was hierbei innerhalb der \*\* steht, wird beim ausführen des Programmes nicht beachtet.

Bsp.:

```java
public class Main{
	public static void main(String[] args){
		System.out.println("Hello World");
		// Kommentar
		}
	/*
	Mehrzeiliger
	Kommentar
	*/
}
```
<br />

---
_Autor: David Neumann_
_Kontakt für Fehler und Fragen: davidneumann2155@gmail.com_

# 5: Variablen und primitive Datentypen

Nun werden Variablen eingeführt. Eine Variable ist grundsätzlich ein wie eine Art Platzhalter, dem man einen Wert zuweisen, den Inhalt manipulieren, und von dem man den Wert auslesen kann. In unterschiedlichen Programmiersprachen werden Variablen unterschiedlich implementiert. In java sind Variablen grundsätzlich statisch typisiert. Das bedeutet, dass man einer Variable einen Datentyp zuweist, und diese Variable behält den Datentyp bei. Gängige Datentypen sind:

int (Integer): Ganzzahlen zwischen -2^31 und 2^31

float (floating point number): Kommazahlen (Aufbau ist etwas deutlich komplexer)

char (character): Buchstabe (aus der ASCII-Tabelle) wird angegeben durch das ' zeichen vor und nach dem Buchstaben ('c'/ '1'/ '%' etc. )

boolean: Wahrheitsvariable, die entweder Wahr oder Falsch ist.

Darüber hinaus gibt es noch ein paar weitere sog. primitive Datentypen, diese erwähne ich jedoch aufgrund ihrer geringen Relevanz nicht näher, eine Beschreibung finden Sie im Anhang.

Es gibt zwei wichtige Schritte beim Erstellen einer Variable. Die Deklarierung, und die Initialisierung:

Bei der Deklarierung werden Datentyp und Scope (siehe Scoping) der Variable festgelegt.

Diese folgt dem Schema:

```java
// Schema
datentyp variablenName;
```

Nomenklatur:

Variablen folgen in Java dem camelCase Style, das heißt, sie beginnen kleingeschrieben, und jedes neue Wort wird großgeschrieben. Der ganze Name muss zusammenhängend sein. Der Anfang darf keine Zahl sein

Bsp.:

```java
float spielerDurchschnitt;

int größterGemeinsamerTeiler;

int xDividiertDurch2;
```

Erweitern Sie ihren Code wie im Beispiel unten um den integer x, den character c, und den boolean bool. Tun Sie dies innerhalb des Bodies der main-methode, vor der Ausgabesystematik (System.out.println("Hello World"))!

```java
public class Main{	
	public static void main(String[] args){
		int x;
		char c;
		boolean bool;
		System.out.println("Hello World");
	}	
}
```

Um eine Variable zu verwenden, muss sie zusätzlich initialisiert werden, das heißt, ihr wird ein Startwert zugewiesen. Dies wird mit dem = Operator gemacht, nachdem die Variable deklariert, wurde:

```java
datentyp variable;

variable = wert;
```

Bsp.:

```java
int x;
x = 0; 
```

Deklarierung und Initialisierung können auch in einem Schritt stattfinden:

```java
datentyp variable = Wert;
```

Bsp.:

```java
int x = 0;
```

Hinweis: Aufgrund des Aufbaus von java müssen variablen, die außerhalb von Methoden initialisiert werden sollen, direkt bei der Deklaration initialisiert werden.

initialisieren Sie nun x mit 4, char mit 'd', und bool mit false. Achten Sie darauf, dies direkt bei der Deklaration zu machen. Ihr code sollte nun so aussehen:

```java
public class Main{  
    public static void main(String[] args){  
        int x = 4;  
        char c = 'd';  
        boolean bool = false;  
        System.out.println("Hello World");  
    }
}
```
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
<br />

## Manipulation von Variablen

Das interessante an Variablen ist, das man Sie nicht nur festlegen, sondern auch manipulieren und auslesen kann. Um dies zu verdeutlichen, ersetzen Sie den Inhalt der main-Methode mit folgendem Code:

```java
int x = 4;  
char c = 'd';  
boolean bool = false;  
System.out.println(bool);  
System.out.println(c);  
System.out.println(x);  
x = x+2;  
System.out.println(x);
```

Ihr code sollte nun so aussehen:

```java
public class Main {  
    public static void main(String[] args) {  
        int x = 4;  
        char c = 'c';  
        boolean bool = false;  
        System.out.println(bool);  
        System.out.println(c);  
        System.out.println(x);  
        x = x + 2;  
        System.out.println(x);  
    }
}
```

Führen Sie den Code aus, und betrachten Sie das Ergebnis.

Wie Sie sehen können, wurde einmal 4 und einmal 6 ausgegeben.

Dies kam durch die Operation x = x + 2 zustande. Diese ist nicht wie in der Mathematik als Gleichung, sondern vielmehr als logischer Ablauf zu lesen:

1. x = y <> setze die Variable links auf den Wert rechts.
2. x + 2 <> berechne x + 2

Logisch geschieht hierbei folgendes:

1. x = x + 2 interpretiert als x = y also setze x auf y
2. y = x + 2 (setze y auf x + 2)
3. x wird ausgelesen
4. der ausgelesene Wert von x wird um 2 erhöht
5. das Ergebnis, das y wäre wird in x eingespeichert.

Wichtig hierbei: Mathematische Operationen beachten Operationspriorität (also Klammern vor Punkt vor Strich)

Für verschiedene Datentypen gibt es verschiedene Operationen, die man mit der Zeit lernt und deshalb hier nicht genauer aufgeführt werden. Was ich nun noch aufzählen werde, sind die wichtigsten Operationen für variablen.

"+=" bzw. "-=" und "\*=" bzw. "/=":

Wie bereits gezeigt, kann man auf eine integer Variable mittels

```java
x = x + 2
```

eine Zahl addieren. Genau so geht das auch mit der Multiplikation, hierfür verwendet man einen Stern \*:

```java
x = x * 2
```

Analog dient "-" für Subtraktion und "/" für Division.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
Da diese Schreibweise jedoch recht umständlich ist, wenn man x einfach nur um eine Zahl verändern möchte, bietet java noch ein paar einfachere Schreibweisen:

```java
//Addition
x = x + 2;
//äquivalent zu
x += 2;

//Subtraktion
x = x - 2;
//äquivalent zu
x -= 2;

//Multiplikation
x = x * 2;
//äquivalent zu
x *= 2;

//Division
x = x / 2;
//äquivalent zu
x /= 2;

//Sonderfall
x = x + 1;
//äquivalent zu
x++;

//Sonderfall
x = x - 1;
//äquivalent zu
x--;

```
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
Aufgabe 1:

Was speichern die folgenden Datentypen:

int

char

float

boolean

Lösung:

siehe unten L1

Aufgabe 2:

Erweitern Sie ihren Code um die Variable y. Diese soll Ganzzahlen halten und auf 5 starten.

Lösung:
siehe unten L2

Aufgabe 3:

Geben Sie y in die Konsole aus, multiplizieren Sie anschließend y mit 3 und geben Sie y wieder in die Konsole aus.

Lösung:
siehe unten L3
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
<br />

## Interaktion von Variablen:

Variablen können auch miteinander Kombiniert werden.

Bsp.:

```java
public class Main{  
    public static void main(String[] args){  
        int x = 3;  
        int y = 7;  
        System.out.println(x); // 3  
        System.out.println(y); // 7  
        x = x + y; // x = 3 + 7 = 10  
        y += x; // y = 10 + 7 = 17  
        System.out.println(x); // 10  
        System.out.println(y); // 17  
    }  
}
```

Dies fasst zum größten Teil zusammen, was es über Variablen zu sagen gibt, es wird später aber noch auf das Scoping von Variablen eingegangen werden.

Lösungen:

L1:

int: ganzzahlen

char: buchstaben

float: kommazahlen

boolean: Wahr oder Falsch
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
L2:

```java
public class Main {  
    public static void main(String[] args){  
        int x = 4;  
        char c = 'c';  
        boolean bool = false;  
        int y = 5;  
        System.out.println(x);  
        x = x + 2;  
        System.out.println(x);  
    }
}
```

L3:

```java
public class Main {  
    public static void main(String[] args){  
        int x = 4;  
        char c = 'c';  
        boolean bool = false;  
        int y = 5;  
        System.out.println(y);  
        System.out.println(x);  
        x = x + 2; // alternativ auch x += 2
        y = y * 3; // alternativ auch y *= 3*  
        System.out.println(x);  
        System.out.println(y);  
    }
}
```
<br />

---
_Autor: David Neumann_
_Kontakt für Fehler und Fragen: davidneumann2155@gmail.com_

# 6: if und else-statements, Vergleichsoperatoren

Um Logische Abläufe modellieren zu können ist es notwendig, if- und else-statements sowie Vergleichsoperatoren zu behandeln.

## if-statement:

ein if-statement stellt eine Art Schalter da. Der Aufbau sieht wie folgt aus:

```java
if(Statement){
	...
}
```

Der Code innerhalb des Bodies({}-Klammern) der if-Methode wird nur dann ausgeführt, wenn Statement true ist, also wenn die Aussage davon erfüllt ist. Um logische Abfragen damit zu machen, gibt es die sog. Vergleichsoperatoren. Es werden hier nur die Essenziellen Vergleichsoperatoren vorgestellt, weitere entnehmen Sie bitte dem Anhang.

## Gleichheitsoperator:

== oder auch Gleichheitsoperator genannt ergibt wahr, wenn links und rechts von dem Operator Gleiche Ergebnisse stehen.

Bsp.:

```java
int x = 4;
int y = 3;
int z = 4;
char a = '4';

4 == 4; // true
4 == 3; // false
x == 4; // true
x == y; // true
x == z; //false
x == a; //false
```

Wichtig hierbei anzumerken, ist das Typen beim Vergleichen mit dem Vergleichsoperator auch immer verglichen werden, also gibt x == a immer falsch zurück, egal welche Werte x und a haben, da ihre Typen unterschiedlich sind.

## Relationsoperatoren:

Die Relationsoperatoren < und > sowie <= und >= vergleichen die Größenrelationen von Zahlen. (Hinweis: hiermit können auch float und int verglichen werden)

Bsp.:

```java
int x = 3;
int y = 4;
int z = 4;
float f = 2;

x < y; // true
x > y; // false
x < z; // false
x <= z; //true
x > f; //true
```
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
<br />

## else-statement:

häufig soll in einem Programm entweder eine Sache oder eine andere Sache ausgeführt werden. Um dies zu erhalten wäre es ungünstig zwei if Statements zu schreiben, da dies zwei Mal die Vergleichsoperation abfragen würde. Deshalb gibt es das else-statement. Dieses wird immer dann aufgerufen, wenn das vorhergehende if-statement NICHT ausgeführt wurde.

Struktur:

```java
if(Statement){
	...
} else{
	...
}
```

Bsp.:

```java
int x = 2; //Immer wieder veränderbar
if (x > 0){
	x--;
} else{
	x++;
}
```

Hierbei wird x um 1 reduziert, wenn es größer als Null ist, und um 1 erhöht, wenn es kleiner-gleich Null ist.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
<br />

## else if

Häufig gibt es mehrere logische Verkettungen von if- und else-statements. auf ein if-statement kann auch ein else if-statement folgen.

Syntax:

```java
if(Statement){
	...
}else if(Statement){
	...
} else if(Statement){
	...
}usw...
```

Hierauf kann auch am Ende noch ein else-statement folgen, dieses muss aber aufgrund des logischen Abschlusses immer ganz am Ende kommen.

## oneliner:

Häufig muss man nach einem if-statement nur eine einzige Operation ausführen. Um sich Arbeit zu sparen, existiert hierfür eine Kurzform:

```java
if(Statement)...;
```

Bsp.:

```java
int x = 2;
if(x > 0)x++;
else x--;
```

Wie man sehen kann, kann eine Operation auch ohne die Klammern des sonst üblichen Bodies durchgeführt werden.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
<br />

## Zusatz!!

Durch Verständnis der oneliner ergibt sich auch der logische Sinn von else-if-statements.

Man könnte den Ablauf auch so ausdrücken:

```java
if(Statement)...;
else{
	if(Statement)...;
	else{
		if(Statement)...;
		else{
			...
		}
	}
}
```

Wie man sehen kann, ist dieser Aufbau aber deutlich aufwendiger.
<br />

---
_Autor: David Neumann_
_Kontakt für Fehler und Fragen: davidneumann2155@gmail.com_

# Exkurs: 6.1: Switches

Zitat Wurst (Informatikstudent aus Karlsruhe) "Das Ding mit Switches in java ist, da java ja auch BDSM ist, switches sind switch"

Switches sind eine Methode zur Simplifikation von langen if-else-if-...-logikketten.

Darüber hinaus bieten sie zumindest in java einen Performance Vorteil gegenüber herkömmlichen if-else-if-ketten.

Syntax:

```java
variable x = Wert;
switch(x){
	case a:
		...
		break;
	case b:
		...
		break;
	case c:
		...
		break;
	...
}
```
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

Bsp.:

```java
int x = 1;  
switch(x) {  
    case 1:  
        x++;  
        break;  
    case 2:  
        x--;  
        break;  
    case 0:  
        x += 3;  
        break;  
    case 3:  
        x *= 2;  
        break;  
}
```

WICHTIGE HINWEISE:

Am Ende von jedem Case muss ein break-Keyword eingebaut werden.

In einem Switch müssen alle Fälle finale Werte sein, also entweder Werte im Code selbst oder Variablen, die durch final Festgelegt wurden. Dies hat den Hintergrund, dass es den Code viel effizienter macht.
<br />

---
_Autor: David Neumann_
_Kontakt für Fehler und Fragen: davidneumann2155@gmail.com_


# 7: for und while schleifen

Häufig möchte man beim Programmieren Dinge mehrfach durchführen.

Bsp.:

```java
public class Main{  
    public static void main(String[] args){  
        int x = 0;  
        system.out.println(x);  
        x++;  
        system.out.println(x);  
        x++;  
        system.out.println(x);  
        x++;  
        system.out.println(x);  
        x++;a  
        system.out.println(x);  
        x++;  
        system.out.println(x);  
        x++;  
        ...  
    }  
}
```

Dies jedoch durch copy und paste durchzuführen, birgt eine riesige Gefahr:

Sobald das kopierte Segment einen Fehler enthält, sind direkt alle Kopien davon auch fehlerhaft. Darüber hinaus ist es auch einiges an Arbeit, und unübersichtlich. 
In diesem Beispiel ist zum Beispiel System klein statt großgeschrieben. Außerdem hat sich ein a eingeschlichen.

Deshalb bietet java sog. Schleifen. Diese wiederholen Code, bis ihr exit-requirement erfüllt ist.

Diese werden nun vorgestellt.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
<br />

## for-schleifen:

for-schleifen bieten meist die Praktikabelste Möglichkeit zum Iterieren(wiederholen) von Code.

Ihre Syntax ist wie folgt:

```java
for(variable x = Anfangswert; exit-statement; Operation auf x){
    ...
}
```

Bsp.:

Der Code von oben, nur als Schleife

```java
public class Main{  
    public static void main(String[] args){  
        for(int x = 0; x <= 4; x++){  
            System.out.println(x);  
        }
    }
}
```

x wird hierbei die Zählervariable oder auch Iterationsvariable genannt.  Das exit-statement, ist das Statement, was false, also falsch sein muss, damit die Schleife beendet wird. Hier ist dies erfüllt, wenn x echt-größer als 5 ist.

Die Operation auf x ist eine beliebige Operation auf x, die am Ende jeder Iteration also jeden Durchlaufs der for-schleife durchgeführt wird. In diesem Fall heißt das, dass x nach jeder Iteration um 1 erhöht wird.

Kehren wir zu unserem Codeprojekt zurück:

Löschen Sie den gesamten Inhalt des Bodies der main-methode.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
Ihr Code sollte nun wieder so aussehen:

```java
public class Main{
	public static void main(String[] args){
	
	}
}
```

Fügen Sie nun die for-loop von oben ein. Ihr code sollte nun so aussehen:

```java
public class Main{
	public static void main(String[] args){
		for(int x = 0; x <= 4; x++){
			System.out.println(x);
		}
	}
}
```

Führen Sie ihren Code aus.

Betrachten Sie, was sie sehen.

Aufgabe 1:

Ändern Sie die Schleife, um die Zahlen bis 10 auszugeben.

Lösung:
siehe unten L1


Aufgabe 2:

Erstellen Sie eine weitere Schleife, die die ersten 5 ungeraden Zahlen (1, 3, 5, 7, 9) ausgibt.

pot. Lösungen:
siehe L2
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

## while-schleifen.

While schleifen sind ähnlich zu for-schleifen, bedürfen aber nicht der gleichen Strenge bei der Konstruktion.

Syntax:

```java
while(statement){
	...
}
```

Der Inhalt der Schleife wird wiederholt, solange das Statement nicht false wird.

for und while schleifen lassen sich fast immer ineinander übersetzen.

Bsp.: Die for-schleife von oben in eine while-schleife translatiert

```java
public class Main{  
    public static void main(String[] args){  
        int x = 0;  
        while(x <= 4){  
            System.out.println(x);  
            x++;  
        }
    }
}
```

Wie Sie sehen können, sind while-schleifen vom Ablauf ähnlich zu for-schleifen, bieten aber den Raum, die Variable zum Beispiel am Anfang statt am Ende zu verändern.

Beide Schleifentypen haben vor und Nachteile, und eignen sich für unterschiedliche Probleme besser und schlechter.

Am Ende ist es auch sehr eine Frage der Übung.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

## while(true) und break;

wie Sie vielleicht schon bemerkt haben, muss eine while-schleife (übrigens auch eine for-schleife) nicht immer ihre exit-requirement erreichen. Das Wohl einfachste Beispiel hierfür stellt:

```java
while(true){
	...
}
```

da. In diesem Beispiel ist das Statement in der while-schleife (obviously) immer true, also wird diese Schleife sich unendlich wiederholen.  Dies kann auch als Funktionalität verwendet werden:

Bsp.:

Möchte man (warum auch immer der arme PC) zum Beispiel ein Programm schreiben, dass alle natürlichen Zahlen der Reihe nach aufzählt, kann man dafür den folgenden Code schreiben.

```java
public class Main{  
    public static void main(String[] args){  
        int x = 0;  
        while(true){  
            System.out.println(x);  
            x++;  
        }
    }
}
```

Möchte man vorzeitig, eine Schleife verlassen, existiert dafür das break-statement.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
Bsp.:

Wieder unsre for-schleife von oben, anders modelliert:

```java
public class Main{  
    public static void main(String[] args){  
        int x = 0;  
        while(true){  
            System.out.println(x);  
            x++;  
            if(x >= 5){  
                break;  
            }
        }
    }
}
```

Bemerkung:

Java verwendet einen Compiler, um Code effizienter zu machen. IntelliJ zeigt Ihnen Änderungen durch den Compiler an, und schlägt ihnen Verbesserungen for. Deshalb wird das exit-statement der while-schleife hier von IntelliJ kritisiert werden.

### Lösungen (weitere Lösungen sind natürlich auch möglich):

L1:
```java
public class Main{  
    public static void main(String[] args){  
        for(int x = 0; x <= 10; x++){  
            System.out.println(x);  
        }
    }
}
```
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

L2:

1.
```java
public class Main{  
    public static void main(String[] args){  
        for(int x = 1; x < 10; x += 2){  
            System.out.println(x);  
        }
    }
}
```

2.
```java
public class Main{  
    public static void main(String[] args){  
        for(int x = 0; x <= 4; x ++){  
            System.out.println(2 * x + 1);  
        }
    }
}
```
<br />

---
_Autor: David Neumann_
_Kontakt für Fehler und Fragen: davidneumann2155@gmail.com_
# 8: Methoden

## EINSCHUB!

Ab hier verkompliziert der Aufbau von java uns den Vorgang leider etwas. Deshalb werden wir einen kleinen Trick verwenden, um uns vieles leichter zu machen. (also eigentlich zu verhindern, dass wir zu viele zu komplexe Themen unbehandelt verwenden müssen)

Ersetzen Sie ihren bisherigen Code durch folgendes (Sie dürfen copy-pasta machen):

```java
  
public class Main {  
    static CodeTeil code = new CodeTeil();  
    
    public static void main(String[] args) {  
        code.main(); // das hier alles noch ignorieren  
    }
}  


class CodeTeil{  
    CodeTeil(){} // Das bitte ignorieren  
    
    // ab hier wieder coden  
    public void main(){
	    
    }  
}
```

Wir werden ab sofort in der main-methode der CodeTeil Klasse weitercoden, d.h. diese ist ab sofort mit der main-methode gemeint. Der ganze obere Teil kann ab sofort ignoriert werden, und wird nicht mehr in Beispiele eingebracht werden (bis wir später über Klassen gesprochen haben). Auch den ersten Abschnitt innerhalb der CodeTeil Klasse ignorieren Sie bitte vorerst.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
<br />

## Motivation

Wie wir bereits gesehen haben, ist es sehr ungünstig, code mehrfach zu verwenden.

Will man trotzdem komplexere Codesegmente mehrfach verwenden, empfiehlt sich die Nutzung von Methoden.

Bsp.:

In die Konsole soll zu unterschiedlichen Zeiten das Quadrat der Variable x ausgegeben werden.

Schlechte Implementation

```java
public class CodeTeil{  
    CodeTeil(){} // Das bitte Ignorieren  
    
    // ab hier coden  
    public void main(){  
        int x = 0;  
        System.out.printl(x + x);  
        x += 5;  
        System.out.printl(x + x);  
        for(int y = 0; y < 4; y++){  
            x++;  
            System.out.printl(x + x);c  
        }  
        x = -4;  
        System.out.printl(x + x);  
    }
}
```

Im Beispiel wurde aus Versehen x + x, statt x \* x verwendet. Außerdem hat sich diesmal ein c eingeschlichen.

Stattdessen bietet sich die Implementierung einer Methode printSquareOfX() an.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
Aber zunächst:
Die Syntax von Methoden:

```java
rückgabewert methodenName(*Parameter){
	...
}
```

rückgabewert stellt hierbei den Datentyp des Rückgabewerts der Methode dar, hierzu mehr bei Rückgabewerte, wir werden erstmal nur void, also keinen Rückgabewert verwenden.

Parameter werden im nächsten Abschnitt behandelt werden.

Der Inhalt des Bodies der Methode stellt den Code da, der beim Aufrufen der Methode ausgeführt werden soll.

Nomenklatur:

Die Namen von Methoden werden wie die Namen von Variablen im camelCase Style gebildet (siehe 5.)

Zurück zu unserem Beispiel:

Eine Methode zum Ausgeben des Quadrates von x könnte zum Beispiel so aussehen:

```java
void printSquareOfX(){
	System.out.println(x * x);
}
```
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
Implementiert in unseren code sähe das ganze wie folgt aus:

```java
class CodeTeil{  
    CodeTeil(){} // Das bitte ignorieren  
  
    // ab hier wieder coden       
    public int x = 0; 
     
    public void main(){  
        System.out.printl(x + x);  
        x += 5;  
        System.out.printl(x + x);  
        for(int y = 0; y < 4; y++){  
            x++;  
            System.out.printl(x + x);}  
        x = -4;  
        System.out.printl(x + x);  
    }
    
    void printSquareOfX(){  
	    System.out.println(x * x);  
    }
}
```

Hinweise:

1. main() ist eine Methode.

2. Methoden müssen immer außerhalb von Methoden definiert werden.

3. da printSquareOfX x als variable verwendet, muss x nun außerhalb der main-methode deklariert werden. Mehr dazu bei Scoping

Bislang macht unsere Methode nichts.

Um eine Methode auszuführen, muss man sie aufrufen.

Dies geschieht, indem man den Methodennamen mit () hinten dran schreibt.

In unserem Beispiel würden wir also alle aufrufe von System.out.printl(x + x); durch printSquareOfX() ersetzen.

Hinweis, Autocompletion:

IntelliJ schlägt Ihnen vermutlich wenn Sie anfangen printSquareOfX() zu schreiben, bereits diese Methode vor. In dem Sie Tab drücken, können Sie das Autocompletion feature von IntelliJ nutzen, um sich Zeit zu sparen!

Unser Code sieht dann wie folgt aus:

```java
class CodeTeil{  
    CodeTeil(){} // Das bitte ignorieren  
    
    // ab hier wieder coden
    public int x = 0;  
	public void main(){  
        printSquareOfX();  
        x += 5;  
        printSquareOfX();  
        for(int y = 0; y < 4; y++){  
            x++;  
            printSquareOfX();  
        }        x = -4;  
        printSquareOfX();  
    }  
    
    void printSquareOfX(){
        System.out.println(x * x);  
    }
}
```

Nun werden wir uns Parameter für Methoden ansehen.
<br />

---
_Autor: David Neumann_
_Kontakt für Fehler und Fragen: davidneumann2155@gmail.com_
# 8.1: Parameter

Eines der größten Probleme unserer bisherigen Implementation der Methode zum Ausdrucken des Quadrats unserer Variable ist der, dass dies nur mit der Variable x funktioniert. Würden wir zum Beispiel noch eine Variable y deklarieren, müssten wir für sie eine ganz neue Methode schreiben.

Außerdem könnte eine Variable, die innerhalb der main-methode deklariert wurde gar nicht verwendet werden.

Eine Lösung hierfür stellen Parameter da. Diese erlauben es uns einen Wert in die Methode zu übergeben, denn wir dann darin verwenden. Ein Parameter ist eine Variable, die beim Aufrufen der Methode erzeugt wird. Parameter werden beim Definieren der Methode als variablen innerhalb der () klammern deklariert, und durch „,“-kommas getrennt.

Syntax:

```java
rückgabewert methodenName(datentyp Parameter1, datentyp Parameter2, ...){
	...
}
```

in unserem Beispiel ließe sich unsere Methode wie folgt verallgemeinern:

```java
void printSquareOfNumber(int number){
	System.out.print(number * number);
}
```

Hinweis: Refractoring:

IntelliJ bietet Möglichkeiten zum refractorn von Code, also zum Umstrukturieren. Eine der simpelsten Beispiele hiervon ist das Umbenennen von Methoden oder Variablen. Durch das Nutzen des Refractoring Features werden gleichzeitig die Methode und alle ihre Aufrufe umbenannt. Zum Benutzen klicken Sie gleichzeitig SHIFT und F6 während Sie die Methode ausgewählt haben, geben Sie den neuen Namen ein, und drücken Sie dann Enter
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
im Code implementiert wäre das:

```java
class CodeTeil{  
    CodeTeil(){} // Das bitte ignorieren  
    
    // ab hier wieder coden
    public int x = 0;  
    
    public void main(){  
        printSquareOfNumber();  
        x += 5;  
        printSquareOfNumber();  
        for(int y = 0; y < 4; y++){  
            x++;  
            printSquareOfNumber();  
        }        x = -4;  
        printSquareOfNumber();  
    }
    
    void printSquareOfNumber(int number) {  
        System.out.println(number * number);  
    }
}
```

Wie Sie vielleicht sehen, unterstreicht IntelliJ nun alle Aufrufe von printSquareOfNumber. Dies liegt daran, dass diese Methode nun bei jedem Aufruf eine Eingabe erwartet. Dies geschieht, in dem man einen Wert (beziehungsweise den Inhalt einer Variable) des passenden Datentyps in die Klammern beim Aufrufen der Methode schreibt. Man sagt, man übergibt den Wert in den Parameter der Methode.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
In unserem Beispiel würde das wie folgt aussehen:

```java
class CodeTeil{  
    CodeTeil(){} // Das bitte ignorieren  
    
    // ab hier wieder coden  
    public void main(){  
        int x = 0;  
        printSquareOfNumber(x);  
        x += 5;  
        printSquareOfNumber(x);  
        for(int y = 0; y < 4; y++){  
            x++;  
            printSquareOfNumber(x);  
        }        x = -4;  
        printSquareOfNumber(x);  
    }
    
    void printSquareOfNumber(int number){  
        System.out.println(number * number);  
    }
}
```

Hinweis: da wir x nur noch übergeben, können wir es wieder in die main-methode verschieben.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
Nun können wir beispielsweise auch die Iterationsvariable y aus der for-schleife in unsere Methode übergeben.

```java
class CodeTeil{  
    CodeTeil(){} // Das bitte ignorieren  
  
    //ab hier wieder coden
    public void main(){  
        int x = 0;  
        printSquareOfNumber(x);  
        x += 5;  
        printSquareOfNumber(x);  
        for(int y = 0; y < 4; y++){  
            x++;  
            printSquareOfNumber(x);  
            printSquareOfNumber(y);  
        }        x = -4;  
        printSquareOfNumber(x);  
    }
    
    void printSquareOfNumber(int number){  
        System.out.println(number * number);  
    }
}
```
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

### java-interne Methoden:

java bietet von sich aus einige Methoden an. So ist zum Beispiel auch System.out.println eine (überladene, mehr hierzu bei Überladung) Methode. Um dies etwas zu verdeutlichen, schreiben wir uns eine eigene print-methode, und verwenden diese in printSquareOfNumber (ja Methoden können auch Methodenaufrufe enthalten) statt System.out.prinln

```java
class CodeTeil{  
    CodeTeil(){} // Das bitte ignorieren  
    
    // ab hier wieder coden  
    public void main(){  
        int x = 0;  
        printSquareOfNumber(x);  
        x += 5;  
        printSquareOfNumber(x);  
        for(int y = 0; y < 4; y++){  
            x++;  
            printSquareOfNumber(x);  
        }        x = -4;  
        printSquareOfNumber(x);  
    }
    
    void printSquareOfNumber(int number){  
        print(number);  
    }
    
    void print(int number){  
        System.out.println(number);  
    }
}
```

Die Funktionalität bleibt hierbei genau die gleiche.
<br />

---
_Autor: David Neumann_
_Kontakt für Fehler und Fragen: davidneumann2155@gmail.com_
# 8.2: Rückgabewerte

Dieses Kapitel ist wohl eines der wichtigsten Kapitel beim Lernen von Programmiersprachen. Ein tieferes Verständnis für Rückgabewerte von Methoden liefert eine große Einsicht in die Funktionalität der meisten Programmiersprachen (auch wenn das auf dem Elementaren Level meistens nochmal etwas komplizierter wird.)

Bisher haben unsere Methoden nur Werte entgegengenommen, aber nichts zurückgegeben. Dies wird sich nun ändern.

Dafür werden wir die bisherige Funktionalität unserer printSquareOfNumber-methode aufspalten, in eine Methode, die uns das Quadrat einer Zahl berechnet, und eine Methode, die uns eine Zahl ausdruckt (bzw. dies haben wir bereits).

Dafür werden wir die Methode square(int number) implementieren.

Diese soll einen integer zurückgeben. Java weist Methoden stets einen festen Rückgabewert zu. Diesen schreibt man beim Definieren der Methode ganz an den Anfang. Bisher war unser Rückgabewert stets void, d.h. unsere Methode hat nichts zurückgegeben.
Man gibt einen Wert mithilfe des Keywords return zurück.

Unsere neue Methode sähe dann so aus:

```java
int square(number){
	int x = number * number;
	return x;
}
```

bzw. noch simpler:

```java
int square(number){
	return number * number;
}
```

(vom Ablauf her wird zunächst das Produkt aus number mit number berechnet, und dieses dann zurückgegeben)
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

In unseren code implementiert sähe das in etwa so aus:

```java
class CodeTeil{  
    CodeTeil(){} // Das bitte ignorieren  
  
    // ab hier wieder coden
    public void main(){  
        int x = 0;  
        printSquareOfNumber(x);  
        x += 5;  
        printSquareOfNumber(x);  
        for(int y = 0; y < 4; y++){  
            x++;  
            printSquareOfNumber(x);  
        }        x = -4;  
        printSquareOfNumber(x);  
    }
    
    void printSquareOfNumber(int number){  
        int squareNumber = square(number);  
        print(squareNumber);  
    }
    
    void print(int number){  
        System.out.println(number);  
    }
    
    int square(int number){  
        return number * number;  
    }
}
```

Wichtige Hinweise:

1. Der Rückgabewert von square muss verarbeitet werden. In unserem Beispiel tun wir dies, indem wir ihn in eine Variable einspeichern.
2. Der Code kann simpler gestaltet werden. Man kann den Rückgabewert einer Methode auch direkt(also ohne ihn in eine Variable zwischen zu speichern) in eine weitere Methode übergeben. Dies würde in unserem Beispiel dann so aussehen:


```java
class CodeTeil{  
    CodeTeil(){} // Das bitte ignorieren  
    
    // ab hier wieder coden
    public void main(){  
        int x = 0;  
        printSquareOfNumber(x);  
        x += 5;  
        printSquareOfNumber(x);  
        for(int y = 0; y < 4; y++){  
            x++;  
            printSquareOfNumber(x);  
        }        x = -4;  
        printSquareOfNumber(x);  
    }
    
    void printSquareOfNumber(int number){  
        print(square(number));  
    }
    
    void print(int number){  
        System.out.println(number);  
    }
    
    int square(int number){  
        return number * number;  
    }
}
```

Vom Ablauf her würde zunächst number in square übergeben werden, dort würde dann das Quadrat von number zurückgegeben werden und dieses würde dann direkt in print() übergeben werden.

---
_Autor: David Neumann_
_Kontakt für Fehler und Fragen: davidneumann2155@gmail.com_
# 8.3: Überladung

Java erlaubt das Überladen von Methoden. D.h. es ist in java möglich mehrere Methoden mit gleichem Namen, aber unterschiedlichen Parametern zu haben. Ein simples Beispiel hierfür stellt unsere print-Methode da. Diese Funktioniert nur, falls die Eingabe ein Objekt des Datentyps int ist. Möchte man z.B. statt einem int einen character Drucken, kann man dafür durch Überladung eine neue print-Methode erstellen:
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

```java
class CodeTeil{  
    CodeTeil(){} // Das bitte ignorieren  
    
    // ab hier wieder coden
    public void main(){  
        int x = 0;  
        printSquareOfNumber(x);  
        x += 5;  
        printSquareOfNumber(x);  
        for(int y = 0; y < 4; y++){  
            x++;  
            printSquareOfNumber(x);  
        }        
        x = -4;  
        printSquareOfNumber(x);  
    }
    
    void printSquareOfNumber(int number){  
        print(square(number));  
    }
    
    void print(int number){  
        System.out.println(number);  
    }
    
    int square(int number){  
        return number * number;  
    }
        
	void print(float number){  
	    System.out.print(number);  
	}
}
```

Bei einer überladenen Methode wird die Methode anhand der Eingabe beim Aufrufen ausgewählt.

---
_Autor: David Neumann_
_Kontakt für Fehler und Fragen: davidneumann2155@gmail.com_
# 9: Scoping
Eines der wichtigsten Konzepte für sauberes Programmieren stellt das sog. Scoping da. Dabei geht es um den Bereich, in dem eine Variable (oder Methode, aber das ist eher nebensächlich) definiert ist. 
Grundsätzlich gilt: Eine Variable ist immer nur innerhalb des Bodies definiert, in dem sie deklariert wurde. Leeren Sie den gesamten Inhalt (bis auf das was Sie ignorieren sollen) der CodeTeil Klasse. 

Ihre CodeTeil Klasse sollte jetzt wieder so aussehen:
```java
class CodeTeil{
	CodeTeil(){} // Das bitte ignorieren
	
	//ab hier wieder coden
}
```

Fügen Sie nun wieder eine public main-Methode (keine Rückgabe) und außerdem zwei Methoden int plusX(int n) und int plusY(int n) hinzu. Ihr code sollte nun so aussehen:

```java
class CodeTeil{
	CodeTeil(){} // Das bitte ignorieren
	
	// ab hier wieder coden
	public void main(){
		
	}
	
	int plusX(int n){
		
	}
	
	int plusY(int n){
		
	}
}
```
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
Nun erstellen wir zwei Variablen int x = 0 und int y = 1, int x hierbei außerhalb des Bodies der main-Methode und int y innerhalb diesen:

```java
class CodeTeil{
	CodeTeil(){} // Das bitte ignorieren
	
	// ab hier wieder coden
	int x = 0;
	public void main(){
		int y = 1;
	}
	
	int plusX(int n){
		
	}
	
	int plusY(int n){
		
	}
}
```

Nun geben wir plusX und plusY Funktionalität. plusX soll n + x zurückgeben, und plusY n + y

```java
class CodeTeil{
	CodeTeil(){} // Das bitte ignorieren
	
	// ab hier wieder coden
	int x = 0;
	public void main(){
		int y = 1;
	}
	
	int plusX(int n){
		return n + x;
	}
	
	int plusY(int n){
		return n + y;
	}
}
```

Wie Sie sehen können, zeigt Ihnen IntelliJ hierbei bei plusY einen Fehler an. Dies liegt daran, dass y nur innerhalb der main-Methode definiert ist (man sagt auch im Scope der main-Methode), und somit für plusY nicht existiert. 

## Shadowing
Scoping erlaubt auch eine weitere Mechanik, dass sog. Shadowing von Variablen. Das bedeutet, dass in java mehrere Variablen mit gleichen Namen in verschiedenen Scopes definiert werden können. Hierbei überschreibt eine Variable des inneren Scopes eine des äußeren Scopes. Ein Beispiel hierfür könnte in unserem Beispiel wie folgt aussehen.

```java
class CodeTeil{
	CodeTeil(){} // Das bitte ignorieren
	
	// ab hier wieder coden
	int x = 0;
	int y = 2;
	public void main(){
		int y = 1;
	}
	
	int plusX(int n){
		return n + x;
	}
	
	int plusY(int n){
		return n + y;
	}
}
```

Hierbei würde y in plusY nun 2 sein, innerhalb von main aber 1, da hier das innere y als variable gilt.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div> 
Dies kann man sehen, indem man plusY mit y in main aufruft und anschließend ausgibt:

```java
class CodeTeil{
	CodeTeil(){} // Das bitte ignorieren
	
	// ab hier wieder coden
	int x = 0;
	int y = 2;
	public void main(){
		int y = 1;
		System.out.println(plusY(y));
	}
	
	int plusX(int n){
		return n + x;
	}
	
	int plusY(int n){
		return n + y;
	}
}
```

Wie Sie sehen können, gibt dieser code in die Konsole 3 aus.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
Will man trotzdem auf das y des äußeren Scopes zurückgreifen, kann man das this-Keyword verwenden, um mit this.y die äußere Variable zu erhalten:

```java
class CodeTeil{  
    CodeTeil(){} // Das bitte ignorieren  
  
    // ab hier wieder coden
    int x = 0;  
    int y = 2;  
    public void main(){  
        int y = 1;  
        System.out.println(plusY(y));  
        System.out.println(plusY(this.y));  
    }  
    
    int plusX(int n){  
        return n + x;  
    }  
    
    int plusY(int n){  
        return n + y;  
    }
}
```

## Style-Regel: Eine Variable sollte immer im innersten möglichen Scope deklariert werden
Dies hat den Hintergrund, dass es den Code übersichtlicher macht, und zusätzlich, dass es verhindert, dass man beim Verwenden von Shadowing durcheinander kommt.
<br />

---
_Autor: David Neumann_
_Kontakt für Fehler und Fragen: davidneumann2155@gmail.com_
# 10: Arrays
Bislang haben wir nur Variablen mit primitiven Datentypen behandelt. Nun werden wir uns mit Datentypen beschäftigen, die mehr als einen Wert speichern können. Der erste dieser Datentypen ist das sog. Array.
Grob vereinfacht stellt ein Array eine Liste da, in der es eine feste Anzahl an Einträgen gibt. 
Möchte man zum Beispiel die ersten 10 Zahlen (beginnend mit 1) festhalten, könnte man das natürlich mit 10 Variablen machen, aber ein Array eignet sich hierfür viel mehr.
Man kann das ganze durch diese Tabelle modellieren:

| Index im Array | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Eintrag | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10|

Wie Sie sehen können, startet ein Array bei seinen Indizes immer mit 0.

Schauen wir uns nun eine Implementierung an. Leeren Sie erstmal wieder ihren CodeTeil bis auf das, was Sie ignorieren sollen, und die main-Methode. Ihr code sollte wieder so aussehen:

```java
class CodeTeil{
	CodeTeil(){} // Das bitte ignorieren
	
	//ab hier wieder coden
	public void main(){
	
	}
}
```

Nun implementieren wir ein Array. In java haben Arrays immer eine feste Länge, und alle Einträge müssen einen festen Datentyp haben. Auch ein Array hat eine Deklaration und eine Initialisierung.

Um einen Datentyp in ein Array zu verwandeln, folgt man der folgenden Syntax:

```java
datentyp[] arrayName; // Deklaration
```

Die []-Klammern beschreiben hierbei die erstellung eines Arrays des Datentyps

Nun die vollständige Syntax:

```java
datentyp[] arrayName; // Deklaration

arrayName = new datentyp[arraylänge]
```

Wichtig ist hierbei die Verwendung des new-Keyword. Dieses kündigt die Erschaffung eines neuen Objektes an, hierzu mehr bei Klassen. 
Dieses muss immer verwendet werden, um ein Array zu erschaffen (Ausnahme direkte Initialisierung, dazu später mehr)
arraylänge muss hierbei ein integer sein.

Erneut können Deklaration und Initialisierung in einem Schritt erfolgen. 
```java
datentyp[] arrayName = new datentyp[arraylänge]
```

Erstellen wir nun ein int-Array der Länge 10 für unser Beispiel:

```java
class CodeTeil{
	CodeTeil(){} // Das bitte ignorieren
	
	//ab hier wieder coden
	public void main(){
		int[] beispielArray = new int[10];
	}
}
```

Unser beispielArray ist nun ein Array der Länge 10. Allerdings sind seine Einträge noch nicht gefüllt. Um einen Eintrag eines Arrays zu bearbeiten, verwendet man folgende Syntax:

```java
arrayName[Eintragsindex]
```

Der Index eines Arrays startet hierbei immer bei 0 und zählt von da hoch. Das heißt unser Array beispielArray lässt sich durch folgende Tabelle modellieren:

| Index im Array | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Eintrag |  |  |  |  |  |  |  |  |  |  |

Sprachlich würde man sagen, alle Einträge unseres Arrays sind NULL, das heißt, ihnen wurde noch kein Wert zugewiesen.

Wir weisen nun dem ersten (also Index 0) Eintrag unseres Arrays den Wert 1 zu und geben diesen anschließend in die Konsole aus.

```java
class CodeTeil{
	CodeTeil(){} // Das bitte ignorieren
	
	//ab hier wieder coden
	public void main(){
		int[] beispielArray = new int[10];
		beispielArray[0] = 1;
		System.out.println(beispielArray[0]);
	}
}
```

Unser Array würde Modelhaft nun so aussehen:

| Index | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Eintrag | 1 |  |  |  |  |  |  |  |  |  |  |

Nun befüllen wir alle Einträge unseres Arrays und geben sie gleichzeitig aus. Hierfür eignet sich eine for-schleife:

```java
class CodeTeil{
	CodeTeil(){} // Das bitte ignorieren
	
	//ab hier wieder coden
	public void main(){
		int[] beispielArray = new int[10];
		for(int x = 0; x < 10; x++){
			beispielArray[x] = x + 1; //Eitnrag eins höher
			System.out.println(beispielArray[x]);
		}
	}
}
```
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

## direkte Initialisierung
Arrays können auch direkt initialisiert werden. Hierfür verwendet man {}-klammern, und trägt die einzelnen Einträge mit ,-Kommas getrennt in die Klammern. In unserem Beispiel sähe das wie folgt aus:

```java
class CodeTeil{
	CodeTeil(){} // Das bitte ignorieren
	
	//ab hier wieder coden
	public void main(){
		int[] beispielArray = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
		for(int x = 0; x < 10; x++){
			System.out.println(beispielArray[x]);
		}
	}
}
```

In diesem Fall wird die Länge des Arrays durch den Java-Compiler festgelegt.

## .length
Häufig ist es nützlich, die Länge eines Arrays zu kennen. Diese ist ein Attribut des Array-Objekts, hierzu mehr bei Klassen. Um die Länge eines Arrays zu erhalten, gibt hängt man hinter den Arraynamen einfach ein .length. (Hinweis, die Arraylänge ist immer 1 über dem letzten Index, d.h. sie beginnt beim Zählen mit 1)
In unserem Beispiel kann man die 10 in der for-loop auch mit beispielArray.length ersetzen:

```java
class CodeTeil{
	CodeTeil(){} // Das bitte ignorieren
	
	//ab hier wieder coden
	public void main(){
		int[] beispielArray = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
		for(int x = 0; x < beispielArray.length; x++){
			System.out.println(beispielArray[x]);
		}
	}
}
```

## for-each:
Eine der umständlichsten Dinge in unserem Beispiel ist die Tatsache, dass wir unser Array mit einer for-schleife manuell ausdrucken müssen. Wollten wir ein weiteres Array drucken, müssten wir eine neue for-schleife erstellen. Um dies zu ändern werden wir nun eine Methode printArray(int[] array) implementieren, die unser Array für uns druckt. Eine mögliche Implementation davon wäre:

```java
class CodeTeil{
	CodeTeil(){} // Das bitte ignorieren
	
	//ab hier wieder coden
	public void main(){
		int[] beispielArray = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
		printArray(beispielArray);
	}
	
	void printArray(int[] array){
		for(x = 0; x < array.length; x++){
			System.out.println(array[x]);
		}
	}
}
```

Es ist vermutlich etwas offensichtlich, dass die Verwendung einer manuellen for-loop zum Iterieren durch ein Array sehr schreibaufwendig ist. Deshalb bietet uns java eine alternative Implementation zum Iterieren durch Arrays. Diese nennt sich for-each Schleife. Die Syntax sieht wie folgt aus:

```java
datentyp[] arrayName = new datentyp[arrayLänge];

for(datentyp x : arrayName) {
	...
}
```

Hierbei durchläuft unsere for-schleife unser Array, und setzt x bei jedem Durchlauf auf den nächsten Eintrag des Arrays.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
In unserem Beispiel sähe die Implementation davon wie folgt aus:

```java
class CodeTeil{
	CodeTeil(){} // Das bitte ignorieren
	
	//ab hier wieder coden
	public void main(){
		int[] beispielArray = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
		printArray(beispielArray);
	}
	
	void printArray(int[] array){
		for(int x : array){
			System.out.println(x);
		}
	}
}
```

Hinweis: Java verwendet für die Funktionalität einer for-each loop einen sog. Iterator. Hierbei handelt es sich um ein Objekt, dass auch für eigene Klassen definiert werden kann. Dadurch ist es möglich auch durch andere Objekte als Arrays/ Arraylisten mit einer for-each-loop zu iterieren. Hierzu vielleicht mehr in einem Exkurs bei Klassen.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

## direkte Erstellung
Manchmal möchte man (z.B. zum Übergeben in eine Methode) ein Array erstellen, ohne es in einer Variable zwischen zu speichern. Dies kann man wie folgt machen:

```java
void doSomething(datentyp[] parameterArray){
	...
}

doSomething(new datentyp[]{...});
```

In unserem Beispiel würde das so aussehen:

```java
class CodeTeil{
	CodeTeil(){} // Das bitte ignorieren
	
	//ab hier wieder coden
	public void main(){
		printArray(new int[]{1, 2, 3, 4, 5, 6, 7, 8, 9, 10});
	}
	
	void printArray(int[] array){
		for(int x : array){
			System.out.println(x);
		}
	}
}
```
<br />

---
_Autor: David Neumann_
_Kontakt für Fehler und Fragen: davidneumann2155@gmail.com_
# Exkurs! 10.1: Arraylists
Ein potentieller Nachteil von Arrays ist die feste Größe dieser. Eine alternative mit beliebiger Größe bieten die sog. Arraylists. Diese stellen ein Array mit einer veränderbaren Größe da. Die Implementation ist etwas anders als mit einem Array.

Syntax:
```java
//ArrayList müssen importiert werden!
import java.util.ArrayList;

//deklaration
ArrayList<Datentypklasse> arrayListName;

//initialisierung
arrayListName = new ArrayList<Datentypklasse>();
```

Wie Sie sehen können wird ganz oben ein import statement verwendet.
Dies liegt daran, dass ArrayLists teil eines java-internen packages sind. Wenn sie ihren Code mit Tab autovervollständigen, wird IntelliJ das package beim erstellen einer ArrayList automatisch importieren, ansonsten müssen sie dies manuell tuen!

Fortsetzung folgt noch...
<br />

---
_Autor: David Neumann_
_Kontakt für Fehler und Fragen: davidneumann2155@gmail.com_
# 11: Strings
Bisher hatten wir uns mit primitiven Datentypen, sowie dem Array befasst. Nun werden wir uns bevor wir uns den Klassen zuwenden noch einen letzten großen Datentyp ansehen, nämlich den String. 
Grundsätzlich gesehen ist ein String eigentlich einfach nur ein char-array. Technisch gesehen geht die Implementation allerdings noch etwas weiter.
Syntax:

```java
String stringName;

stringName = "Hier text eingeben!";
```

Java nutzt wie viele Programmiersprachen zur Identifikation eines Strings "-zeichen. Alles innerhalb der Anführungszeichen wird dem String zugeordnet.

Wir haben einen String bereits in unserem ersten Programm benutzt, um Hello World auszugeben. \[zur Erinerung:

```java
public class Main{  
    public static void main(String[] args){  
        System.out.println("Hello World" //Das ist ein String);  
    }
}
```
\]

Da es bei Strings nicht so viele Unterschiede zu anderen Datentypen gibt, wird hier nicht viel auf sie eingegangen werden, und nur ein paar nützliche Fakten werden erzählt werden. Für eine gute Übersicht von allen Funktionalitäten von Strings empfehle ich [diese Referenz](https://www.w3schools.com/java/java_strings.asp). 

Hinweis: String stellt in java eine Klasse dar, deswegen wird das Keyword großgeschrieben, mehr hierzu bei Klassen.

Hinweis: Durch die Implementation von Strings in Java ist es möglich mit einer for-each-loop durch Strings zu iterieren.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

## String-concatination
Um Strings in java zu kombinieren kann man den +-Operator verwenden. Dieser hängt den String rechts vom Operator an das an Ende des Strings links davon.
<br />

---
_Autor: David Neumann_
_Kontakt für Fehler und Fragen: davidneumann2155@gmail.com_
# 12: Klassen
Dieses Kapitel stellt vermutlich mit Abstand das wichtigste Kapitel im ganzen Kurs da. Klassen bilden wortwörtlich die Grundsteine von Java.

## Was ist eine Klasse?
Grundsätzlich stellt eine Klasse eine Methode zur einfachen Darstellung komplexer Systeme in einem Computerprogramm da.

Als Beispiel werden wir uns nun eine Klasse Mensch vorstellen.
Damit unser Beispiel nicht zu kompliziert ist, werden wir nun für unser Modell ein paar Annahmen machen:
Alle Menschen sind gleich, bis auf ein paar Unterschiede. Diese Unterschiede sind:
- Name
- Größe
- Haarfarbe
- Bewegungsgeschwindigkeit
- Position

Darüber hinaus können unsere Modellmenschen folgendes:
- Bewegen
- Reden

Das ist natürlich extrem vereinfacht, aber es ist für unsere Zwecke ausreichend.

Unsere Klasse Mensch müsste hierbei nun die Attribute größe, haarfarbe, bewegungsgeschwindigkeit und position, sowie die Methoden bewegen und reden implementieren. Dies werden wir nun Schritt für Schritt machen.

All das beantwortet nun immer noch nicht, was eine Klasse ist. Eine Klasse ist quasi eine Schablone, um sog. Objekte als Instanzen von der Klasse zu erzeugen. Ein Objekt ist somit immer eine Instanz einer Klasse. 
Zurück auf unser Beispiel bezogen, wäre Mensch unsere Klasse, und Instanzen (also Objekte) wären zum Beispiel:
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

- Bob:
	- Name = Bob
	- Größe = 170 cm
	- Haarfarbe = Blond
	- Bewegungsgeschwindigkeit = 5 km/h
	- Position = Berlin (52.51868697050777, 13.376152203432627)
- Alice:
	- Name = Alice
	- Größe = 200 cm
	- Haarfarbe = Dunkelbraun
	- Bewegungsgeschwindigkeit = 7 km/h
	- Position = Karlsruhe (49.013163202083504, 8.401971322585181)
- David:
	- Name = David
	- Größe = 180 cm
	- Haarfarbe = Rot
	- Bewegungsgeschwindigkeit = 100 km/h
	- Position = Halle (51.50510286180915, 11.96363985222662)

Jede Instanz der Klasse Mensch würde hierbei dieselben sog. Attribute größe, haarfarbe, bewegungsgeschwindigket, und position besitzen, allerdings andere Werte darin.

Syntax einer Klasse:

```java
class KlassenName{
	...
}
```

KlassenNamen folgen hierbei auch dem camelCase-style, allerdings wird bei ihnen der erste Buchstabe großgeschrieben.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
Wir werden nun eine eigene Klasse bauen. Ersetzen sie dafür CodeTeil wieder mit der leeren Vorlage:

```java
class CodeTeil{  
    CodeTeil(){} // Das bitte ignorieren  
  
    //ab hier wieder coden    
    public void main(){  
        
    }  
}
```

Wir erstellen nun eine neue Klasse Mensch. Klassen müssen außerhalb anderer Klassen erstellt werden. Wir werden Mensch in einem eigenen .java File erstellen. Gehen sie dafür vor, wie auch beim Erstellen der Main-Klasse, und geben sie beim Namen Mensch ein.
Bislang ist unsere Klasse noch leer, wir werden sie nun nach und nach mit Dingen füllen.

Hinweis:
Ab hier wird sowohl in CodeTeil als auch in Mensch weiterprogrammiert werden. Generell wird die meiste Arbeit zu Mensch gehören, deshalb ist allgemein primär Mensch gemeint, wenn in CodeTeil programmiert werden soll wird dies speziell erwähnt werden.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

## constructor
Damit Instanzen einer Klasse erzeugt werden können, bedarf es einem sog. constructor. Dieser stellt Quasi eine Gussform da, wo man Startwerte reingießt, und eine fertige Klasse zurückbekommt.
Die Syntax des constructors sieht wie folgt aus:

```java
class KlassenName{
	...
	KlassenName(...){//Das ist der constructor
		...
	}
	...
}
```

Für unsere Klasse Mensch sieht der constructor vorerst so aus:
```java
class Mensch{
	Mensch(){
	
	}
}
```

Wir werden unseren constructor später mit Funktionalität erweitern.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

## Attribute
Attribute sind einer der Kernpunkte von Klassen. Ein Attribut stellt eine Variable, die der Instanz einer Klasse zugeordnet ist, da. Um ein Attribut zu erstellen, deklariert man einfach eine Variable innerhalb der Klasse:

```java
class KlassenName{
	datentyp Attribut1;
	datentyp Attribut2;
	...
}
```

In unserer Klasse Mensch wären unsere Attribute Größe, Haarfarbe, Bewegungsgeschwindigkeit und Position
Zur Implementierung bieten sich für diese Attribute folgende Datentypen an:

Name lässt sich prima als String implementieren

Größe würde man entweder mit einem Integer oder einem Double implementieren, wir werden einen Integer in cm verwenden.
Außerdem werden wir Größe aufgrund seiner doofen Zeichen(ö und ß kennt der java-compiler nicht) mit size bezeichnen

Für die Haarfarbe bietet sich am meisten ein ENUM an, hierzu mehr im Zusatz ENUM. Wir werden in unserer Implementation einen String verwenden.

Bewegungsgeschwindigkeit kann man wieder mit einem Integer oder einem Double implementieren, wir werden einen Double in km/h verwenden

Die Implementierung der Position ist Interesant, am meisten würde sich hierfür eine eigene Klasse eignen, wir werden stattdessen ein Double-Array verwenden.
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
Implementiert in unsere Mensch-Klasse sieht das ganze wie folgt aus:

```java
class Mensch{ 
	String name;
	int size;
	String haarfarbe;
	double geschwindigkeit;
    double[] position; 
     
    Mensch(){    
    }
}
```

Bisher hat unsere Klasse zwar die Attribute, diese werden jedoch nie initialisiert. Möchte man feste Werte haben, kann man dies bereits bei der Deklarierung festlegen, möchte man diese Werte jedoch für jede Instanz der Klasse Individuell festlegen, so implementiert man die initialisierung im constructor der Klasse. Dabei werden die Attributwerte beim Instanziieren der Klasse (mehr hierzu später) in den Constructor übergeben, und dieser setzt diese in die Attribute.

Es empfiehlt sich bei der Benennung der Attribute des constructors Shadowing zu verwenden.

```java
class Mensch{ 
	String name;
	int size;
	String haarFarbe;
	double geschwindigkeit;
    double[] position; 
     
    Mensch(String name, int size, String haarFarbe, double geschwindigkeit, double[] position){
	    this.name = name;
		this.size = size;
		this.haarFarbe = haarFarbe;
		this.geschwindigkeit = geschwindigkeit;
		this.position = position;
    }
}
```

Hierbei setzt der constructor die Attribute, die mit this. aufgerufen werden, auf die in seine Parameter gegebenen Werte.

## Instanziierung
Nun sind wir bereit unsere ersten Instanzen unserer Klasse Mensch zu erstellen. 
Instanzen einer Klasse sind Objekte, und folgen dementsprechend dem camelCase-style.
Zum Erstellen einer Klasse benötigt man das new-Keyword. 
Syntax:

```java
class KlassenName{
	...
	
	KlassenName(...){
		...
	}
	...
}

class Main{
	KlassenName instanzVonKlassenName;
	
	instanzVonKlassenName = new KlassenName(...);
}
```

Erneut können Deklaration und Instanziierung in einem Schritt erfolgen:

```java
class KlassenName{
	...
	
	KlassenName(...){
		...
	}
	...
}

class Main{
	KlassenName instanzVonKlassenName = new KlassenName(...);
}
```

Am Beispiel unserer Mensch-Klasse werden wir drei Instanzen mit unseren drei Menschen von oben zu erstellen. Dies geschieht in der CodeTeil-Klasse:

```java
class CodeTeil{  
    CodeTeil(){} // Das bitte ignorieren  
  
    //ab hier wieder coden
    Mensch bob = new Mensch("Bob", 170, "Blond", 5, new double[]{52.51868697050777, 13.376152203432627});  
    Mensch alice = new Mensch("Alice", 200, "Dunkelbraun", 7, new double[]{49.013163202083504, 8.401971322585181});  
    Mensch david = new Mensch("David", 180, "Rot", 100, new double[]{51.50510286180915, 11.96363985222662});  
    public void main(){  
  
    }
}
```

Um auf ein Attribut eines Objektes zuzugreifen, verwendet man folgende Syntax:
```java
class Klasse{
	datentyp attribut;
	...
	Klasse(datentyp attribut, ...){
		this.attribut = attribut;
		...
	}
}

Klasse objekt = new Klasse(attribut, ...);

objekt.attribut // zugriff auf das attribut von objekt
```
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
Möchten wir z.B. die Haarfarben unserer drei Personen ausgeben, kann man das wie folgt umsetzen (wir befinden uns immer noch in CodeTeil!):

```java
class CodeTeil{  
    CodeTeil(){} // Das bitte ignorieren  
  
    //ab hier wieder coden
    Mensch bob = new Mensch("Bob", 170, "Blond", 5, new double[]{52.51868697050777, 13.376152203432627});  
    Mensch alice = new Mensch("Alice", 200, "Dunkelbraun", 7, new double[]{49.013163202083504, 8.401971322585181});  
    Mensch david = new Mensch("David", 180, "Rot", 100, new double[]{51.50510286180915, 11.96363985222662});  
  
    public void main(){  
        System.out.println(bob.haarFarbe);  
        System.out.println(alice.haarFarbe);  
        System.out.println(david.haarFarbe);  
    }
}
```
<br />

---
_Autor: David Neumann_
_Kontakt für Fehler und Fragen: davidneumann2155@gmail.com_
# 12.1: Methoden von Klassen
Bisher halten Objekte unserer Klasse Mensch nur Daten, sie besitzen jedoch keinerlei Funktionalität. Dies werden wir nun mit drei Methoden machen:
talk, eine Methode, die einen String in die Konsole ausgibt
move, eine Methode, die die Koordinaten des Objekts nach gewissen regeln verändert.

Zunächst implementieren wir die talk-methode. Diese soll einen String entgegennehmen, und diesen zusammen mit dem Namen des Verfassers in die Konsole ausgeben. Die Implementation in die Klasse Mensch sähe wie folgt aus:

```java
class Mensch{  
	String name;
    int size;  
    String haarFarbe;  
    double geschwindigkeit;  
    double[] position;  
  
    Mensch(String name, int size, String haarFarbe, double geschwindigkeit, double[] position){  
	    this.name = name;
        this.size = size;  
        this.haarFarbe = haarFarbe;  
        this.geschwindigkeit = geschwindigkeit;  
        this.position = position;  
    }    
    
    void talk(String satz){  
        System.out.println(name + ":" + satz);  
    }
}
```
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>
Um nun talk aufzurufen, gehen wir wie auch mit Attributen vor (wieder in CodeTeil!):

```java
class CodeTeil{  
    CodeTeil(){} // Das bitte ignorieren  
  
    //ab hier wieder coden
    Mensch bob = new Mensch("Bob", 170, "Blond", 5, new double[]{52.51868697050777, 13.376152203432627});  
    Mensch alice = new Mensch("Alice", 200, "Dunkelbraun", 7, new double[]{49.013163202083504, 8.401971322585181});  
    Mensch david = new Mensch("David", 180, "Rot", 100, new double[]{51.50510286180915, 11.96363985222662});  
  
    public void main(){  
        System.out.println(bob.haarFarbe);  
        System.out.println(alice.haarFarbe);  
        System.out.println(david.haarFarbe); 
        bob.talk("Ich sage diesen Satz")
    }
}
```

Nun werden wir uns noch mit der Implementierung der move-methode befassen. Vorerst wird diese noch sehr primitiv sein, wir werden sie evtl. später noch ausbauen. Bislang wird die move-methode einfach nur den ersten Eintrag des Positionsarrays manipulieren, indem sie einen double als Angabe für die Zeit, die bewegt wurde, entgegennimmt, und diesen mit der Geschwindigkeit verrechnet. Auch die Eigenschaft das Koordinaten nur bis 360° laufen wird vorerst ignoriert werden. Eine Implementation kann z.B. so aussehen:
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

```java
class Mensch{  
    String name;  
    int size;  
    String haarFarbe;  
    double geschwindigkeit;  
    double[] position;  
    
    Mensch(String name, int size, String haarFarbe, double geschwindigkeit, double[] position){  
        this.name = name;  
        this.size = size;  
        this.haarFarbe = haarFarbe;  
        this.geschwindigkeit = geschwindigkeit;  
        this.position = position;  
    }  
    
    void talk(String satz){  
        System.out.println(name + ": " + satz);  
    }
    
	void move(double dauer){  
	    position[0] = position[0] + dauer * geschwindigkeit;  
	}
}
```

Die Formel für die Berechnung der neuen Position kann hierbei frei manipuliert werden, der Ansatz dahinter sollte aber in einem Kommentar festgehalten werden!
<br />

---
_Autor: David Neumann_
_Kontakt für Fehler und Fragen: davidneumann2155@gmail.com_

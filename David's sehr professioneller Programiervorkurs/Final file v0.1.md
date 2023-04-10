# 0: Einleitung
Bei diesem Kurs handelt es sich um einen groben Einstieg in das Programieren und die Programiersprache Java.

Aufgrund der angepeilten Länge, werden tiefere Konzepte wie etwa die Objektorientierung nur sehr oberflächlich angeschnitten werden. Die Konzepte die hier vermittelt werden sollen, sind lediglich die Grundstrukturen die für das Arbeiten mit Java nötig sind.

Aufbau:
1. Was ist ein Programm/ Algorithmus
2. Einführung und Installation einer IDE
3. Standardaufbau eines Java Programms
4. "Hello World" oder auch das erste Programm
5. Variablen und simple datentypen
6. if und else statements, Vergleichsoperatoren
	1. *switches*
7. for und while
8. methoden
	1. Parameter
	2. Rückgabewerte
	3. Überladung
	4. *Rekursion*
9. Scoping
10. Arrays (listen)
	1. Arrayllists
11. Strings (Das Textdingsda)
12. Klassen und Objekte
	1. Methoden
	2. Vererbung
13. static und final
14. public, private und protected
### Zusatz
15. ENUMs (Enumerations)
16. Funktionale Programmierung
17. Nachwort

Hinweis: 
Das sieht nach viel aus, aber viele dieser Konzepte lassen sich sehr Intuitiv verstehen, und bedürfen vor allem von der Sprachlichen Konstruktion (Syntax) übung. Ein verständnis für diese Konzepte zu haben reicht als vorteil für Objektorientierte Programmierung definitiv aus. Zusätzlich sind vor allem nur die Punkte 1 - 14 wirklich wichtig, der Rest wird noch in der Vorlesung zu genüge behandelt.

# 1: Was ist ein Programm
Formal defniert ist das etwas dumm, deshalb hier eine kurze erklärung:
Ein Programm ist eine Abfolge von Schritten, die ausgeführt werden sollen. 
Beispielsweise kann ein Programm eine Zusammenfassung verschiedener Algorithmen zum lösen eines Zauberwürfels, oder auch eine System zum berechenen von verschiedenen Mathematischen Operationen (z.B. Addition, Multiplikation, Taylorreihe, Newton-Methode etc.) sein.
Allgemein folgt eine Program einer logischen Abfolge von teilschritten, um eine gewünschte Operation durchzuführen

Falls trotzdem jemand die offizielle Definition hören will bitte sehr:
Ein **Computerprogramm** oder kurz **Programm** ist eine den Regeln einer bestimmten Programmiersprache genügende Folge von Anweisungen (bestehend aus Deklarationen und Instruktionen), um bestimmte Funktionen bzw. Aufgaben oder Probleme mithilfe eines Computers zu bearbeiten oder zu lösen. (Danke [Wikipedia](https://de.wikipedia.org/wiki/Computerprogramm))

# 2: Einführung und Installation einer IDE

1. Was ist eine IDE:

Bei einer IDE einer sogennanten "integrated develop enviroment" handelt es sich um ein Programm, das einem Funktionalitäten zum einfacheren entwickeln von Programmen bietet. (z.B. Syntaxkontrolle, autovervollständigung etc.)
Grundsätzlich kann man ein Programm in jedem Texteditor erstellen, es ist aber trotzdem empfehlenswert, eine IDE zu verwenden, um sich einiges an Arbeit zu sparen. 
Es gibt verschiedene IDE's für verschiedene Sprachen. Für Java gibt es zwei große IDE's:
Eclipse und IntelliJ IDEA. Diese Installationserklärung wird sich auf die InteliJ Community Edition beziehen, da es die IDE ist, die ich empfehlen würde, zu Eclipse findet man aber auch mehr als genug Tutorials im Internet.

2. Installation und Einrichtung

Den Download von IntelliJ IDEA Community Edition finden Sie unter
https://www.jetbrains.com/idea/download/#section=windows
hier:
![[Download.png]]
Laden Sie die Datei herunter, und führen Sie sie aus. Sie werden in ihrem Betriebssystem der Installation zustimmen müssen. Anschließend öffnet sich das Installationsfenster. Klicken Sie in diesem auf Next >
![[installer1.png]]
Nun können Sie den Installationsort auswählen. Falls Sie das gemacht haben, oder ihn nicht ändern wollen, gehen Sie wieder auf next >
![[installer2.png]]
Nun haben Sie verschiedene Optionen. Ich würde es empfehlen hierbei eine assoziation mit .java dateien zu erstellen, dies ist aber nicht nötig. Auch einen Desktopshortcut können Sie hier erstellen. Durch Add "Open Folder as Project" können Sie in Windows mit rechtsclick ordner als IntelliJ Projekt in IntelliJ öffnen. Alle diese Dinge sind nicht nötig. Falls Sie sie trotzdem wollen, können Sie sie auswählen. Sie brauchen ihre PATH-Variablen nicht zu Updaten. Wällen Sie aus was Sie wollen, und clicken Sie dann auf next >
![[installer3.png]]
Nun können Sie eine Startmenüordner auswählen. Ich würde empfehlen, diesen beim standard zu belassen. Clicken Sie auf Install um die Installation zu starten.
![[installer4.png]]
Die Installation wird eine Weile brauchen. Clicken Sie anschließend Run IntelliJ IDEA Community Edition und dann auf finish.
![[installer5.png]]
Warten Sie, bis IntelliJ gestartet ist. Was Sie nun sehen, ist die Öffnungsseite von IntelliJ. 
Wir werden nun ein Projekt erstellen. Clicken Sie auf New Project
![[intellij CE 1.png]]
In dem jetzigen Fenster haben Sie eine menge Optionen. Geben Sie bei Name einen Namen für das Projekt ein. Der hier verwendete Name wird TestProjekt (achtung auf die Groß- und Kleinschreibung!!!) sein. Entfernen Sie den Haken bei "Add sample code"!
Sie werden eine JDK spezifizieren müssen. Dabei handelt es sich um eine Datei, die quasi Werkzeuge für das Programieren von Java bereitstellt. Clicken Sie dafür auf JDK.
![[ProjektSetup1.png]]
Bei Ihnen werden vermutlich keinerlei JDK bereit liegen, bei mir sind bereits einige vorinstalliert. Wir werden so oder so nun die neueste JDK (aktuell Version 19) installieren. Clicken Sie dafür auf "Donload JDK..."
![[JDKInstallation1.png]]
Das neue Fenster sollte wie folgt aussehen
![[JDK2.png]]
Falls dem so ist, gehen Sie auf Download
Nun öffnet sich ein Ladevorgang. Warten Sie, bis dieser abgeschlossen ist.
Die JDK sollte nun automatisch als JDK ausgewählt worden sein.
![[ProjektSetup2.png]]
Falls dem nicht so ist, wählen Sie sie einfach in dem JDK Fenster aus.
Clicken Sie nun auf Create

Ich werde Ihnen nur einen kurzen überblick über das allerwichtigste geben, vieles werden Sie im laufe der Zeit kennen lernen.

Hier sehen Sie die Dateien ihres Projektes:
![[projektDateien.png]]

Hier ist die Konfiguration des Projektes, dazu später mehr.
![[config.png]]

Und hier sind einige wichtige Utility Tools, auch hierzu später mehr.
![[utility.png]]

Fahren Sie nun mit Abschnitt 3 weiter fort.

# 3: Aufbau eines Javaprogramms
## Erste Schritte

Rechtsclicken Sie auf den Ordner namens src bei den Dateien
![[src.png]]
gehen Sie ganz oben auf den Reiter New,
![[New.png]]
und wählen Sie dann java class aus, um eine neue Datei zu erstellen.
![[java class.png]]
Was das genau ist wird erneut später erklärt werden. Geben Sie in das Namensfeld einen Namen (am besten einfach "Main") ein. 
![[Main.png]]
Diese Klasse wird ihre Hauptklasse, die auch die main methode enthalten wird (siehe unten). Erneut, ergibt dies viel mehr Sinn, wenn man die späteren Konzepte versteht.

Im Hauptbereich sollte sich nun ein Fenster geöffnet haben, dies ist "ihr Programm" (Technisch gesehen handelt es sich hierbei um den Code der Hauptklasse ihres Programms, aber naja close enough IMO).

Ihr Programm sollte bisher so aussehen:
```java
public class Main {
}
```

Die geschwungenen Klammern beschreiben hierbei den Body der Klasse, alles was darin steht, steht innerhalb der Klasse.


Nun werden wir die main methode implementieren.

## main methode:
Die main methode ist der Teil des Programms, der beim Start des Programms einmal ausgeführt wird. Diese wird immer gleich Konstruiert. Es empfiehlt sich ihren aufbau auswendig zu lernen.
Erstellen Sie einen neuen Abschnitt(Enter) im inneren des Bereichs der geschwungen Klammern (Body), und schreiben Sie das folgende in den Body der Main-Klasse:
```java
	public static void main(String[] args){
	
	}
```

Bemerkungen:
1. IntelliJ verfolständigt automatisch einiges, z.B. klammern für Sie
2. Hierbei dienen die Einrückungen zum Behalten des überblicks zum Body, in dem man sich befindet. IntelliJ nimmt Ihnen die Einrückarbeit größten Teils ab. Einrückungen können auch mit Tab erzeugt werden.
Ihr Code sollte nun wie folgt aussehen:

```java
public class Main {
	public static void main(String[] args){
		
	}
}
```

Was diese Keywords genau bedeuten, wird später noch genauer erläutert werden.

Javacode wird normalerweise in mehre eigene Dateien aufgeteilt, dazu mehr bei Klassen
Die main-methode kommt innerhalb eines Projektes allerdings nur einmal vor, und stellt quasi das Herz des Programms da. Ihr Inhalt wird dabei durch die geschwungenen {} Klammern (ihren Body) begrenzt. Alles innerhalb dieser Klammern steht in der Methode, alles außerhalb steht außerhalb der Methode!
Außerhalb und innerhalb der main-methode können Variablen, Klassen, sowie weitere methoden definiert werden. Dazu aber bei den einzelnen Bereichen mehr. Der Hauptunterschied ergibt sich hierbei durch das sog. Scoping (dazu mehr in Scoping)

## Libraries

Häufig benötigt man in java sog. Libraries. Das sind quasi Sammlungen, in denen von anderen Programmierern bereits funktionalitäten umgesetzt wurden (zum Beispiel das berechnen des logarithmus oder so). Diese werden mit dem import Keyword in das Program geladen. Aus Stilgründen werden imports immer ganz am Anfang des Programms geschrieben. 
Bsp. (bitte nicht mitcoden):

```java
import Fisch
import xyz

public class Main{
	public static void main(String[] args){
	...
	}
}
```

Dies sind die größten Dinge über den Aufbau von java-code, näheres wird dann in den einzelnen Kapiteln erklärt.

Fahren Sie nun mit Abschnitt 4 fort. Dort werden wir unser erstes Programm ausführen.

# 4: "Hello World" oder auch das erste Programm

Nun soll das erste Java-Programm geschrieben werden. Das erste was man eigentlich in jeder Programiersprache macht, ist ein Program zu schreiben, das "Hello World" ausgiebt.

Dies werden Sie nun ebenfalls machen.

Ihr code sollte bislang wie folgt aussehen:

```java
public class Main{
	public static void main(String[] args){
		
	}
}
```

Geben Sie nun in den Body der main-methode folgendes ein:

```java
		System.out.println("Hello World");
```

Ein besonderer Hinweis hierbei auf das Semicolon am Ende des Befehls. Dieses dient in Java immer zur signalisierung eines beendeten Teilschritts, und muss zwangsweise nach fast allen Dingen verwendet werden. (Nach jeder Deklaration oder manipulation von Variablen, sowie nach aufruf einer Methode)

Ihr code sollte nun wie folgt aussehen:

```java
public class Main{
	public static void main(String[] args){
		System.out.println("Hello World");
	}
}
```

Nun konfigurieren wir das Projekt um es ausführbar zu machen!
Gehen Sie dafür auf current File und dann auf Edit Configuration:
![[current.png]]
Clicken Sie auf +, dann auf Application
![[application.png]]
Geben Sie nun in das Feld Main class den Namen ihrer Hauptklasse in unserem Beispiel Main ein, clicken Sie Enter und nochmal Enter
![[Mainclass.png]]
Nun können Sie das Programm mit dem grünen Pfeil in der Oberen Rechten Ecke ausführen. (Dies wird auch in zukunft mit "führen Sie das Programm aus" gemeint sein) Tun Sie das
![[run.png]]
Es wird etwas brauchen, dann sollte ein Fenster im unteren Bereich aufpoppen, das wie folgt aussieht.
![[fenster.png]]
Im folgenden wird dieser Teil als Konsole bezeichnet werden. Sie können sehen, dass darin Hello World geschrieben wurde.
Falls dies Funktioniert hat, fahren Sie mit Abschnitt 5 fort.

## Kommentare:

Um code übersichtlicher zu gestallten, ist es häufig sinnvoll, kommentare zur funktionalität von Dingen im Code selbst zu verfassen. Dies kann in Java auf zwei Arten erfolgen:

### 1: //
ein Kommentar mit zwei // Strichen blendet alles auf der selben Zeile rechts der Striche beim ausführen aus, dass heißt, hiermit kann man bemerkungen zu einer Zeile schreiben

### 2: /\*Inhalt\*/
Will man mehrzeilige kommentare verfassen, so kann man /\*...\*/ verwenden. Alles was hierbei innerhalb der \*\* steht, wird beim ausführen des Programmes nicht beachtet.

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

# 5: Variablen und primitive Datentypen

Nun werden Variablen eingeführt. Eine Variable ist grundsätzlich ein wie eine Art Platzhalter, dem man einen Wert zuweisen, den inhalt manipulieren,  und von dem man den Wert auslesen kann. In unterschiedlichen Programiersprachen werden Variablen unterschiedelich implementiert. In java sind Variablen grundsätzlich statisch typisiert. Das bedeutet, das man einer Variable einen Datentyp zuweist, und diese Variable behält den Datentyp bei. Gängige Datentypen sind:

int (Integer): Ganzzahlen zwischen -2^31 und 2^31

float (floating point number): Kommazahlen (Aufbau ist etwas deutlich komplexer)

char (character): Buchstabe (aus der ASCII-Tabelle) wird angegeben durch das ' zeichen vor und nach dem Buchstaben ('c'/ '1'/ '%' etc. )

boolean: Wahrheitsvariable, die entweder Wahr oder Falsch ist.

Darüber hinaus gibt es noch ein paar weitere sog. primitive Datentypen, diese erwähne ich jedoch aufgrund ihrer unrelevanz nicht näher, eine Beschreibung finden Sie im Anhang.

Es gibt zwei wichtige Schritte beim erstellen einer Variable. Die Deklarierung, und die Innitialisierung:
Bei der Deklarierung werden Datentyp und Scope (siehe Scoping) der Variable festgelegt. 

Diese folgt dem Schema:
```java
// Schema
datentyp variablenName;
```

Nomenklatur:
Variablen folgen in Java dem camelCase Style, das heißt, sie beginnen kleingeschrieben, und jedes neue Wort wird groß geschrieben. Der ganze Name muss zusammenhängend sein. Der Anfang darf keine Zahl sein

Bsp.:

```java

float spielerDurchschnitt;

int größterGemeinsamerTeiler;

int xDividiertDurch2;
```


Erweitern Sie ihren Code wie im Beispiel unten um den integer x, den character c, und den boolean bool. Tun Sie dies innerhalb des Bodies der main-methode, vor der Ausgabesystematik(System.out.println("Hello World"))!

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

Um eine Variable zu verwenden, muss sie zusätzlich Initialisiert werden, dass heißt, ihr wird ein Startwert zugewiesen. Dies wird mit dem = Operator gemacht, nachdem die Variable deklariert wurde:

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
datentyp variable = wert;
```

Bsp.:

```java
int x = 0;
```

Hinweis: Aufgrund des Aufbau von java müssen variablen, die ausserhalb von methoden initialisiert werden sollen, direkt bei der Deklaration initialisiert werden.

initialisieren Sie nun x mit 4, char mit 'd', und bool mit false. Achten Sie darauf, dies direkt bei der Deklaration zu machen. Ihr code sollte nun so aussehen:

```java
public class Main{	
	public static void main(String[] args){
		int x = 4;
		char c = 'd';
		boolean bool;
		System.out.println("Hello World");
	}
}
```

## Manipulation von Variablen

Das interessante an Variablen ist, das man Sie nicht nur festlegen, sondern auch manipulieren und auslesen kann. Um dies zu verdeutlichen, ersetzen Sie den Inhalt der main methode mit folgendem Code:

```java
		System.out.println(bool);
		System.out.println(c);
		System.out.println(x);
		x = x+2
		System.out.println(x);
```

Ihr code sollte nun so aussehen:
```java
public class Main {  
    public static void main(String[] args){  
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
Wie Sie sehen können wurde einmal 4 und einmal 6 ausgegeben.
Dies kam durch die Operation x = x + 2 zustande. Diese ist nicht wie in der Mathematik als Gleichung sondern vielmehr als logischer ablauf zu lesen:

1. x = y <> setze die Variable links auf den Wert rechts.
2. x + 2 <> Berechne x + 2

Logisch geschiet hierbei folgendes:
1. x = x + 2 interpretiert als x = y also setze x auf y
2. y = x + 2 (setze y auf x + 2)
3. x wird ausgelesen
4. der ausgelesene wert von x wird um 2 erhöhrt
5. das ergebnis, das y wäre wird in x eingespeichert.

Wichtig hierbei: Mathematische Operationen beachten Operationspriorität (also Klammern vor Punkt vor Strich)

Für verschiedene Datentypen gibt es verschiedene Operationen, die man mit der Zeit lernt und deshalb hier nicht genauer aufgeführt werden. Was ich nun noch aufzählen werde, sind die wichtigsten operationen für variablen.

"+=" bzw. "-=" und "\*=" bzw. "/=":

Wie bereits gezeigt, kann man auf eine integer Variable mittels

```java
x = x + 2
```

eine Zahl addieren. Genau so geht das auch mit der multiplikation, hierfür verwendet man einen Stern \*:
```java
x = x * 2
```

Analog dient "-" für subtraktion und "/" für division.

Da diese Schreibweise jedoch recht umständlich ist, wenn man x einfach nur um eine Zahl verändern möchte, bietet java noch ein paar einfachere Schreibweisen:

```java
//adition
x = x + 2;
//äquivalent zu
x += 2;

//subtraktion
x = x - 2;
//äquivalent zu
x -= 2;


//multiplikation
x = x * 2;
//äquivalent zu
x *= 2;

//division
x = x / 2;
//äquivalent zu
x /= 2;

//sonderfall
x = x + 1;
//äquivalent zu
x++;

//sonderfall
x = x - 1;
//äquivalent zu
x--;
```

Aufgabe 1:

Was speichern die folgenden Datentypen:

int

char

float

boolean


Lösung:
int: ganzzahlen
char: buchstaben
float: kommazahlen
boolean: Wahr oder Falsch

Aufgabe 2:

Erweitern Sie ihren Code um die Variable y. Diese soll Ganzzahlen halten und auf 5 starten.


Lösung: 

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

Aufgabe 3:

Geben Sie y in die Konsole aus, multiplizieren Sie anschließend y mit 3 und geben Sie y wieder in die Konsole aus.


Lösung:

```java
public class Main {  
    public static void main(String[] args){  
        int x = 4;  
        char c = 'c';  
        boolean bool = false;  
        int y = 5;
  
		System.out.println(y)
        System.out.println(x);  
        x = x + 2;
        y = y * 3;
        // alternativ auch y *= 3*
        System.out.println(x);  
        System.out.println(y);
    }  
}
```

## Interaktion von Variablen:

Variablen können auch mit einander Kombiniert werden.

Bsp.:

```java
public class Main{
	public static void main(string[] args){
		int x = 3;
		int y = 7;

		System.out.println(x); // 3
		System.out.println(y); // 7
		x = x + y // x = 3 + 7 = 10
		y += x // y = 10 + 7 = 17
		System.out.println(x); // 10
		System.out.println(x); // 17
	}
}
```

Dies fasst zum größten Teil zusammen, was es über Variablen zu sagen gibt, es wird später aber noch auf das Scoping von Variablen eingegangen werden.

# 6: if und else statements, Vergleichsoperatoren

Um Logische Abläufe modelieren zu können ist es notwendig, if und else statements sowie Vergleichsoperatoren zu behandeln.

## if-statement:
ein if-statement stellt eine Art Schalter da. Der Aufbau sieht wie folgt aus:

```java
if(statement){
...
}
```

Der Code innerhalb des Bodies({}-Klammern) der if-Methdode wird nur dann ausgeführt, wenn statement true ist, also wenn die Aussage davon erfüllt ist. Um logische Abfragen damit zu machen gibt es die sog. Vergleichsoperatoren. Es werden hier nur die Essentiellen Vergleichsoperatoren vorgestellt, weitere entnehmen Sie bitte dem Anhang. 

### Gleichheitsoperator:
== oder auch gleicheitsoperator gennant ergibt wahr, wenn links und rechts von dem Operator Gleiche Ergebnisse stehen.

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

Wichtig hierbei anzumerken, ist das Typen beim vergleichen mit dem Vergleichsoperator auch immer verglichen werden, also gibt x == a immer falsch zurück, egal welche Werte x und a haben, da ihre Typen unterschiedlich sind.


## Relationsoperatoren:
Die Relationsoperatoren < und > sowie <= und >= vergleichen die größenrelationen von Zahlen. (Hinweis: hiermit können auch float und int verglichen werden)

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

## else-statement:
häufig soll in einem Programm entweder eine Sache oder eine andere Sache ausgeführt werden. Um dies zu erhalten wäre es ungünstig zwei if statements zu schreiben, da dies zwei mal die vergleichsoperation Abfragen würde. Deshalb gibt es das else-statement. Dieses wird immer dann aufgerufen, wenn das vorhergehende if-statement NICHT ausgeführt wurde.

Struktur:

```java
if(statement){
...
}else{
...
}
```

Bsp.:

```java
int x = 2; //Immer wieder veränderbar

if(x > 0){
x--;
}else{
x++;
}
```

Hierbei wird x um 1 reduziert, wenn es größer als Null ist, und um 1 erhöht, wenn es kleiner-gleich Null ist.


## else if

Häufig gibt es mehrere logische verkettungen von if und else statements. auf ein if statement kann auch ein else if statement folgen.

Syntax:

```java
if(statement){
...
}else if(statement){
...
}else if(statement){
...
}usw...
```

Hierrauf kann auch am Ende noch ein else-statement folgen, dieses muss aber aufgrund des logischen Abschlusses immer ganz am Ende kommen.

## onliner:

Häufig muss man nach einem if-statement nur eine einzige Operation ausführen. Um sich Arbeit zu sparen existiert hierfür eine Kurzform:

```java
if(statement)...;
```

Bsp.:

```java
int x = 2;
if(x > 0)x++;
else x--;
```

Wie man sehen kann, kann eine Operation auch ohne die Klammern des sonst üblichen Bodies durchgeführt werden.

## Zusatz!!
Durch verständnis der oneliner ergibt sich auch der logische Sinn von else-if-statements.
Man könnte den Ablauf auch so ausdrücken:

```java
if(statement)...;
else{
	if(statement)...;
	else{
		if(statement)...;
		else{
			...
		}
		}
}
```

Wie man sehen kann ist dieser Aufbau aber deutlich aufwendiger.

# 7: for und while schleifen

Häufig möchte man beim Programieren Dinge mehrfach durchführen.

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

Dies jedoch durch copy und paste durchzuführen birgt eine riesige Gefahr:
Sobald das kopierte Segment einen Fehler enthält sind direkt alle Kopien davon auch fehlerhaft. Darüber hinaus ist es auch einiges an Arbeit, und unübersichtlich. In dem Beispiel ist zum Beispiel system klein statt groß geschrieben. Außerdem hat sich ein a eingeschlichen.

Deshalb bietet java sog. Schleifen. Diese wiederholen Code, bis ihr exit-requirement erfüllt ist.
Diese werden nun vorgestellt.

## for-schleifen:

for-schleifen bieten meist die Praktikabelste Möglichkeit zum iterieren(wiederholen) von Code.
Ihre Syntax ist wie folgt:

```java
for(variable x = Anfangswert; exit-statement; operation auf x){
...
}
```

Bsp.:

Der Code von oben, nur als Schleife

```java
for(int x = 0; x < 5; x++){
System.out.println(x);
}
```

x wird hierbei die Zählervariable oder auch Iterationsvariable genannt.  Das exit-statement, ist das Statement, was false, also falsch sein muss, damit die Schleife beendet wird. Hier ist dies erfüllt wenn x echt-größer als 5 ist. Die Operation auf x ist eine beliebige Operaton auf x, die am Ende jeder Iteration also jeden Durchlaufs der for-schleife durchgeführt wird. In diesem Fall heißt das, dass x nach jeder Iteration um 1 erhöht wird.

Kehren wir zu unserem Codeprojekt zurück:

Löschen Sie den gesamten Inhalt des Bodies der main()-methode.

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
		for(int x = 0; x < 5; x++){
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

```java
public class Main{
	public static void main(String[] args){
		for(int x = 0; x < 11; x++){
			System.out.println(x);
		}
	}
}
```

bzw.

```java
public class Main{
	public static void main(String[] args){
		for(int x = 0; x <= 10; x++){
			System.out.println(x);
		}
	}
}
```

Aufgabe 2:

Erstellen Sie eine weitere Schleife, die die ersten 5 ungeraden Zahlen (1, 3, 5, 7, 9) ausgibt.

pot. Lösungen:

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
		for(int x = 0; x < 4; x ++){
			System.out.println(2x + 1);
		}
	}
}
```

weitere Lösungen sind auch möglich

## while-schleifen.

While schleifen sind ähnlich zu for-schleifen, bedürfen aber nicht der gleichen Strenge bei der Konstruktion.

Synatx:

```java
while(statement){
...
}
```

Der Inhalt der Schleife wird wiederholt, solange das statement nicht false wird.

for und while schleifen lassen sich fast immer in einander übersetzen.

Bsp.: Die for-schleife von oben in eine while-schleife translatiert

```java
int x = 0;
while(x < 5){
	System.out.println(x);
	x++;
}
```

Wie Sie sehen können sind while-schleifen vom Ablauf ähnlich zu for-schleifen, bieten aber den Raum, die Variable zum beispiel am Anfang statt am Ende zu verändern.

Beide Schleifentypen haben vor und nachteile, und eignen sich für unterschiedliche Probleme besser und schlechter.

Am Ende ist es auch sehr eine Frage der übung.


## while(true) und break;
wie Sie vielleicht schon bemerkt haben, muss eine while-schleife (übrigens auch eine for-schleife) nicht immer ihre exit-requirement erreichen. Das Wohl einfachste beispiel hierfür stellt:

```java
while(true){
	...
}
```

da. In diesem Beispiel ist das Statement in der while-schleife (obviously) immer true, also wird diese Schleife sich unendlich wiederholen.  Dies kann auch als Funktionalität verwendet werden:

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

Möchte man vorzeitig, eine schleife verlassen, existiert dafür das break-statement.

Bsp.:

Wieder unsre for-schleife von oben, anders modeliert:

```java
int x = 0;

while(true){
	System.out.println(x);
	if(x == 5){
		break;
	}
}
```

Bemerkung: 
Java verwendet einen Compiler um Code effizienter zu machen. IntelliJ zeigt Ihnen Änderungen durch den Compiler an, und schlägt ihnen Verbesserungen for. Deshalb wird das exit-statement der while-schleife hier von IntelliJ kritisiert werden.

# 8: Methoden
Wie wir bereits gesehen haben, ist es sehr ungünstig, code mehrfach zu verwenden. 
Will man trotzdem komplexere Codesegmente mehrfach verwenden, empfiehlt sich die Nutzung von Methoden.

EINSCHUB!:
Ab hier verkompliziert der Aufbau von java uns den Vorgang leider etwas. Deshalb werden wir einen kleinen Trick verwenden, um uns vieles leichter zu machen.(also eigentlich zu verhindern, das wir zu viele zu komplexe Themen unbehandelt verwenden müssen)

Ersetzen Sie ihren bisherigen Code durch folgendes (Sie dürfen copy-pasta machen):

```java
public class Main{  
    static CodeTeil code = new CodeTeil();  
    public static void main(String[] args){  
        code.main();  
    }  // das hier alles noch ignorieren
}  
  
class CodeTeil{  
    CodeTeil(){}  //diesen Teil ignorieren  
// ab hier wieder coden

  
    public void main(){  
    } 
}
```

Wir werden ab sofort in der main-methode der CodeTeil Klasse weitercoden, d.h. diese ist absofort mit der main-methode gemeint. Der ganze obere Teil kann ab sofort ignoriert werden, und wird nicht mehr in Beispiele eingebracht werden (bis wir später über Klassen gesprochen haben). Auch den ersten Abschnitt innerhalb der CodeTeil Klasse ignorieren Sie bitte vorerst.

Bsp.:
In die Konsole soll zu unterschiedlichen Zeiten das Quadrat der Variable x ausgegeben werden.

Schlechte Implementation

```java
public class CodeTeil{
	CodeTeil(){}
	public static void main(String[] args){
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

Im Beispiel wurde ausversehen x + x, statt x \* x verwendet. Außerdem hat sich erneut ein c eingeschlichen. 

Stattdessen bietet sich die Implementierung einer Methode printSquareOfX() an.

Aber zunächst:

Die Syntax von Methoden:

```java
rückgabewert methodenName(*Parameter){
	...
}
```
rückgabewert stellt hierbei den Typ des Rückgabewerts der Methode dar, hierzu mehr bei Rückgabewerte, wir werden erstmal nur void, also keinen Rückgabewert verwenden.

Parameter werden im nächsten Abschnitt behandelt werden.

Der Inhalt des Bodies der Methode stellt den Code da, der beim aufrufen der Methode ausgeführt werden soll.

Nomenklatur:

Die Namen von Methoden werden wie die Namen von Variablen im camelCase Style gebildet (siehe 5.)

Zurück zu unserem Beispiel:

Eine Methode zum ausgeben des Quadrates von x könnte zum Beispiel so aussehen:
```java
void printSquareOfX(){
	System.out.println(x * x);
}
```

Implementiert in unseren code sähe das ganze wie folgt aus:

```java
class CodeTeil{  
    CodeTeil(){} // Das bitte ignorieren  
    //ab hier wieder coden    
    public int x = 0;  
    
    public void main(){  
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
Um eine Methode auszuführen muss man sie aufrufen.
Dies geschiet, indem man den Methodennamen mit () hinten dran schreibt.
In unserem Beispiel würden wir also alle aufrufe von System.out.printl(x + x); durch printSquareOfX() ersetzen.

Hinweis, AutoCompletion:
IntelliJ schlägt Ihnen vermutlich wenn Sie anfangen printSquareOfX() zu schreiben, bereits diese Methode vor. In dem Sie Tab drücken, können Sie das Autocompletion feature von IntelliJ nutzen, um sich Zeit zu sparen!

Unser Code sieht dann wie folgt aus:
```java
class CodeTeil{  
    CodeTeil(){} // Das bitte ignorieren  
    //ab hier wieder coden    public int x = 0;  
  
    public void main(){  
        printSquareOfX();  
        x += 5;  
        printSquareOfX();  
        for(int y = 0; y < 4; y++){  
            x++;  
            printSquareOfX();  
        }  
        x = -4;  
        printSquareOfX();  
    }  
  
    void printSquareOfX(){  
        System.out.println(x * x);  
    }  
}
```

Nun werden wir uns Parameter für Methoden ansehen.
## 8.1: Parameter

Eines der größten Probleme unserer bisherigen Implementation der Methode zum ausdrucken des Quadrats unserer Variable ist der, dass dies nur mit der Variable x funktioniert. Würden wir zum Beispiel noch eine Variable y deklarieren, müssten wir für sie eine ganz neue Methode schreiben.
Außerdem könnte eine Variable, die innerhalb der main-methode deklariert wurde gar nicht verwendet werden.

Eine Lösung hierfür stellen Parameter da. Diese erlauben es uns einen Wert in die Methode zu übergeben, denn wir dann darin verwenden. Ein Parameter ist quasi eine Variable, die beim aufrufen der Methode erzeugt wird. Parameter werden beim definieren der Methode als variablen innerhalb der () klammern deklariert, und durch , getrennt.

Syntax:

```java
rückgabewert methodenName(datentyp Parameter1, datentyp Parameter2, ...)
```

in unserem Beispiel ließe sich unsere Methode wie folgt verallgemeinern:

```java
void printSquareOfNumber(int number){
	System.out.print(number * number);
}
```

Hinweis: Refractoring:
IntelliJ bietet möglichkeiten zum Refractorn von Code, also zum umstrukturieren. Eine der simpelsten beispiele hiervon ist das umbennen von methoden oder variablen. Durch das nutzen des Refractoring features werden gleichzeitig die methode und alle ihre Aufrufe umbenannt. Zum benutzen clicken Sie gleichzeitig SHIFT und F6 während Sie die Methode ausgewählt haben, geben Sie den neuen Namen ein, und drücken Sie dann Enter

im Code implementiert wäre das:

```java
class CodeTeil{  
    CodeTeil(){} // Das bitte ignorieren  
    //ab hier wieder coden    public int x = 0;  
	int x = 0;

    public void main(){  
        printSquareOfNumber();  
        x += 5;  
        printSquareOfNumber();  
        for(int y = 0; y < 4; y++){  
            x++;  
            printSquareOfNumber();  
        }  
        x = -4;  
        printSquareOfNumber();  
    }  
  
    void printSquareOfNumber(int number){  
        System.out.println(number * number);  
    }  
}
```

Wie Sie vielleicht sehen untertreicht IntelliJ nun alle Aufrufe von printSquareOfNumber. Dies liegt daran, dass diese Methode nun bei jedem Aufruf eine Eingabe erwartet. Dies geschiet, in dem man einen Wert (beziehungsweise den Inhalt einer Variable) des passenden Datentypen in die klammern beim Aufrufen der Methode schreibt. Man sagt, man übergibt den Wert in den Parameter der Methode.

In unserem Beispiel würde das wie folgt aussehen:
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
        }  
        x = -4;  
        printSquareOfNumber(x);  
    }  
  
    void printSquareOfNumber(int number){  
        System.out.println(number * number);  
    }  
}
```

Hinweis: da wir x nur noch übergeben, können wir es wieder in die main-methode verschieben.

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
        }  
        x = -4;  
        printSquareOfNumber(x);  
    }  
  
    void printSquareOfNumber(int number){  
        System.out.println(number * number);  
    }  
}
```

### java-interne methoden:
java bietet von sich aus einige methoden an. So ist zum Beispiel auch System.out.println eine (überladene, mehr hierzu bei Überladung) Methode. Um dies etwas zu verdeutlichen, schreiben wir uns eine eigene print()-methode, und verwenden diese in printSquareOfNumber (ja methoden können auch methodenaufrufe enthalten) statt System.out.prinln

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
        }  
        x = -4;  
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

Die funktionalität bleibt hierbei genau die gleiche.

Im nächsten Abschnitt werden wir uns nun mit Rückgabewerten beschäftigen

## 8.2: Rückgabewerte
Dieses Kapitel ist wohl eines der wichtigsten Kapitel beim Lernen von Programiersprachen. Ein tieferes Verständnis für Rückgabewerte von methoden liefert eine große Einsicht in die funktionalität der meisten Programiersprachen (auch wenn das auf dem Elementaren Level meistens nochmal etwas komplizierter wird.)

Bisher haben unsere methoden nur Werte entgegen genommen, aber nichts zurück gegeben. Dies wird sich nun ändern.
Dafür werden wir die bisherige funktionalität unserer printSquareOfNumber-methode aufspalten, in eine Methode, die uns das Quadrat einer Zahl berechnet, und eine Methode die uns eine Zahl ausdruckt (bzw. dies haben wir bereits).

Dafür werden wir die Methode square(int number) implementieren. 
Diese soll einen integer zurückgeben. Java weist methoden stets einen festen Rückgabewert zu. Diesen schreibt man beim Definieren der Methode ganz an den Anfang. Bisher war unser Rückgabewert stets void, d.h. unsere Methode hat nichts zurück gegeben. 
Mann gibt einen Wert mithilfe des keywords return zurück.
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
(vom ablauf her wird zunächst das produkt aus number mit number berechnet, und dieses dann zuückgegeben)
In unseren code implementiert sähe das in etwa so aus:

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
        }  
        x = -4;  
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
1. Der Rückgabewert von square muss verarbeitet werden. In unserem Beispiel tun wir dies, in dem wir ihn in eine Variable einspeichern. 
2. Der Code kann simpler gestaltet werden. Man kann den Rückgabewert einer methode auch direkt(also ohne ihn in eine Variable zwischen zu speichern) in eine weitere methode übergeben. Dies würde in unserem Beispiel dann so aussehen:
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
}
```
vom Ablauf her würde zunächst number in square übergeben werden, dort würde dann das Quadrat von number zurückgegeben werden und dieses würde dann direkt in print() übergeben werden.

#### Operatoren sind methoden (zumindest in etwa)

Wir haben in unseren Programmen ja bereits Operatoren wie  \==, < oder auch + verwendet. Diese lassen sich prima als methoden modelieren (auch wenn sie am Ende definitiv ganz anders implementiert sind)

Bsp.:
1. Stellen wir uns eine modelhafte dastellung des \== Operators für integer vor:
```java
boolean ==(int leftSide, int rightSide){
	if(leftSide gleich rightSide) return true;
	else return false;
}
```

2. Stellen wir uns die modelhafte Darstellung des +-Operators für integer vor:
```java
int +(int leftSide, int rightSide){
	return (summe aus leftSide und rightSide);
}
```

Technisch ist die Implementation beide male natürlich ganz anders, (etwas zu kompliziert für das hier, da geht es dann um sowas auf einer maschinellen Ebene) aber diese Dastellung stellt recht gut da, dass Operatoren eigentlich auch nur einen Rückgabewert zurückgeben.

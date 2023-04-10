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
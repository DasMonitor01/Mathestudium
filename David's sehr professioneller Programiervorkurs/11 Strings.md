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
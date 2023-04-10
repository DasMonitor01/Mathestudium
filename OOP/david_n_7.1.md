Probleme:
1.:
Das Array books wurde nie initialisiert. Deshalb sind keine Aufrufe von Elementen aus books möglich, da dies Versucht, Elemente von null auszulesen. Dies erzeugt eine NullPointerException

2.:
In addAsBooks wird versucht dem Eintrag nextFreePos in books die Parameter mit Hilfe der Methoden von Book zuzuweisen. Allerdings wird ein Array über Objekte in java standardmäßig mit null als Wert für alle Objekte des Arrays initialisiert. Deswegen verweißt der Aufruf books\[nextFreePos\].setTitle(...) auf ein null, es wird also versucht die Methode setTitle von null auszuführen. Da null kein Objekt ist, erzeugt dieser Methodenaufruf eine NullPointerException, analog für die anderen setter aufrufe. Stattdessen muss eine neue Instanz von Book erstellt und in books\[nextFreePos\] abgespeichert werden.

3.:
nextFreePos wurde nicht erhöht, also wurde nur auf eine Position des Arrays zugegriffen
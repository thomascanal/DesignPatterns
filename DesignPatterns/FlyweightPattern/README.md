# Problem
Wie kann man grosse zusammengesetzte Objekte durch den Einsatz von elementaren Objekten, effizient beschreiben?

# Lösung
Definiere eine abstrakte und schmale Schnittstelle, dass durch ein konkretes leichtgewichtiges Objekt und vom normalen Objekt implementiert wird.

Eine Factory erzeugt und verwaltet alle Flyweights. Somit werden nur die notwendigen Objekte bei Bedarf erzeugt.

# UML
![Fylweight Uml](Flyweigth_UML.png?raw=true "UML")

# Vorteile
Das Verfahren reduziert Speicherkosten proportional zur Größe des ausgelagerten Zustands und zur Anzahl der Fliegengewichte. Die Speicherkosten 
sinken weiter, wenn der ausgelagerte Zustand nicht gespeichert werden muss, sondern berechnet werden kann.

# Nachteile
Die Komplexität steigt relativ stark, insbesondere bei Designs, die Fliegengewicht gemeinsam mit Kompositum nutzen. Eine saubere Dokumentation 
der Verantwortlichkeiten ist ein Muss. Die Laufzeitkosten steigen möglicherweise an, da der ausgelagerte Zustand wieder aufgefunden und dem 
Fliegengewicht beim Methodenaufruf übergeben werden muss. Sie steigen weiter, wenn der Zustand berechnet wird.
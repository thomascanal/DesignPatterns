# Problem
Wie kann eine Abstraktion implementiert werden ohne die Vererbung in der Abstraktion, als auch in der Implementierung hineinzuziehen.

# Lösung
Werden die abstrakten Klassen und die Implementierungen in zwei verschiedenen Hierarchien verwaltet, so gewinnt erstens die Übersichtlichkeit 
und zweitens wird die Anwendung unabhängig von der Implementierung.

# UML
![Bridge Uml](Bridge_UML.png?raw=true "UML")

# Vorteile
* Abstraktion und Implementierung werden entkoppelt.
* Die Implementierung ist während der Laufzeit dynamisch änderbar.
* Die Erweiterbarkeit von Abstraktion und Implementierung ist verbessert.
* Durch Angabe eines Parameters bei der Erzeugung einer Abstraktion kann die Implementierung gewählt werden.
* Für den Klienten wird die Implementierung vollständig versteckt.
* Vermeidung einer starken Vergrößerung der Anzahl der Klassen.

# Nachteile
* Keine Implementierung von Funktionalität in abstrakten Klassen erlaubt
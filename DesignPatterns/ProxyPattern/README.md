# Problem
Wie kann auf ein Objekt welches mit speziellen Vorbedingungen und Verbindungen zugriffen werden?

# Lösung
Definiere eine Schnittstelle und implementiere sowohl das reale als auch das Proxy Objekt. Der Zugriff auf das reale Objekt soll jedoch nur über den Proxy erfolgen.

# UML
![Proxy Uml](Proxy_UML.png?raw=true "UML")

# Vorteile
* Proxies können den Zugang zu Objekten kontrollieren, bevor sie die Methodenaufrufe an das Subjekt delegieren
* Der Client bemerkt die Kontrolle des Objekts nicht
* Proxies funktionieren ebenfalls, wenn das eigentliche Objekt noch nicht im Speicher verfügbar ist (z.B. Lazy Loading)
* Proxies können helfen, die Geschwindigkeit der Applikation zu steigern (z.B. Caching)
* Proxies können die Interprozesskommunikation/Fernkommunikation zwischen Objekten ermöglichen

# Nachteile
* Proxies können je nach Implementierung die Antwortzeit verzögern
* Proxies fügen eine weitere Abstraktionsschicht ein, welche zu Umwegen führen kann und die Komplexität steigert
* Es müssen alle von der Schnittstelle definierten Methoden für das Proxy erstellt und an das Subjekt delegiert werden
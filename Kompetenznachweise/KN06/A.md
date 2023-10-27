# Auftragserfüllung

## Recherche zu Fachbegriffen
- **High Availability (HA)**: Kontinuierliche Systemverfügbarkeit durch Redundanz und Automatisierung. Beispiel: USV bei Stromausfall.

- **Fault Tolerance (FT)**: Systemfunktion trotz schwerwiegender Fehler oder Ausfälle. Beispiel: RAID für Datensicherheit.

### HA-Maßnahmen bei Stromausfall
- *Beispiel*: Installation einer USV im Serverraum für Stromausfallschutz.

- *Cloud-Provider*: Geringere Relevanz, da diese eigene Stromversorgungssysteme besitzen.

### HA-Maßnahmen bei Erdbeben
- *Beispiel*: Erdbebenerkennungssensoren zur automatischen Systemabschaltung bei Erschütterungen.

- *Cloud-Provider*: Geografisch verteilte Rechenzentren minimieren Katastrophenrisiken.

### FT-Maßnahmen
- *Beispiel*: RAID für Datenintegrität und Redundanz.

- *Cloud-Provider*: Automatische Redundanz in Cloud-Services, z.B. doppelte Datenbankserver.

## Load Balancer (AWS)
- *AWS Load Balancer*: Verteilt Datenverkehr auf Server für Lastenausgleich, Skalierbarkeit und Hochverfügbarkeit.

- *Typen von AWS Load Balancern*:
    1. **Application Load Balancer (ALB)**: Für HTTP/HTTPS, z.B. Webanwendungen.
    2. **Network Load Balancer (NLB)**: Für TCP/UDP, z.B. IoT-Anwendungen.
    3. **Classic Load Balancer (CLB)**: Einfacher Lastenausgleich.

- *Beispiel*: ALB für HTTP-Verkehr auf Webserver.

- *Kombination mit Auto Scaling*: Auto Scaling passt Instanzen an Bedarf an, Load Balancer verteilt Verkehr.

- *Sicherheitsmaßnahmen*: WAF, AWS Shield, Netzwerksicherheitsgruppen.

- *Leistungsüberwachung und -optimierung*: CloudWatch für Metrikenbasierte Skalierung.

## Auto Scaling (AWS)
- *AWS Auto Scaling*: Automatische Anpassung von EC2-Instanzen für Skalierbarkeit und Verfügbarkeit.

- *Arten von Richtlinien*: 
    - *Zielverfolgung*: Anpassung basierend auf Metriken wie CPU-Auslastung.
    - *Manuelle Skalierung*: Benutzerdefinierte Einstellungen.
    - *Zeitpläne*: Geplante Skalierung.

- *Beispiel*: Auto Scaling startet Instanzen bei hohem Verkehr.

- *Kostenoptimierung*: Reduziert Ressourcenkosten durch bedarfsgerechte Skalierung.

- **Elastic Load Balancing (ELB)**: Gleichmäßige Lastenverteilung auf Auto Scaling-Gruppen.
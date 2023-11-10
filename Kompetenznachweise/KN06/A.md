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

## Auto Scaling (AWS) -> horizontal Scaling
- *AWS Auto Scaling*: Automatische Anpassung von EC2-Instanzen für Skalierbarkeit und Verfügbarkeit.

- *Arten von Richtlinien*: 
    - *Zielverfolgung*: Anpassung basierend auf Metriken wie CPU-Auslastung.
    - *Manuelle Skalierung*: Benutzerdefinierte Einstellungen.
    - *Zeitpläne*: Geplante Skalierung.

- *Beispiel*: Auto Scaling startet Instanzen bei hohem Verkehr.

- *Kostenoptimierung*: Reduziert Ressourcenkosten durch bedarfsgerechte Skalierung.

- **Elastic Load Balancing (ELB)**: Gleichmäßige Lastenverteilung auf Auto Scaling-Gruppen.

## Redundanz im Serverraum


1. **Serverreplikation**:
   - Serverraum: Betrieb von zwei identischen Servern, um bei Hardwarefehlern oder Ausfällen nahtlos zu wechseln.
   - Cloud-Provider: Bereitstellung mehrerer virtueller Maschinen (VMs) in verschiedenen Verfügbarkeitszonen oder Regionen und Verwendung eines Load Balancers zur Traffic-Verteilung.

2. **Redundante Netzwerkkomponenten**:
   - Serverraum: Verwendung von redundanten Switches und Firewalls, um die Netzwerkkontinuität sicherzustellen.
   - Cloud-Provider: Bereitstellung von mehreren Load Balancern und Konfiguration von virtuellen Netzwerken mit Failover-Optionen.

3. **Datensicherung und Backup**:
   - Serverraum: Regelmäßige Backups von Daten und Konfigurationen, um Datenverluste zu verhindern.
   - Cloud-Provider: Verwendung von integrierten Datensicherungsdiensten und automatisierten Backups für VM-Images und Datenbanken in verschiedenen Regionen oder Rechenzentren.

Vertical Scaling und Horizontal Scaling sind zwei verschiedene Ansätze zur Steigerung der Leistung und Kapazität von IT-Systemen:

## Vertical / Horizontal Scaling

**Vertical Scaling (auch als "Scale Up" bezeichnet)**:
- Beim Vertical Scaling wird die Leistung eines einzelnen Servers oder einer einzelnen Maschine erhöht, indem mehr Ressourcen wie CPU, RAM oder Festplattenkapazität hinzugefügt werden.
- Dieser Ansatz ist in der Regel teurer, da er den Austausch oder die Aktualisierung der Hardware des Servers erfordert.
- Es eignet sich gut für Anwendungen, die eine begrenzte Skalierung benötigen oder bei denen eine einzige leistungsstarke Maschine ausreicht.

**Horizontal Scaling (auch als "Scale Out" bezeichnet)**:
- Beim Horizontal Scaling werden zusätzliche Server oder Maschinen hinzugefügt, um die Last auf mehrere Einheiten zu verteilen.
- Dieser Ansatz ist oft kosteneffizienter, da günstigere Standardhardware verwendet werden kann, und er bietet eine bessere Skalierbarkeit für Anwendungen mit starkem Verkehrsaufkommen.
- Es ist besonders geeignet für webbasierte Anwendungen, die eine hohe Skalierbarkeit erfordern.

Unterschiede:
- Der Hauptunterschied liegt in der Art und Weise, wie sie die Leistung erhöhen. Vertical Scaling erweitert einen einzelnen Server, während Horizontal Scaling zusätzliche Server hinzufügt.
- Vertical Scaling kann teurer sein und ist auf die physische Kapazität eines Servers beschränkt, während Horizontal Scaling besser für große Workloads und flexiblere Skalierbarkeit geeignet ist.
- Horizontal Scaling ist oft ein Schlüsselkonzept in Cloud-Computing-Umgebungen, wo Ressourcen bedarfsgerecht hinzugefügt werden können.

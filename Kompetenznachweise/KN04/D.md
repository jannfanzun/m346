## Speicherdienste und entsprechende Eigenschaften kennen 

Die drei unterschiedlichen Storage-Optionen in AWS sind Block Storage, Object Storage und File Storage. Hier sind die Kategorisierungen und Use-Cases für jede dieser Optionen:

**1. Block Storage:**
   - Persistenz: Ja
   - Geschwindigkeit: Hoch
   - Sicherheit: Je nach Einstellungen und Verschlüsselung
   - Standort: Region
   - Weitere Charakteristiken: Direkter Blockzugriff, für virtuelle Maschinen und Datenbanken geeignet.

   **Use-Case:** Block Storage wird oft für Daten verwendet, die von virtualisierten Umgebungen und Datenbanken benötigt werden, wo eine hohe Geschwindigkeit und Zuverlässigkeit erforderlich sind. Zum Beispiel, das Hosten einer Datenbank oder das Bereitstellen von schnellem Speicher für virtuelle Maschinen.

**2. Object Storage:**
   - Persistenz: Ja
   - Geschwindigkeit: Variabel, oft hoch
   - Sicherheit: Gute Sicherheitsfunktionen für Objekte
   - Standort: Global
   - Weitere Charakteristiken: Skalierbarkeit, Metadaten, geeignet für unstrukturierte Daten.

   **Use-Case:** Object Storage wird häufig für das Speichern großer Mengen von unstrukturierten Daten wie Bilder, Videos, Backups und Log-Dateien verwendet. Zum Beispiel, das Hosting von Mediendateien für eine Website oder das Sichern von Backups in der Cloud.

**3. File Storage:**
   - Persistenz: Ja
   - Geschwindigkeit: Mittel bis hoch
   - Sicherheit: Abhängig von Konfiguration und Berechtigungen
   - Standort: Region
   - Weitere Charakteristiken: Gemeinsam genutzter Dateizugriff, Datei-Protokolle (NFS, SMB).

   **Use-Case:** File Storage wird oft für gemeinsam genutzten Dateizugriff in einem Netzwerk verwendet, wo mehrere Benutzer auf dieselben Dateien zugreifen müssen. Zum Beispiel, das Speichern von Benutzerdateien in einer Dateifreigabe oder das Teilen von Dokumenten zwischen Benutzern in einer Organisation.

Diese Kategorisierung hilft dabei, die jeweiligen Stärken und Schwächen der verschiedenen Storage-Optionen in AWS zu verstehen und den besten Storage-Typ für bestimmte Anwendungsfälle auszuwählen.
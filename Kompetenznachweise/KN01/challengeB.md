# Evaluation Cloud-Migration für ein Unternehmen mit 50 Mitarbeitern (Einstiegsübung)
---
### Ausgangslage:
Ihr Unternehmen mit **50 Mitarbeitern** betreibt aktuell die IT **On-premises**. Die monatlichen IT-Kosten setzen sich aus verschiedenen Faktoren zusammen, darunter ein NAS-Speicher von **20 TB**. Die Hardware wird innerhalb von 3 Jahren abgeschrieben. 

#### Schritte:

**Schritt 1:** Kostenanalyse On-Premises Fixkosten **pro Monat** aufnehmen.
 

| **Kostenart**                    | **Betrag**  |
|:---------------------------------|------------:|
| Raummiete                        | 1'000.-     |
| Administration (20% Stelle)      | 1'000.-     |
| Server (HPE Proliant)            | 2'500.-     |
| Netzwerk und weitere Geräte      | 2'500.-     |
| Diverses (Lizenzen etc.)         | 2'500.-     |
| **Gesamtkosten On-Premises**     | **9'500.-** |

<br>

 

**Schritt 2a:** Kostenanalyse **Variante Low** - AWS Instance-Type **t2.micro** pro Monat evaluieren:
| **Kostenart**                    | **Betrag**  |
|:---------------------------------|------------:|
| AWS EC2 **t2.micro** (Var. A)    | 11.66.-     |
| AWS S3-Speicher **20TB**         | 460.-       |
| Administrator                    | 1000 .-     | 
| Diverses                         | 2500 .-     |
| **Gesamtkosten AWS Low**         | **3’971.66.-** |

<br>

**Schritt 2b:** Kostenanalyse **Variante X-Large** - AWS Instance-Type **m4.xlarge** pro Monat evaluieren:

| **Kostenart**                    | **Betrag**  |
|:---------------------------------|------------:|
| AWS EC2 **m4.xlarge** (Var. B)   | 276.48      |      
| AWS S3-Speicher **20TB**         | 460.-       |
| Administrator                    | 1000.-      |  
| Diverses                         | 2500.-      |
| **Gesamtkosten AWS xlarge**      | **4’236.48.-** |

 

<br>

**Schritt 3:** Vergleich der drei Varianten pro Monat, pro Jahr und auf 3 Jahre:

| **Variante**   | **Pro Monat**  | **Pro Jahr**   | **3 Jahre**    |
|:---------------|--------------:|--------------:|--------------:|
| On-Premises    | 9'500.-       | 114'000.-     | 342'000.-     |
| t2.micro       | 3'971.66.-    | 47'659.92.-   | 142'979.76.-  |
| m4.xlarge      | 4'236.48.-    | 50'837.76.-   | 152'513.28.-  |

 

<br>

#### Vorteile und Nachteile der Cloud im Vergleich zu On-Premises.

**Vorteile:**
- **Skalierbarkeit:** Die Cloud ermöglicht es, Ressourcen nach Bedarf zu skalieren, was flexibler ist als die Vorhaltung von Hardware in On-Premises-Rechenzentren.

- **Kosteneffizienz:** Cloud-Dienste bieten Pay-as-you-go-Modelle, bei denen Sie nur für die tatsächlich genutzten Ressourcen zahlen, was potenziell kosteneffizienter ist als der Kauf und die Wartung von Hardware.

- **Weltweite Erreichbarkeit:** Cloud-Dienste sind global verfügbar und ermöglichen den Zugriff von überall auf der Welt, was die Zusammenarbeit und den Datenaustausch erleichtert.

- **Automatisierung:** Cloud-Plattformen bieten umfangreiche Automatisierungstools, die die Bereitstellung und Verwaltung von Anwendungen erleichtern.

- **Aktualisierungen und Sicherheit:** Cloud-Anbieter kümmern sich um Software-Updates und Sicherheitsaspekte, was die Wartung vereinfacht.

**Nachteile:**
- **Abhängigkeit vom Anbieter:** Die Nutzung der Cloud bedeutet eine Abhängigkeit von einem externen Dienstanbieter, was Datenschutz- und Verfügbarkeitsbedenken aufwerfen kann.

- **Kostenkontrolle:** Ohne effektives Kostenmanagement können die monatlichen Ausgaben in der Cloud außer Kontrolle geraten.

- **Datenschutz und Compliance:** Die Speicherung sensibler Daten in der Cloud kann datenschutzrechtliche und compliancebezogene Herausforderungen mit sich bringen.

- **Internetverbindung erforderlich:** Die Nutzung der Cloud erfordert eine zuverlässige Internetverbindung, was in abgelegenen Regionen oder in Situationen mit begrenzter Konnektivität problematisch sein kann.

- **Latenz:** Bei bestimmten Anwendungen, die eine geringe Latenz erfordern, kann die Cloud möglicherweise nicht die beste Option sein.

- **Risiko von Ausfällen:** Cloud-Dienste können gelegentlich Ausfälle haben, was die Verfügbarkeit beeinträchtigen kann.

- **Vendor-Lock-in:** Wenn Sie sich für eine Cloud-Plattform entscheiden, sind Sie möglicherweise an diese gebunden, was die Migration zu einem anderen Anbieter schwierig machen kann.


<br>


#### Quellen

- [Amazon EC2 - Preise](https://aws.amazon.com/de/ec2/pricing/)
- [Amazon S3 - Preise](https://aws.amazon.com/de/s3/pricing/)
- [AWS Pricing Calculator](https://calculator.aws/#/)




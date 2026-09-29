# M231 Lernjournal

### Ylli Uka

### PE26a

### Tag 6

### 28.09.26
---
 <details>
  <summary>
Block: Checklisten Datenschutzbeauftragter 
  </summary>




**Thema:** Webtracking & Datenschutz auf Websites  
**Quelle:** [datenschutz.ch - Webtracking verhindern](https://www.datenschutz.ch/meine-daten-schuetzen/webtracking-verhindern)

---





### Checkliste 1: Website-Datenschutz & Cookie-Handling (Eigene Nutzung)

| # | Prüfpunkt | Einschätzung | Kommentar / Massnahme |
|---|---|---|---|
| 1 | **Einwilligung (Consent-Banner)**: Werden Tracking-Cookies abgelehnt? | Erfüllt | Cookies werden zu 90 % konsequent abgelehnt(manuell); Brave Shields blockiert viele Banner direkt. |
| 2 | **Transparenz in Datenschutzerklärung**: Werden genutzte Dienste geprüft? | Teilweise | Auf besuchten Seiten wird die Datenschutzerklärung bei Bedarf stichprobenartig auf Tracking-Dienste geprüft. |
| 3 | **IP-Anonymisierung & Schutz**: Wird die IP-Adresse geschützt? | Erfüllt | Brave Shields und Adblocker verhindern direkte Anfragen an bekannte Tracking-Server. |
| 4 | **Do Not Track (DNT) / GPC**: Wird das Signal zur Nicht-Nachverfolgung gesendet? | Erfüllt | Brave sendet automatisch Signale wie Global Privacy Control (GPC) / DNT an Webseiten. |
| 5 | **Drittlandübermittlung**: Werden Datenabflüsse in Drittstaaten minimiert? | Erfüllt | Durch das Blockieren von US-Trackern (z. B. Google Analytics) wird der ungewollte Datenabfluss verhindert. |

---

 
### Checkliste 2: Technische Schutzmassnahmen (Konkretes Setup)

| # | Prüfpunkt | Einschätzung | Kommentar / Massnahme |
|---|---|---|---|
| 1 | **Deaktivierung von Drittanbieter-Cookies**: Sind Third-Party-Cookies blockiert? | Erfüllt | Der Brave Browser blockiert Third-Party-Cookies standardmässig und konsequent. |
| 2 | **Einsatz datenschutzfreundlicher Alternativen**: Werden sichere Tools genutzt? | Erfüllt | Brave Browser sowie 1Password / Proton Pass für sicheres Passwort-Management im Einsatz. |
| 3 | **Skript- und Tracker-Blockierung**: Werden Fingerprinting & Skripte blockiert? | Erfüllt | Integrierter Adblocker & Brave Shields blockieren Werbe-Skripte und Tracker automatisch. |
| 4 | **Sichere Passwort- & Sitzungsverwaltung**: Werden Zugangsdaten geschützt? | Erfüllt | Verwenden von Passwort-Managern (1Password / Proton Pass) schützt vor Phishing und schwachen Passwörtern. |
| 5 | **Isolierung von Nutzungskontexten**: Werden Sitzungsdaten getrennt? | Erfüllt | Brave isoliert Storage und Cookies pro Domain (Ephemeral Storage / Fingerprinting Protection). |
---

### Aha-Moment:
Wie krass viele digitale Spuren man beim ganz normalen Surfen hinterlässt, ohne es überhaupt zu merken, aber gleichzeitig, wie **einfach** man sich davor schützen kann. Man muss absolut kein IT-Profi sein und oft reichen schon ein paar gezielte Einstellungen im Browser aus.

### Was ich gelernt habe:
* **Schutz ist eine Kombination:** Es reicht nicht, nur gelegentlich Cookie-Banner wegzuklicken. Wirklich effektiv ist das Zusammenspiel aus eigenem Verhalten (z. B. Logouts nach der Nutzung), richtigen Browser-Einstellungen (Drittanbieter-Cookies blockieren) und passenden Schutz-Tools.
* **Automatische Helfer nutzen:** Ein datenschutzorientierter Browser (wie Brave) oder gute Add-ons nehmen einem 90 % der Arbeit ab und blockieren Tracker ganz automatisch im Hintergrund.
* **Gewohnheiten anpassen:** Schon kleine Änderungen wie die Nutzung von alternativen Suchmaschinen (DuckDuckGo/Startpage) oder Passwort-Managern (1Password/Proton Pass) bringen extrem viel Schutz mit sehr wenig Aufwand.
* 
---
</details>
 

<details>
<summary>Vigenère-Chiffre mit Cryptool.org</b></summary>

### Vigenère-Verschlüsselung (Praxis-Test)
* **Funktionsweise:** Im Gegensatz zur Caesar-Chiffre wird kein fester Zahlenwert, sondern ein **Schlüsselwort (nur aus Buchstaben)** genutzt.
* **Durchführung auf cryptool.org:**
  * **Klartext:** `DATENSCHUTZ`
  * **Schlüssel:** `MODUL`
  * **Geheimtext:** `POWYYEQKOEL`

![cryptool](img/Cryptool.png)

### Was ich bei Vigenère gelernt habe
* **Polyalphabetische Verschlüsselung:** Derselbe Klartext-Buchstabe wird je nach Position im Schlüsselwort zu unterschiedlichen Geheimtext-Buchstaben verschoben.
* **Schutz vor einfacher Häufigkeitsanalyse:** Da Buchstaben nicht immer gleich ersetzt werden, verwischen die typischen Buchstaben-Muster einer Sprache.

</details>


<details>
<summary> KI-Werkstatt : Caesar-Häufigkeitsanalyse</b></summary>

### Caesar-Code knacken mit Häufigkeitsanalyse
* **Rolle der KI:** Generatorin des Chiffrats (Schlüssel vorab geheim).
* **Geheimtext:** `KPL KHALUZPJOLYOLPA PZA PT TVKBS ZLOY DPJOAPN`
* **Analyse-Schritte:**
  * Buchstabenzählung: `P` (7x) und `L` (3x) kommen am häufigsten vor.
  * Anwendung des Merkworts **ENISRAT** (Annahme: Der häufigste Buchstabe im Deutschen ist **E**).
  * Die Annahme `L` = `E` ergibt eine Verschiebung von 7 Stellen im Alphabet.
* **Ergebnis:**
  * **Schlüssel:** `7`
  * **Klartext:** `DIE DATENSICHERHEIT IST IM MODUL SEHR WICHTIG`

### Was ich bei der Caesar-Häufigkeitsanalyse gelernt habe
* **Unzulänglichkeit von Caesar:** Monoalphabetische Verfahren sind sehr unsicher, da die Sprachstatistik (z. B. **ENISRAT** im Deutschen) im Geheimtext vollständig erhalten bleibt.
* **Schnelle Verifikation:** Kurze Häufigkeitswörter (wie `KPL` → `DIE` oder `PZA` → `IST`) verraten und bestätigen den Schlüssel innerhalb von Sekunden.

</details>


`
## Fazit Tag 06

* **Webtracking:** Mit den richtigen Browser-Einstellungen (Brave, Drittanbieter-Cookies blockieren) und Tools (Proton Pass / 1Password) stoppt man 90 % der Spuren automatisch.
* **Caesar & ROT13:** Sehr einfach, aber unsicher – mit der deutschen Buchstaben-Häufigkeit (**ENISRAT**) lässt sich der Code sofort knacken.
* **Vigenère (Cryptool):** Durch ein Schlüsselwort ändern sich die Verschiebungen, was einfaches Abzählen verhindert.

**Fazit:** Alle Blöcke von Tag 06 gelöst und das Prinzip symmetrischer Verschlüsselung komplett verstanden!

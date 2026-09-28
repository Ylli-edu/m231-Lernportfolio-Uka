# M231 Lernjournal

### Ylli Uka

### PE26a

### Tag 6

### 28.09.26



**Thema:** Webtracking & Datenschutz auf Websites  
**Quelle:** [datenschutz.ch - Webtracking verhindern](https://www.datenschutz.ch/meine-daten-schuetzen/webtracking-verhindern)  


---

## Checkliste 1: Website-Datenschutz & Cookie-Consent

| # | Prüfpunkt | Einschätzung | Kommentar / Massnahme |
|---|---|---|---|
| 1 | **Einwilligung (Consent-Banner)**: Werden Tracking-Cookies erst nach expliziter Zustimmung gesetzt? | Teilweise | Cookie-Banner ist vorhanden, aber der «Ablehnen»-Button ist schwer auffindbar. Muss gleichwertig platziert werden. |
| 2 | **Transparenz in Datenschutzerklärung**: Werden alle Tracking-Tools namentlich genannt? | Nicht erfüllt | Ein Analytics-Dienst ist aktiv, fehlt aber in der Datenschutzerklärung. Sofortige Ergänzung notwendig. |
| 3 | **IP-Anonymisierung**: Werden IP-Adressen bei Analyse-Tools gekürzt? | Erfüllt | IP-Anonymisierung im Skript ist korrekt konfiguriert. |
| 4 | **Do Not Track (DNT)**: Respektiert die Website das DNT-Signal des Browsers? | Nicht erfüllt | DNT-Header wird vom Server ignoriert. Konfiguration auf dem Webserver anpassen. |
| 5 | **Drittlandübermittlung**: Werden Daten in Länder ohne angemessenen Datenschutz (z. B. USA) übermittelt? | Teilweise | Übermittlung findet statt; Standardvertragsklauseln (SCC) vorhanden, Risikoanalyse fehlt noch. |

### Reflexion zu Checkliste 1
Bei der Überprüfung der Webtracking-Massnahmen fällt auf, dass technische Grundeinstellungen wie die IP-Anonymisierung oft problemlos funktionieren, während rechtliche Vorgaben wie die transparente Datenschutzerklärung vernachlässigt werden. Besonders Cookie-Consent-Banner stellen eine häufige Schwachstelle dar, wenn das Ablehnen erschwert wird. Überrascht hat mich, wie viele Daten ungewollt an Drittanbieter abfliessen können, wenn keine genaue Überprüfung stattfindet.

---

## Checkliste 2: Technische & Organisatorische Schutzmassnahmen (Webtracking verhindern)

| # | Prüfpunkt | Einschätzung | Kommentar / Massnahme |
|---|---|---|---|
| 1 | **Deaktivierung von Drittanbieter-Cookies**: Sind Third-Party-Cookies standardmässig blockiert? | Teilweise | Im Browser empfohlen; auf der Website werden Third-Party-Cookies noch nicht konsequent verhindert. |
| 2 | **Einsatz datenschutzfreundlicher Alternativen**: Werden datenschutzfreundliche Suchmaschinen und Dienste genutzt? | Erfüllt | Dienste wie DuckDuckGo oder Startpage werden als datenschutzfreundliche Alternativen gefördert. |
| 3 | **Skript- und Tracker-Blockierung**: Werden nicht erforderliche Skripte eingeschränkt oder kontrolliert? | Teilweise | Keine automatische Skript-Blockierung vorhanden; Einsatz von Tools wie NoScript/Ghostery empfohlen. |
| 4 | **Automatische Löschung von Caches & Verlauf**: Gibt es Richtlinien zur automatischen Bereinigung von Sitzungsdaten? | Nicht erfüllt | Caches und Verlauf bleiben unbegrenzt gespeichert. Automatische Löschregeln einrichten. |
| 5 | **Isolierung von Nutzungskontexten**: Werden datenintensive Dienste (z. B. Social Media) isoliert betrieben? | Teilweise | Keine strikte Containering-Pflicht (z. B. Facebook Container); Sensibilisierung der Nutzer erforderlich. |

### Reflexion zu Checkliste 2
Die Analyse der technischen und organisatorischen Schutzmassnahmen zeigt, dass der Schutz vor Webtracking stark von einer Kombination aus serverseitigen Einstellungen und benutzerseitigem Verhalten abhängt. Während serverseitig oft die notwendigen Vorkehrungen fehlen (z. B. automatische Löschfristen oder DNT-Unterstützung), müssen Anwendende zusätzliche Tools wie Tracker-Blocker einsetzen. Überrascht hat mich, wie effektiv einfache technische Massnahmen wie Container-Plugins sein können, um browserübergreifendes Tracking wirksam einzudämmen.

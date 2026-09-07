# M231 Lernjournal
### Ylli Uka
### PE26a
### Tag 4
### 07.09.26
**Mein LB1-Ergebnis:** 7.04 / 10.00 Punkte (in nur 2.5 Minuten)

---

## Was wir heute gelernt haben 

*   **Lizenzen & Urheberrecht:** Wer Code schreibt oder Fotos macht, bestimmt die Regeln. **Proprietär** (wie Windows) kostet meistens und der Code bleibt geheim . **Open Source** (OSS) ist gratis und jeder darf den Code sehen und anpassen.
*   **Tracking & Fingerprinting:** Webseiten spionieren uns voll aus [4]. Nicht nur mit Cookies, sondern auch mit **Fingerprinting** – die checken deine Auflösung, Schriftarten und Co. ab, um dich ohne Cookies wiederzuerkennen.
*   **Dark Patterns:** Das sind fiese Design-Tricks auf Webseiten, die uns austricksen wollen . Zum Beispiel, um uns heimlich Geld aus der Tasche zu ziehen oder uns Abos anzudrehen .

---

## Gelöste Aufgaben

### 1. Lizenzen zuordnen [10]
*   Schulprojekt (frei für alle, mit Namensnennung) -> **CC BY** 
*   Firma teilt Code (will Änderungen nicht zwingend zurück) -> **MIT** 
*   Fotograf teilt Bilder (kein Kommerz, keine Bearbeitung) -> **CC BY-NC-ND** 
*   Code-Bibliothek für eigene Kauf-Software -> **LGPL** 

### 2. Mein Fingerprint-Test (Cover Your Tracks) 
Ich habe meinen Browser getestet:
*   **Ad-Blocker:** Läuft, blockiert alles!
*   **Fingerprint-Schutz:** Richtig stabil, weil mein Browser den Fingerprint ständig **zufällig verändert** (randomisiert).
*   **Infos:** Hat trotzdem noch **18.3 Bits** an Infos rausgegeben (wegen Zeitzone, Sprache etc. – das kann man fast nicht blockieren).

### 3. Dark Patterns auf echten Webseiten gefunden 

*   **MediaMarkt (PC-Suche):**
    *   *Trick:* **Disguised Ads** (Getarnte Werbung) & **Misdirection** (Ablenkung) .
    *   *Warum:* Das erste Produkt ist eigentlich nur Werbung ("Gesponsert"), sieht aber exakt so aus wie ein normales Suchergebnis . Man übersieht das "Gesponsert" voll, weil daneben ein fetter rote Rabatt-Sticker (**-31%**) einen voll ablenkt.
*   **Galaxus (Sofa-Suche):**
    *   *Trick:* **Urgency / Scarcity** (Künstlicher Stress) .
    *   *Warum:* Da steht fett in Orange **"nur noch 1 Stück im Sale"** . Das macht einem voll Druck im Kopf, damit man schnell zuschlägt, ohne vorher woanders die Preise zu vergleichen .

---

## Was ich heute persönlich gelernt habe (Mein Fazit)

*   **Ich bin jetzt schlauer beim Shoppen:** Ich weiss jetzt, dass diese "Nur noch 1 Stück"-Meldungen oft nur Tricks sind Ich lass mich da nicht mehr stressen.
*   **Werbung wird immer fieser getarnt:** Dass sich Werbung so krass als echtes Suchergebnis tarnt, ist echt unverschämt Da muss man echt zweimal hinschauen.
*   **Man ist nie ganz unsichtbar im Netz:** Selbst mit guten Blockern schickt der Browser wegen Zeitzone und Co. immer noch kleine Infos mit  Aber immerhin erschweren wir es den Trackern maximal!
  




*   ## Bilder/Inhalt:



```mermaid 
mindmap
  root((Lizenzmodelle im Überblick))
    (Urheberrecht)
      [Das Recht das automatisch entsteht wenn man etwas erschafft]
      [Zum Beispiel ein Text ein Bild oder ein Programm]
      [Andere dürfen es nur nutzen wenn man es erlaubt]
    (Proprietäre Software)
      [Das bedeutet die Firma zeigt den Bauplan nicht]
      [Man darf es nur so nutzen wie es der Vertrag erlaubt]
      [Dieser Vertrag heisst EULA]
      [EULA ausgeschrieben End User License Agreement]
      [Das heisst auf Deutsch Endnutzer Lizenzvertrag]
      [Man darf es meist nicht einfach weitergeben]
      {{Microsoft Office}}
      {{Adobe Photoshop}}
      {{macOS}}
    (Open Source Software)
      [Kurz auch OSS genannt]
      [Ausgeschrieben Open Source Software]
      [Das heisst auf Deutsch offener Quellcode]
      [Jeder darf den Bauplan der Software sehen]
      [Meist kostenlos auch für Firmen nutzbar]
      [Weitergabe ist erlaubt aber jede Lizenz hat eigene Regeln]
    (Copyleft)
      [Eine wichtige Regel bei manchen Lizenzen]
      [Wer die Software verändert muss seine Änderung wieder offenlegen]
      [So bleibt die Software für immer frei zugänglich]
    (MIT Lizenz)
      [Benannt nach der amerikanischen Universität MIT]
      [Die einfachste und lockerste Lizenz]
      [Fast keine Regeln man darf fast alles damit machen]
      [Hat kein Copyleft]
      {{VS Code}}
    (Apache Lizenz)
      [Die Zahl 2 Punkt 0 ist nur die Versionsnummer]
      [Ähnlich locker wie MIT]
      [Hat kein Copyleft]
      [Schützt zusätzlich davor dass man wegen Patenten verklagt wird]
      {{Android}}
    (GPL)
      [Ausgeschrieben General Public License]
      [Das heisst auf Deutsch Allgemeine Öffentliche Lizenz]
      [Die Zahl 3 ist nur die Versionsnummer]
      [Hat ein starkes Copyleft]
      [Wenn man den Code verändert muss man es unter der gleichen Lizenz teilen]
      {{Linux Kernel}}
    (LGPL)
      [Ausgeschrieben Lesser General Public License]
      [Das heisst auf Deutsch etwa Kleinere Allgemeine Öffentliche Lizenz]
      [Eine abgeschwächte Version der GPL]
      [Gedacht für kleine Programmteile die andere Programme mitbenutzen]
      [Man darf sie einbauen ohne dass das ganze Programm auch GPL wird]
      {{LibreOffice}}
    (AGPL)
      [Ausgeschrieben Affero General Public License]
      [Fast wie GPL]
      [Der Unterschied gilt auch wenn man die Software nur über das Internet nutzt]
      [Zum Beispiel bei einer Webseite oder einem Online Dienst]
      {{Nextcloud}}
```


## Dark Patterns

Dark Patterns sind **Gestaltungstricks in Benutzeroberflächen**, die Nutzer zu einer Handlung verleiten, die sie nicht wollten oder beabsichtigt hätten.

### Wie Dark Patterns Entscheidungen manipulieren

```mermaid
flowchart TD
  A["Nutzer interagiert\nmit Interface"]
  B{"Dark Pattern\nvorhanden?"}
  C["Informierte\nEntscheidung\nmöglich"]
  D["Nutzer verwirrt,\nunter Druck gesetzt\noder irregeführt"]
  E["Unbeabsichtigte Handlung\n(Kauf, Abo, Datenweitergabe)"]
  F["Unternehmensgewinn\nauf Kosten des Nutzers"]
  G["Nutzer bemerkt es (oft)\nerst später"]

  A --> B
  B -- "Nein" --> C
  B -- "Ja" --> D
  D --> E
  E --> F
  F --> G
  G -- "Beschwerde / Rückgabe\noft nicht möglich" --> F
```

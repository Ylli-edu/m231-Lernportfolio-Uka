# M231 Lernjournal

### Ylli Uka

### PE26a

### Tag 8

### 26.10.26

---

## 1. Kurzer Einstieg: CIA-Prinzip (Repetition)

Am Anfang haben wir die drei Schutzziele kurz wiederholt:
* **Confidentiality (Vertraulichkeit):** Nur Berechtigte dürfen Daten lesen (z. B. via Verschlüsselung & Passwörter).
* **Integrity (Integrität):** Daten dürfen nicht unbemerkt verändert werden (z. B. via Hashes & Signaturen).
* **Availability (Verfügbarkeit):** Daten und Systeme müssen da sein, wenn man sie braucht (z. B. via Backups).

---

## 2. Arbeitsblatt: Risikomanalyse KMU (Aufgabe B)

**Szenario:** 15 Mitarbeitende, lokaler Server ohne Backup, Homeoffice über ungesichertes WLAN, alle teilen sich denselben Admin-Account.

| Nr. | Risiko / Bedrohung | Wahrscheinlichkeit | Ausmass | Strategie | Konkrete Massnahme |
|:---:|---|:---:|:---:|:---:|---|
| **R1** | **Datenverlust Server-Defekt** (kein Backup) | Hoch | Hoch | Vermindern | **3-2-1-Backup** einrichten. |
| **R2** | **Datenabfluss via WLAN** (Homeoffice) | Hoch | Hoch | Vermindern | **VPN-Pflicht** mit Verschlüsselung. |
| **R3** | **Admin-Passwort kompromittiert** (Shared Login) | Hoch | Kritisch | Vermindern | Eigene Konten + **MFA** + **Least Privilege**. |
| **R4** | **Ransomware-Befall** (Betriebsstillstand) | Mittel | Kritisch | Vermindern | **Offline-Backup**, Updates & Antivirus. |

* **Höchste Priorität:** **R3** und **R1**, da ohne Backup sofort alles weg ist und ein geteiltes Passwort keine Nachvollziehbarkeit bietet.

---

## 3. Praktische Umsetzung: GPG mit Kleopatra (Aufgabe C)

Unter Windows mit **Gpg4win / Kleopatra**:
1. **Schlüsselpaar erstellt:** Eigenes OpenPGP-Schlüsselpaar mit Name, E-Mail und Passphrase generiert.
2. **Public Key exportiert:** Als `.asc`-Datei gespeichert und an Herr Gassmann gemailt.
3. **Key von Herr Gassmann importiert:** Seinen öffentlichen Schlüssel in Kleopatra geladen und beglaubigt (`trust`).
4. **Nachricht verschlüsselt & signiert:** Nachricht mit seinem Public Key verschlüsselt, mit meinem Private Key signiert und die verschlüsselte Datei per Mail an ihn geschickt.

---

## 4. Was habe ich heute gelernt?

* **CIA in echt:** Sicherheit ist nicht nur Geheimhaltung, sondern vor allem Verfügbarkeit (Backups!).
* **Risiko-Formel:** $\text{Risiko} = \text{Wahrscheinlichkeit} \times \text{Ausmass}$ hilft beim Priorisieren von Massnahmen.
* **Das Schloss-Prinzip (GPG):** Der Public Key ist ein offenes Vorhängeschloss, das man jedem geben kann. Nur der Empfänger hat den passenden Private Key zum Aufsperren.
* **Persönliches Fazit:** Mit der App Kleopatra war es einfach. Sicherheit crasht fast nie an der Technik, sondern an Bequemlichkeit (wie 15 Leute mit einem Passwort).

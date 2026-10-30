# M231 Lernjournal

### Ylli Uka

### PE26a

### Tag 7

### 19.10.26
---

## Verschlüsselungsverfahren



```mermaid
---
title: Symmetrische Verschlüsselung 
---
flowchart LR
    A["Sender (Alice)"] -- "1. Klartext" --> V["Verschlüsselung"]
    K["🔑 Geheimer Schlüssel (K)\n(Gemeinsamer Schlüssel)"] -.-> V
    V -- "2. Geheimtext" --> N["Unsicheres Netzwerk"]
    N -- "3. Geheimtext" --> E["Entschlüsselung"]
    K -.-> E
    E -- "4. Klartext" --> B["Empfänger (Bob)"]
```

```mermaid
---
title: Asymmetrische Verschlüsselung
---
flowchart LR
    A["Sender (Alice)"] -- "1. Klartext" --> V["Verschlüsselung"]
    PUB["🔑 Bobs Public Key\n(Öffentlich)"] -.-> V
    V -- "2. Geheimtext" --> N["Netzwerk"]
    N -- "3. Geheimtext" --> E["Entschlüsselung"]
    PRIV["🔑 Bobs Private Key\n(Geheim)"] -.-> E
    E -- "4. Klartext" --> B["Empfänger (Bob)"]
```




## Integritätsprüfung mit PowerShell (Hashwerte)

### **Erklärung & Ziel**
Um sicherzustellen, dass eine Datei bei der Übertragung nicht verändert oder beschädigt wurde (**Integritätsprüfung**), wird ein kryptografischer **Hashwert** (Fingerabdruck) berechnet. Ändert sich die Datei auch nur minimal, verändert sich der Hashwert komplett.

### **1. Durchführung**
In der Windows PowerShell wurde der MD5-Hashwert für die Datei `Gebäudeplan.png` ermittelt:

```powershell
Get-FileHash "C:\Users\yiua\Downloads\Gebäudeplan.png" -Algorithm MD5
```

**Ausgabe / Ergebnis:**
* **Algorithmus:** MD5
* **Hash-Wert:** `95ADEF958BB3081AAD876D55B0F6357D`
* **Datei-Pfad:** `C:\Users\yiua\Downloads\Gebäudeplan.png`




<img width="1732" height="407" alt="Screenshot 2026-10-19 144749" src="https://github.com/user-attachments/assets/aa98d5d7-e6da-4af2-800e-ea71b6ec2283" />

---
### **2. Durchführung**
In der Windows PowerShell wurde der MD5-Hashwert für die Datei `Hallo.vbs` ermittelt:
Get-FileHash "C:\Users\yiua\OneDrive - Bellini Personal AG\Desktop\hallo.vbs" -Algorithm MD5

**Ausgabe / Ergebnis:**

* **Algorithmus:** MD5
* **Hash-Wert:** FB888618B9B15712532FD36B33C5C14A
* **Datei-Pfad:** C:\Users\yiua\OneDrive - Bellini Personal AG\Desktop\hallo.vbs
<img width="1094" height="119" alt="Screenshot 2026-10-30 092013" src="https://github.com/user-attachments/assets/162ce580-2416-4f0b-bb62-83c30259fd16" />






# Was habe ich heute gelernt?

* **Symmetrische Verschlüsselung:** Ein gemeinsamer Schlüssel für Ver- und Entschlüsselung (schnell, aber Schlüsselaustausch ist schwierig).
* **Asymmetrische Verschlüsselung:** Schlüsselpaar aus Public Key (zum Verschlüsseln) und Private Key (zum Entschlüsseln).
* **Hashwerte (PowerShell):** Überprüfung der Datei-Integrität mittels `Get-FileHash` (z. B. MD5 / SHA256).
* **Lernjournal-Review mit Linus Gätzi:** Erfolgreich erledigt! Wir eide hatten ein gutes strukturiertes Journal.

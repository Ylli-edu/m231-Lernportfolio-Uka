# M231

## Tag 2

### Was habe ich heute gemacht?
Heute haben wir einen **Quiz** über die letzte Woche gemacht.  
Danach erstellten wir in einer Gruppe eine Tabelle zum **Spaghetti kochen** und benutzen **Mermaid.live** um ein Diagramm zu erstellen.  
Zum Schluss lernten wir etwas über **Datenschutzgesetz** in der EU und der Schweiz.  
Danach mussten wir in den gleichen Gruppen eine **PPT** darüber machen.

---

### Notizen zum revidierten Datenschutzgesetz (revDSG) (Notizen von anderen PPT's)

#### Die 5 Grundsätze:
1. **Rechtmässigkeit:** Ohne Einwilligung Daten nicht an dritte Personen abgeben, ausser es liegen rechtliche Gründe vor.
2. **Verhältnismässigkeit:** Daten nur so lange behalten, wie man sie braucht. Danach müssen sie gelöscht werden.
3. **Zweckbindung:** Die Person muss wissen, wieso man ihre Daten braucht.
4. **Richtigkeit:** Die Daten müssen richtig und aktuell (neu) sein.
5. **Datensicherheit:** Die Daten müssen gut gesichert sein.

#### Schutz der Personendaten:
*   **Öffentliche Daten:** z. B. Namen
*   **Interne Daten:** z. B. Handyfotos
*   **Vertrauliche Daten:** z. B. Lohnangaben und Krankheitsdaten
*   **Geheime Daten:** z. B. Passwörter

#### Wenn das Gesetz gebrochen wird (Konsequenzen):
*   **Geldbusse:** Bis zu 250'000 CHF
*   **Firmenbusse:** Bis zu 50'000 CHF
*   **Haftstrafe**
*   **Schadenersatz**









Code:

```mermaid
flowchart TB
    A(["🍝 Spaghetti kochen"]) --> B["Wasser in einen großen Topf geben"]
    B --> C["Salz hinzufügen"]
    C --> D["Wasser zum Kochen bringen"]
    D --> E["Spaghetti vorsichtig ins Wasser legen"]
    E --> F["Nach Packungsangabe kochen<br>gelegentlich umrühren"]
    F --> G{"Sind die Spaghetti<br>al dente?"}
    G -- Nein --> F
    G -- Ja --> H["Spaghetti abgießen"]
    H --> I["Etwas Kochwasser auffangen"]
    I --> J["Evt. mit Sauce vermischen"]
    J --> K(["🍽️ Servieren und genießen"])

     A:::start
     B:::prep
     C:::prep
     D:::prep
     E:::cook
     F:::cook
     G:::check
     H:::finish
     I:::finish
     J:::finish
     K:::start
    classDef start fill:#fff7ed,stroke:#fb923c,stroke-width:3px,color:#7c2d12
    classDef prep fill:#eef2ff,stroke:#818cf8,stroke-width:2px,color:#312e81
    classDef cook fill:#f0fdfa,stroke:#2dd4bf,stroke-width:2px,color:#134e4a
    classDef check fill:#fefce8,stroke:#facc15,stroke-width:2px,color:#713f12
    classDef finish fill:#f0fdf4,stroke:#4ade80,stroke-width:2px,color:#14532d
```

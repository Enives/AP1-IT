# Netzpläne mit Vorgängen und Abhängigkeiten

## 1. Einführung
Ein **Netzplan** ist ein grafisches Werkzeug zur Planung, Steuerung und Überwachung von Projekten. Er zeigt:
- **Vorgänge** (Aktivitäten oder Aufgaben),
- **Abhängigkeiten** (Reihenfolgebeziehungen zwischen Vorgängen),
- **Zeitliche Planung** (Start- und Endtermine).

---

## 2. Grundbegriffe
### Vorgänge (Aktivitäten)
- **Beschreibung**: Eine Aufgabe oder ein Arbeitsschritt im Projekt.
- **Dauer**: Zeit, die für die Durchführung benötigt wird (z. B. in Tagen oder Wochen).
- **Beispiel**: "Material beschaffen" (Dauer: 2 Tage).

### Abhängigkeiten
- **Beschreibung**: Logische Beziehungen zwischen Vorgängen.
- **Typen**:
  1. **Ende-Start (ES)**: Vorgang B kann erst beginnen, wenn Vorgang A abgeschlossen ist.
  2. **Start-Start (SS)**: Vorgang B kann erst beginnen, wenn Vorgang A begonnen hat.
  3. **Ende-Ende (EE)**: Vorgang B kann erst enden, wenn Vorgang A abgeschlossen ist.
  4. **Start-Ende (SE)**: Vorgang B kann erst enden, wenn Vorgang A begonnen hat.

### Ereignisse (Knoten)
- **Beschreibung**: Zeitpunkte, die den Beginn oder das Ende von Vorgängen markieren.
- **Beispiel**: "Projektstart" oder "Material beschafft".

---

## 3. Erstellung eines Netzplans
### Schritte:
1. **Vorgänge identifizieren**: Alle Aufgaben im Projekt auflisten.
2. **Abhängigkeiten festlegen**: Beziehungen zwischen den Vorgängen definieren.
3. **Dauern schätzen**: Zeitbedarf für jeden Vorgang ermitteln.
4. **Netzplan zeichnen**: Vorgänge und Abhängigkeiten grafisch darstellen.

### Beispiel:
| **Vorgang**         | **Dauer** | **Vorgänger** |
|---------------------|-----------|---------------|
| A: Material beschaffen | 2 Tage  | –             |
| B: Material prüfen   | 1 Tag     | A             |
| C: Produktion starten | 3 Tage   | B             |

---

## 4. Darstellungsmethoden
### 1. **Vorgangsknotennetzplan (AON)**
- **Vorgänge** werden als **Knoten** dargestellt.
- **Abhängigkeiten** werden als **Pfeile** zwischen den Knoten gezeigt.

[A] --> [B] --> [C]

### 2. **Vorgangspfeilnetzplan (AOA)**
- **Vorgänge** werden als **Pfeile** dargestellt.
- **Ereignisse** (Knoten) markieren den Beginn und das Ende von Vorgängen.

(Start) --> A --> (Ereignis 1) --> B --> (Ereignis 2) --> C --> (Ende)

---

## 5. Kritischer Pfad
- **Definition**: Die längste Abfolge von Vorgängen im Netzplan, die die Gesamtprojektdauer bestimmt.
- **Eigenschaften**:
  - Verzögerungen auf dem kritischen Pfad verzögern das gesamte Projekt.
  - Vorgänge auf dem kritischen Pfad haben keine Pufferzeit.

### Beispiel:
- **Kritischer Pfad**: A → B → C (Gesamtdauer: 6 Tage).

---

## 6. Pufferzeiten
- **Gesamtpuffer**: Zeit, um die ein Vorgang verschoben werden kann, ohne den Projektendtermin zu gefährden.
- **Freier Puffer**: Zeit, um die ein Vorgang verschoben werden kann, ohne nachfolgende Vorgänge zu beeinflussen.

### Formel:
$\text{Gesamtpuffer} = \text{spätester Endtermin} - \text{frühester Endtermin}$

---

## 7. Praxisbeispiel: Bauprojekt
### Vorgänge:
| **Vorgang**         | **Dauer** | **Vorgänger** |
|---------------------|-----------|---------------|
| A: Fundament gießen | 5 Tage    | –             |
| B: Wände errichten  | 7 Tage    | A             |
| C: Dach decken      | 3 Tage    | B             |
| D: Elektrik installieren | 2 Tage | B             |

### Netzplan:
[A] --> [B] --> [C] --> [D]

### Kritischer Pfad:
A → B → C (Gesamtdauer: 15 Tage).

---

## 8. Fazit
Netzpläne sind ein **wichtiges Werkzeug** im Projektmanagement, um:
- Abhängigkeiten zwischen Vorgängen zu visualisieren,
- Den kritischen Pfad zu identifizieren,
- Ressourcen und Zeit effizient zu planen.

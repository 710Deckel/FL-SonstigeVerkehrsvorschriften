# 📚 FL-SonstigeVerkehrsvorschriften - Sonstige Verkehrsvorschriften Editor

**Fahrlehrer-Ausbildung FL-BE_07/25**  
Justin Lee Probis

---

## 📚 Über dieses Repository

Dieses Repository enthält die Daten für den **Sonstige Verkehrsvorschriften Editor** - ein professionelles Werkzeug zur systematischen Aufbereitung weiterer verkehrsrelevanter Gesetze und Verordnungen für die Fahrlehrer-Ausbildung.

Der Editor ermöglicht die strukturierte Erfassung von Gesetzestexten zu EG-Fahrgenehmigungen, Arbeitszeiten und Elektrokleinstfahrzeugen sowie deren Synchronisation über GitHub.

---

## 📂 Repository-Struktur

```
FL-SonstigeVerkehrsvorschriften/
├── README.md       (diese Datei - Projektbeschreibung)
└── data.json       (Sonstige-Daten, automatisch synchronisiert vom Editor)
```

---

## 📋 Enthaltene Gesetze & Verordnungen

Dieses Tool vereint weitere wichtige Verkehrsvorschriften in einem Editor:

- **EG-FGV** - EG-Fahrgenehmigungsverordnung (Taxi, Mietwagen)
- **ArbZG** - Arbeitszeitgesetz (verkehrsrelevante Teile)
- **eKFV** - Elektrokleinstfahrzeug-Verordnung (E-Scooter, etc.)
- **Sonstiges** - Platzhalter für weitere Vorschriften

---

## 🔄 Daten-Synchronisation

Die Datei `data.json` wird **automatisch** vom Sonstige Verkehrsvorschriften Editor synchronisiert:

- ✅ Jedes Speichern im Editor aktualisiert diese Datei
- ✅ Änderungen werden mit Zeitstempel versioniert
- ✅ Team-Kollaboration möglich (mehrere Nutzer, ein Repository)

**⚠️ WICHTIG:** Die `data.json` sollte **nicht manuell bearbeitet** werden!  
Alle Änderungen bitte nur über den Sonstige Verkehrsvorschriften Editor vornehmen.

---

## 🛠️ Verwendung

### 1. Repository-Setup (einmalig)
- Repository erstellt: ✅ `710Deckel/FL-SonstigeVerkehrsvorschriften`
- README.md hochgeladen: ✅

### 2. Editor-Verwendung
- HTML-Datei lokal öffnen (`sonstige-verkehrsvorschriften-editor.html`)
- GitHub Token eingeben (einmalig, gleicher Token wie andere Tools!)
- Gesetz aus Dropdown auswählen (EG-FGV, ArbZG, eKFV, Sonstiges)
- Paragraphen hinzufügen und speichern
- Automatische Synchronisation erfolgt

### 3. Token-Anforderungen
Der verwendete Token benötigt folgende Berechtigungen:
- ✅ `repo` (Full control of private repositories)

**Hinweis:** Du kannst denselben Token für alle Fahrlehrer-Tools verwenden!

---

## 📋 Datenstruktur

Die `data.json` enthält alle Paragraphen aus allen Gesetzen im folgenden Format:

```json
{
  "paragraphen": [
    {
      "id": "timestamp",
      "gesetz": "EG-FGV",
      "nummer": "§ 1",
      "titel": "Geltungsbereich",
      "gesetzestext": "...",
      "quelle": "https://...",
      "praxisbeispiele": [
        {
          "titel": "Beispiel",
          "klasse": "ALLE",
          "beschreibung": "...",
          "wichtigkeit": "CRITICAL"
        }
      ]
    }
  ]
}
```

---

## 🎯 Features des Editors

- **2-Spalten-Layout:** Gesetzestext | Praxisbeispiele
- **Gesetz-Auswahl:** Dropdown für EG-FGV, ArbZG, eKFV, Sonstiges
- **GitHub Auto-Sync:** Automatische Synchronisation
- **Template-System:** Vordefinierte Beispiele
- **Badge-System:** CRITICAL (rot) | HIGH (orange) | BANAL (grün)
- **PDF-Export:** Professionelle Druckausgabe
- **Import/Export:** JSON-Backup-System
- **Keyboard Shortcuts:** Strg+S zum Speichern
- **Teal Theme:** Speziell für sonstige Vorschriften

---

## 📚 Wichtige Bereiche

**EG-FGV (EG-Fahrgenehmigungsverordnung):**
- Taxi-Genehmigungen
- Mietwagen-Regelungen
- Personenbeförderung im Kleingewerbe

**ArbZG (Arbeitszeitgesetz):**
- Arbeitszeiten für Berufskraftfahrer
- Ruhepausen und Ruhezeiten
- Sonntagsfahrverbote

**eKFV (Elektrokleinstfahrzeug-Verordnung):**
- E-Scooter Zulassung
- Versicherungspflicht
- Verkehrsregeln für Elektrokleinstfahrzeuge

---

## 🔗 Weitere Fahrlehrer-Tools

Dieses Repository ist Teil einer systematischen Tool-Suite für die Fahrlehrer-Ausbildung:

- [📘 FL-StVO](https://github.com/710Deckel/stvo-teleprompter) - StVO Teleprompter
- [🚛 FL-FPersV-EG-VO](https://github.com/710Deckel/FL-FPersV-EG-VO) - Fahrpersonalverordnung & EU-Verordnung
- [⚖️ FL-StVG](https://github.com/710Deckel/FL-StVG) - Straßenverkehrsgesetz
- [🔧 FL-StVZO](https://github.com/710Deckel/FL-StVZO) - Straßenverkehrs-Zulassungs-Ordnung
- [📋 FL-FeV](https://github.com/710Deckel/FL-FeV) - Fahrerlaubnis-Verordnung
- [🚗 FL-FZV](https://github.com/710Deckel/FL-FZV) - Fahrzeug-Zulassungsverordnung
- [👨‍🏫 FL-FahrlehrerGesetze](https://github.com/710Deckel/FL-FahrlehrerGesetze) - Fahrlehrer-Gesetze (erweitert)
- [⚖️ FL-VerkehrsrechtStrafrecht](https://github.com/710Deckel/FL-VerkehrsrechtStrafrecht) - Verkehrsrecht & Strafrecht (erweitert)
- [📝 FL-Pruefungsrichtlinie](https://github.com/710Deckel/FL-Pruefungsrichtlinie) - Prüfungsrichtlinie Kfz
- [📚 FL-SonstigeVerkehrsvorschriften](https://github.com/710Deckel/FL-SonstigeVerkehrsvorschriften) - Sonstige Verkehrsvorschriften (dieses Repository)

---

## 📝 Lizenz & Verwendung

**Projekt:** Fahrlehrer-Ausbildung FL-BE_07/25  
**Ersteller:** Justin Lee Probis  
**Zweck:** Ausbildung und Podcast "Fahrlehrer Inside"

Dieses Tool und die Daten sind für **Ausbildungszwecke** erstellt.

---

## 📞 Kontakt & Feedback

Bei Fragen, Problemen oder Verbesserungsvorschlägen:
- GitHub Issues in diesem Repository
- Feedback über das Tool (Thumbs Down Button)

---

**Erstellt mit ❤️ für die Fahrlehrer-Ausbildung**

*Letzte Aktualisierung: Dezember 2024*

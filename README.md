# Mission Control Dashboard — CoderXP

## Projektübersicht

Das Mission Control Dashboard ist eine webbasierte Oberfläche zur Verwaltung und Überwachung autonomer KI-Agenten. Es ermöglicht die zentrale Steuerung von bis zu 10 Agenten, die verschiedene Aufgaben im Software-Entwicklungsprozess übernehmen.

## Funktionen

### Kernfunktionen

- **Agenten-Verwaltung**: Übersicht und Steuerung von bis zu 10 autonomen KI-Agenten
- **Echtzeit-Monitoring**: Live-Anzeige von Fortschritt, Ressourcennutzung und Systemstatus
- **API-Konfiguration**: Individuelle API-Endpunkte, Authentifizierung und Keys pro Agent
- **Prompt-Management**: Benutzerdefinierte Prompts für jeden Agenten mit Variablen-Unterstützung
- **Aufgabenplanung**: Zeitgesteuerte Ausführung von Agenten-Aufgaben
- **Aktivitäts-Logs**: Detaillierte Protokollierung aller Agenten-Aktionen
- **Team-Chat**: Direkte Kommunikation mit einzelnen Agenten

### Dashboard-Bereiche

1. **Missionskontrolle**: Hauptansicht mit Orchestrator-Panel und Agenten-Grid
2. **Überwachung**: Systemmetriken, Performance-Charts und Orchestrierungs-Logs
3. **Build-Zentrum**: CI/CD-Pipeline-Status und Deployment-Informationen
4. **Agenten**: Erweiterte Verwaltungsoberfläche für alle Agenten
5. **Daten# Mission Control Dashboard — CoderXP

## Projektübersicht

Das Mission Control Dashboard ist eine webbasierte Oberfläche zur Verwaltung und Überwachung autonomer KI-Agenten. Es ermöglicht die zentrale Steuerung von bis zu 10 Agenten, die verschiedene Aufgaben im Software-Entwicklungsprozess übernehmen.

## Funktionen

### Kernfunktionen

- **Agenten-Verwaltung**: Übersicht und Steuerung von bis zu 10 autonomen KI-Agenten
- **Echtzeit-Monitoring**: Live-Anzeige von Fortschritt, Ressourcennutzung und Systemstatus
- **API-Konfiguration**: Individuelle API-Endpunkte, Authentifizierung und Keys pro Agent
- **Prompt-Management**: Benutzerdefinierte Prompts für jeden Agenten mit Variablen-Unterstützung
- **Aufgabenplanung**: Zeitgesteuerte Ausführung von Agenten-Aufgaben
- **Aktivitäts-Logs**: Detaillierte Protokollierung aller Agenten-Aktionen
- **Team-Chat**: Direkte Kommunikation mit einzelnen Agenten

### Dashboard-Bereiche

1. **Missionskontrolle**: Hauptansicht mit Orchestrator-Panel und Agenten-Grid
2. **Überwachung**: Systemmetriken, Performance-Charts und Orchestrierungs-Logs
3. **Build-Zentrum**: CI/CD-Pipeline-Status und Deployment-Informationen
4. **Agenten**: Erweiterte Verwaltungsoberfläche für alle Agenten
5. **Daten-Tool**: Analyse von Aufgaben-Abschlussraten und Performance-Kennzahlen
6. **KI-Labor**: Experimentelle Tools für Modell-Training und Prompt-Engineering
7. **Logs**: Vollständige Audit-Protokolle aller Systemereignisse
8. **Projekte**: Verwaltung mehrerer Coding-Projekte mit eigenem Agenten-Setup
9. **Einstellungen**: Anpassung von UI-Präferenzen und Systemverhalten

## Technische Implementierung

### Frontend-Technologien

- HTML5, CSS3, Vanilla JavaScript
- Google Fonts: Orbitron, Rajdhani, Share Tech Mono
- Canvas API für Chart-Visualisierungen
- CSS Custom Properties für theming
- Responsive Design mit Mobile-First-Ansatz

### Datenstruktur

Jeder Agent wird durch ein JavaScript-Objekt repräsentiert:

```javascript
{
  id: Number,
  name: String,
  role: String,
  status: 'active' | 'ready' | 'inactive',
  progress: Number, // 0-100
  task: String,
  apiEndpoint: String,
  authType: 'none' | 'bearer' | 'apikey' | 'basic',
  apiKey: String,
  customPrompt: String,
  logs: Array<{ time: String, level: String, msg: String }>,
  cpu: Number,
  mem: Number,
  net: Number
}
```

## Installation und Nutzung

### Lokale Ausführung

1. Speichern Sie den HTML-Code als `index.html`
2. Öffnen Sie die Datei in einem modernen Browser (Chrome, Firefox, Edge)
3. Keine Server-Konfiguration erforderlich

### Browser-Anforderungen

- JavaScript aktiviert
- Unterstützung für CSS Grid und Flexbox
- Canvas API für Chart-Darstellungen
- Empfohlene Auflösung: 1280x720 oder höher

## Konfiguration

### API-Einrichtung pro Agent

1. Öffnen Sie das Detail-Modal eines Agenten
2. Tragen Sie im Bereich "API-Konfiguration" ein:
   - API-Endpunkt (vollständige URL)
   - Authentifizierungstyp (Keine, Bearer Token, API Key, Basic Auth)
   - API-Schlüssel oder Token
3. Speichern Sie mit "Konfiguration speichern"

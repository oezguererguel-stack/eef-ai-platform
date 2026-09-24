# Architektur – EEF AI v1

## Zielbild

EEF AI wird als modulares System aufgebaut. Ein zentraler Master-Agent koordiniert spezialisierte Agenten und greift über definierte Tools auf Website, Datenbank, Dokumente und Kommunikationssysteme zu.

## Komponenten

### Master Agent
- versteht Nutzeraufträge
- delegiert an Spezialagenten
- führt keine sensiblen externen Aktionen ohne Freigabe aus

### E-Mail Agent
- klassifiziert eingehende Nachrichten
- erkennt Kunde, Projekt, Priorität und Fristen
- erstellt Antwortentwürfe
- versendet nur nach definierter Freigaberegel

### CRM Agent
- verwaltet Kunden, Projekte, Ansprechpartner, Aufgaben und Wiedervorlagen
- erzeugt Statusübersichten

### Dokument Agent
- erstellt Entwürfe für Angebote, Verträge, NDAs, Rechnungen und Anschreiben
- nutzt freigegebene Vorlagen

### Website Agent
- prüft Inhalte, Links und Aktualität
- erstellt Änderungsvorschläge
- veröffentlicht nur nach Freigabe

### Research Agent
- recherchiert aktuelle externe Informationen
- trennt Quellenmaterial von internen Unternehmensdaten

## Technischer Stack

- KI: OpenAI API / Agents SDK
- Automatisierung: n8n
- Datenbank: PostgreSQL
- Website/CMS: WordPress mit REST API oder entkoppeltes Frontend
- Dokumente: externer Dokumentenspeicher
- Versionsverwaltung: GitHub

## Datenfluss

Nutzeranfrage → Master Agent → Spezialagent → Daten/Tools → Entwurf/Ergebnis → Freigabe → externe Aktion

## Trennung von Code und Geschäftsdaten

Im Repository liegen ausschließlich Code, Konfiguration ohne Geheimnisse, Datenbankschemata und technische Dokumentation. Kunden- und Projektdaten werden in dafür vorgesehenen Speichern verarbeitet.

# Sicherheitsmodell

## Freigabestufen

### Grün – automatisch zulässig
- lesen
- klassifizieren
- interne Zusammenfassungen
- Status aktualisieren
- Entwürfe erzeugen

### Gelb – kontrollierter Entwurf
- E-Mail-Antwort vorbereiten
- Dokument erstellen
- Website-Änderung vorbereiten
- CRM-Folgeaktion vorschlagen

### Rot – menschliche Freigabe erforderlich
- externe E-Mail versenden
- Website veröffentlichen
- Verträge final ändern
- sensible Kundendaten weitergeben
- Bank- oder Finanzierungskommunikation versenden
- produktive Daten löschen

## Geheimnisse

API-Schlüssel, Passwörter, Tokens und Zugangsdaten gehören ausschließlich in Secret Stores bzw. Umgebungsvariablen.

Nie committen:
- `.env`
- API Keys
- Datenbankpasswörter
- OAuth Tokens
- Kundendokumente
- Ausweiskopien
- Bankunterlagen

## Datenschutz

- Datenminimierung
- zweckgebundene Verarbeitung
- rollenbasierte Zugriffe
- Protokollierung sensibler Aktionen
- definierte Lösch- und Aufbewahrungsregeln
- getrennte Entwicklungs- und Produktivumgebung

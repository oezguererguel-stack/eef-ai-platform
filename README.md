# EEF AI Platform

Zentrale technische Basis für die digitale EEF-Plattform.

## Ziel

Die Plattform soll Website, KI-Assistenten, Automationen, CRM-nahe Datenstrukturen und Dokumentenprozesse modular verbinden.

## Module

- `website/` – Website und CMS-Anbindung
- `agents/` – Master-, E-Mail-, CRM-, Dokument- und Website-Agenten
- `automations/n8n/` – Automatisierungs-Workflows
- `database/schema/` – Datenmodell und Migrationen
- `docs/` – Architektur, Sicherheit und Roadmap

## Grundprinzipien

1. Sensible Aktionen benötigen menschliche Freigabe.
2. Keine Zugangsdaten oder API-Schlüssel im Repository speichern.
3. Kundendaten werden nicht im Quellcode abgelegt.
4. Agenten erhalten nur die Rechte, die sie für ihre Aufgabe benötigen.
5. Änderungen an produktiven Systemen werden protokolliert.

## Status

EEF AI v1 – Grundstruktur.

> Hinweis: Dieses Repository darf keine vertraulichen Kunden-, Bank- oder personenbezogenen Daten enthalten.

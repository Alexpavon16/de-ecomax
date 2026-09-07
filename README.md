# 🇩🇪 de.ecomax.site — Grundsicherung Deutschland

Informationsportal über die Neue Grundsicherung (Grundsicherungsgeld) in Deutschland. Statische HTML-Seiten, gehostet auf Vercel.

## Struktur

```
de-ecomax/
├── funnel/
│   ├── 01-landing.html      → /fn-gs-1  (Landing Page)
│   ├── 02-rechner.html       → /fn-gs-2  (Rechner / Calculator)
│   └── 03-ergebnis.html      → /fn-gs-3  (Ergebnis / Guide)
├── impressum.html             → /impressum
├── datenschutz.html           → /datenschutz
├── knowledge/
│   └── grundsicherung-brain.md  (Knowledge Base)
├── vercel.json                (Routing & Headers)
└── README.md
```

## Funnel-Flow

```
Meta Ad → fn-gs-1 (Landing) → fn-gs-2 (Rechner) → fn-gs-3 (Guide/Ergebnis)
                                    ↓
                              E-Mail Capture (MailerLite)
```

## Legal Compliance

- ✅ **Impressum** (§5 DDG) — ⚠️ Echte Daten eintragen!
- ✅ **Datenschutzerklärung** (DSGVO/GDPR)
- ✅ **Cookie Consent** (Opt-in vor AdSense/Analytics/Pixel)
- ✅ **Disclaimer** (Unabhängiges Portal, keine Behörde)

## Deployment

```bash
# Vercel CLI
vercel --prod

# Oder: Push to GitHub → Vercel auto-deploy
```

## ⚠️ Vor dem Launch

1. **Impressum ausfüllen** — Echte Daten in `impressum.html` und `datenschutz.html`
2. **MailerLite Gruppe** — Neue Gruppe für DE-Subscribers erstellen
3. **Meta Pixel** — Neue Pixel-ID für DE-Kampagnen (oder bestehende verwenden)
4. **AdSense** — Property für de.ecomax.site hinzufügen
5. **GA4** — Neue Property erstellen
6. **Domain** — de.ecomax.site als Subdomain konfigurieren

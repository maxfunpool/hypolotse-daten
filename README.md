# Hypolotse Daten: Baufinanzierung in Deutschland

Offene Datensätze zur Immobilienfinanzierung in Deutschland, gepflegt von [Hypolotse](https://hypolotse.de).
Lizenz: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.de). Nutzung frei, auch kommerziell, mit Quellenangabe „Hypolotse“ und Link.

## Inhalt

| Datei | Inhalt | Aktualisierung | Live-Quelle |
|---|---|---|---|
| `baufinanzierungs-monitor.csv` | Neugeschäft und Effektivzinsen für Wohnungsbaukredite an private Haushalte nach Zinsbindung, monatlich, letzte 25 Monate. Aufbereitet aus der MFI-Zinsstatistik der Deutschen Bundesbank. | monatlich | [hypolotse.de/baufinanzierungs-monitor](https://hypolotse.de/baufinanzierungs-monitor), JSON unter [/api/monitor](https://hypolotse.de/api/monitor) |
| `foerderung.json` | Grunderwerbsteuersätze aller 16 Bundesländer mit Gültigkeitsdatum und die Wohneigentums-Förderprogramme der Landesförderinstitute mit Zielgruppe und Konditionen. | bei Änderung | [hypolotse.de/daten/foerderung](https://hypolotse.de/daten/foerderung/) |

## Spalten `baufinanzierungs-monitor.csv`

- `monat`: Berichtsmonat (JJJJ-MM)
- `volumen_*_mio_eur`: neu vergebene Kredite in Mio. €, gesamt und nach anfänglicher Zinsbindung (variabel/bis 1 Jahr, 1–5, 5–10, über 10 Jahre)
- `davon_neu_verhandelt_mio_eur`: Anteil neu verhandelter Kredite (z. B. Prolongationen)
- `effzins_*_pct`: Effektivzinssatz in Prozent (ohne sonstige Kosten), nach Zinsbindung
- `eff_jahreszins_inkl_kosten_pct`: effektiver Jahreszins einschließlich Kosten, über alle Zinsbindungen

Quelle der Rohdaten: Deutsche Bundesbank, MFI-Zinsstatistik (Reihen SUD231, SUD219, SUD119, SUD131, SUD131Z, SUD289).

## Rechner zum Einbetten

Der Grunderwerbsteuer- und Kaufnebenkosten-Rechner lässt sich kostenlos in jede Website einbetten: [hypolotse.de/einbetten](https://hypolotse.de/einbetten)

## Zitieren

> Hypolotse Baufinanzierungs-Monitor, https://hypolotse.de/baufinanzierungs-monitor, auf Basis der MFI-Zinsstatistik der Deutschen Bundesbank.

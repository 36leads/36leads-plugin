# 36leads

Findet neue Kunden: klärt den idealen Kunden, findet Zielfirmen und Ansprechpartner und übernimmt sie in eine 36leads-Kampagne, direkt im Chat mit Claude oder Codex.

Voraussetzung ist ein [36leads](https://36leads.io)-Konto mit aktiver Kontaktsuche.

## Installation

**Claude Code**

```bash
claude plugin marketplace add 36leads/36leads-plugin
claude plugin install 36leads@36leads
```

Beim ersten Aufruf meldest du dich mit deinem 36leads-Konto an.

**Codex**

```bash
codex plugin marketplace add 36leads/36leads-plugin
codex plugin add 36leads@36leads
codex mcp add 36leads --url https://app.36leads.io/api/mcp/mcp
codex mcp login 36leads
```

Danach eine neue Sitzung starten.

## Nutzung

Sag, dass du mehr Kunden suchst, oder nenne direkt Firmen oder Personen. Der Assistent nutzt, was in deinem Projektordner schon über dein Angebot steht, und arbeitet über dein 36leads-Konto.

## Daten

Das Plugin liest im aktuellen Projektordner Angaben zu deinem Angebot und deinen Kunden. Es sendet Zielbild, Firmen und Personen über `https://app.36leads.io/api/mcp/mcp` an dein 36leads-Konto. Die Anmeldung läuft über OAuth, das Plugin enthält keine Zugangsdaten.

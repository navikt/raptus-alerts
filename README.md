[![Build status](https://github.com/navikt/raptus-alerts/workflows/Deploy%20alerts%20to%20dev/badge.svg)](https://github.com/navikt/raptus-alerts/workflows/Deploy%20alerts%20to%20dev/badge.svg)

# raptus-alerts
Lager alerts for applikasjoner i namespace raptus.

For mer informasjon om hvordan alarmene fungerer, se: `https://doc.nais.io/observability/alerts`.

## Komme i gang
Bruk Prometheus for å teste queries.
- `https://prometheus.prod-gcp.nais.io` (prod-gcp)
- `https://prometheus.dev-gcp.nais.io` (dev-gcp)

## Utvikling
Det er foreløpig bare laget alerts for dev, siden prod er litt langt fram i tid.
Dersom man senere tar i bruk vars-fil, må referanser til labels escapes med "\". Eksempel: \{{ $labels.service }}

## Deploy
Endring på utviklingsbranch trigger deploy til dev-gcp.

## Oppfølging
Triggede alerts i dev-miljø dukker opp i #team-raptus-alerts-dev på Slack.

## For NAV ansatte
Vi er tilgjenngelig på slack kanalen #team-meldeplikt.

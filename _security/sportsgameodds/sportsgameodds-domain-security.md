---
api_specs:
- filename: sportsgameodds-account-api-openapi.yml
  format: yaml
  label: SportsGameOdds Account API
  slug: sportsgameodds-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsgameodds/refs/heads/main/openapi/sportsgameodds-account-api-openapi.yml
- filename: sportsgameodds-events-api-openapi.yml
  format: yaml
  label: SportsGameOdds Events API
  slug: sportsgameodds-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsgameodds/refs/heads/main/openapi/sportsgameodds-events-api-openapi.yml
- filename: sportsgameodds-leagues-api-openapi.yml
  format: yaml
  label: SportsGameOdds Leagues API
  slug: sportsgameodds-leagues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsgameodds/refs/heads/main/openapi/sportsgameodds-leagues-api-openapi.yml
- filename: sportsgameodds-markets-api-openapi.yml
  format: yaml
  label: SportsGameOdds Markets API
  slug: sportsgameodds-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsgameodds/refs/heads/main/openapi/sportsgameodds-markets-api-openapi.yml
- filename: sportsgameodds-players-api-openapi.yml
  format: yaml
  label: SportsGameOdds Players API
  slug: sportsgameodds-players-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsgameodds/refs/heads/main/openapi/sportsgameodds-players-api-openapi.yml
- filename: sportsgameodds-sports-api-openapi.yml
  format: yaml
  label: SportsGameOdds Sports API
  slug: sportsgameodds-sports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsgameodds/refs/heads/main/openapi/sportsgameodds-sports-api-openapi.yml
- filename: sportsgameodds-stats-api-openapi.yml
  format: yaml
  label: SportsGameOdds Stats API
  slug: sportsgameodds-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsgameodds/refs/heads/main/openapi/sportsgameodds-stats-api-openapi.yml
- filename: sportsgameodds-teams-api-openapi.yml
  format: yaml
  label: SportsGameOdds Teams API
  slug: sportsgameodds-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsgameodds/refs/heads/main/openapi/sportsgameodds-teams-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sportsgameodds.com
  spf: true
hosts:
- cert_expires: Aug 16 12:50:06 2026 GMT
  host: sportsgameodds.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 12:50:06 2026 GMT
  host: api.sportsgameodds.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sportsgameodds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SportsGameOdds, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SportsGameOdds
provider_slug: sportsgameodds
slug: sportsgameodds-domain-security
source_filename: sportsgameodds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sportsgameodds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 12:50:06 2026 GMT\n  hsts: false\n- host: api.sportsgameodds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 12:50:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sportsgameodds.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sportsgameodds/refs/heads/main/security/sportsgameodds-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sports Betting
- Odds
- Sports Data
- Fantasy Sports
- Gambling
---

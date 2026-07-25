---
api_specs:
- filename: pandascore-changes-api-openapi.yml
  format: yaml
  label: PandaScore Changes API
  slug: pandascore-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-changes-api-openapi.yml
- filename: pandascore-game-cs-go-api-openapi.yml
  format: yaml
  label: PandaScore Game - CS:GO API
  slug: pandascore-game-cs-go-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-game-cs-go-api-openapi.yml
- filename: pandascore-game-dota-2-api-openapi.yml
  format: yaml
  label: PandaScore Game - Dota 2 API
  slug: pandascore-game-dota-2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-game-dota-2-api-openapi.yml
- filename: pandascore-game-league-of-legends-api-openapi.yml
  format: yaml
  label: PandaScore Game - League of Legends API
  slug: pandascore-game-league-of-legends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-game-league-of-legends-api-openapi.yml
- filename: pandascore-game-valorant-api-openapi.yml
  format: yaml
  label: PandaScore Game - Valorant API
  slug: pandascore-game-valorant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-game-valorant-api-openapi.yml
- filename: pandascore-leagues-api-openapi.yml
  format: yaml
  label: PandaScore Leagues API
  slug: pandascore-leagues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-leagues-api-openapi.yml
- filename: pandascore-matches-api-openapi.yml
  format: yaml
  label: PandaScore Matches API
  slug: pandascore-matches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-matches-api-openapi.yml
- filename: pandascore-players-api-openapi.yml
  format: yaml
  label: PandaScore Players API
  slug: pandascore-players-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-players-api-openapi.yml
- filename: pandascore-series-api-openapi.yml
  format: yaml
  label: PandaScore Series API
  slug: pandascore-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-series-api-openapi.yml
- filename: pandascore-teams-api-openapi.yml
  format: yaml
  label: PandaScore Teams API
  slug: pandascore-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-teams-api-openapi.yml
- filename: pandascore-tournaments-api-openapi.yml
  format: yaml
  label: PandaScore Tournaments API
  slug: pandascore-tournaments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-tournaments-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: pandascore.co
  spf: true
hosts:
- cert_expires: Aug 14 09:29:21 2026 GMT
  host: pandascore.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 06:17:20 2026 GMT
  host: app.pandascore.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 04:32:50 2026 GMT
  host: developers.pandascore.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pandascore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PandaScore, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: PandaScore
provider_slug: pandascore
slug: pandascore-domain-security
source_filename: pandascore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pandascore.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 09:29:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.pandascore.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 06:17:20 2026 GMT\n  hsts: false\n- host: developers.pandascore.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 04:32:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pandascore.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/security/pandascore-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Esports
- Odds
- Betting
- Live Data
- Stats
- Fantasy
- WebSocket
- REST
---

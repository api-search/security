---
api_specs:
- filename: goalserve-commentaries-api-openapi.yml
  format: yaml
  label: GoalServe Commentaries API
  slug: goalserve-commentaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goalserve/refs/heads/main/openapi/goalserve-commentaries-api-openapi.yml
- filename: goalserve-fixtures-api-openapi.yml
  format: yaml
  label: GoalServe Fixtures API
  slug: goalserve-fixtures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goalserve/refs/heads/main/openapi/goalserve-fixtures-api-openapi.yml
- filename: goalserve-live-scores-api-openapi.yml
  format: yaml
  label: GoalServe Live Scores API
  slug: goalserve-live-scores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goalserve/refs/heads/main/openapi/goalserve-live-scores-api-openapi.yml
- filename: goalserve-player-data-api-openapi.yml
  format: yaml
  label: GoalServe Player Data API
  slug: goalserve-player-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goalserve/refs/heads/main/openapi/goalserve-player-data-api-openapi.yml
- filename: goalserve-standings-api-openapi.yml
  format: yaml
  label: GoalServe Standings API
  slug: goalserve-standings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goalserve/refs/heads/main/openapi/goalserve-standings-api-openapi.yml
- filename: goalserve-team-data-api-openapi.yml
  format: yaml
  label: GoalServe Team Data API
  slug: goalserve-team-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goalserve/refs/heads/main/openapi/goalserve-team-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: goalserve.com
  spf: true
hosts:
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: www.goalserve.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Goalserve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoalServe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: GoalServe
provider_slug: goalserve
slug: goalserve-domain-security
source_filename: goalserve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.goalserve.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: goalserve.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goalserve/refs/heads/main/security/goalserve-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Sports Data
- Live Scores
- Odds
- Fixtures
- Soccer
---

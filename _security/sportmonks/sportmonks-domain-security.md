---
api_specs:
- filename: postman.yaml
  format: yaml
  label: Sportmonks Cricket API
  slug: cricket-api
  spec_type: Postman
  url: https://cricket-postman.sportmonks.com/
- filename: sportmonks-fixtures-api-openapi.yml
  format: yaml
  label: Sportmonks Fixtures API
  slug: sportmonks-fixtures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportmonks/refs/heads/main/openapi/sportmonks-fixtures-api-openapi.yml
- filename: sportmonks-leagues-api-openapi.yml
  format: yaml
  label: Sportmonks Leagues API
  slug: sportmonks-leagues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportmonks/refs/heads/main/openapi/sportmonks-leagues-api-openapi.yml
- filename: sportmonks-livescores-api-openapi.yml
  format: yaml
  label: Sportmonks Livescores API
  slug: sportmonks-livescores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportmonks/refs/heads/main/openapi/sportmonks-livescores-api-openapi.yml
- filename: sportmonks-odds-api-openapi.yml
  format: yaml
  label: Sportmonks Odds API
  slug: sportmonks-odds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportmonks/refs/heads/main/openapi/sportmonks-odds-api-openapi.yml
- filename: sportmonks-players-api-openapi.yml
  format: yaml
  label: Sportmonks Players API
  slug: sportmonks-players-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportmonks/refs/heads/main/openapi/sportmonks-players-api-openapi.yml
- filename: sportmonks-predictions-api-openapi.yml
  format: yaml
  label: Sportmonks Predictions API
  slug: sportmonks-predictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportmonks/refs/heads/main/openapi/sportmonks-predictions-api-openapi.yml
- filename: sportmonks-schedules-api-openapi.yml
  format: yaml
  label: Sportmonks Schedules API
  slug: sportmonks-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportmonks/refs/heads/main/openapi/sportmonks-schedules-api-openapi.yml
- filename: sportmonks-seasons-api-openapi.yml
  format: yaml
  label: Sportmonks Seasons API
  slug: sportmonks-seasons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportmonks/refs/heads/main/openapi/sportmonks-seasons-api-openapi.yml
- filename: sportmonks-standings-api-openapi.yml
  format: yaml
  label: Sportmonks Standings API
  slug: sportmonks-standings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportmonks/refs/heads/main/openapi/sportmonks-standings-api-openapi.yml
- filename: sportmonks-teams-api-openapi.yml
  format: yaml
  label: Sportmonks Teams API
  slug: sportmonks-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportmonks/refs/heads/main/openapi/sportmonks-teams-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sportmonks.com
  spf: true
hosts:
- cert_expires: Sep 20 01:45:32 2026 GMT
  host: www.sportmonks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 12:02:24 2026 GMT
  host: my.sportmonks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 10:19:20 2026 GMT
  host: docs.sportmonks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sportmonks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sportmonks, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sportmonks
provider_slug: sportmonks
slug: sportmonks-domain-security
source_filename: sportmonks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sportmonks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 01:45:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: my.sportmonks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 12:02:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sportmonks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 10:19:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sportmonks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sportmonks/refs/heads/main/security/sportmonks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cricket
- Data
- Developer-Friendly
- Football
- Formula 1
- Livescores
- Motorsport
- Real-Time
- Soccer
- Sports
- Sports Data
- Statistics
---

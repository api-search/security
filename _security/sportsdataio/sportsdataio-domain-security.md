---
api_specs:
- filename: sportsdataio-nfl-openapi.yml
  format: yaml
  label: SportsDataIO NFL API
  slug: sportsdataio-nfl
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdataio/refs/heads/main/openapi/sportsdataio-nfl-openapi.yml
- filename: sportsdataio-mlb-openapi.yml
  format: yaml
  label: SportsDataIO MLB API
  slug: sportsdataio-mlb
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdataio/refs/heads/main/openapi/sportsdataio-mlb-openapi.yml
- filename: sportsdataio-nba-openapi.yml
  format: yaml
  label: SportsDataIO NBA API
  slug: sportsdataio-nba
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdataio/refs/heads/main/openapi/sportsdataio-nba-openapi.yml
- filename: sportsdataio-nhl-openapi.yml
  format: yaml
  label: SportsDataIO NHL API
  slug: sportsdataio-nhl
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdataio/refs/heads/main/openapi/sportsdataio-nhl-openapi.yml
- filename: sportsdataio-soccer-openapi.yml
  format: yaml
  label: SportsDataIO Soccer API
  slug: sportsdataio-soccer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdataio/refs/heads/main/openapi/sportsdataio-soccer-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sportsdata.io
  spf: true
hosts:
- cert_expires: Aug  1 08:53:15 2026 GMT
  host: sportsdata.io
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 02:38:25 2026 GMT
  host: api.sportsdata.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sportsdataio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SportsDataIO, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SportsDataIO
provider_slug: sportsdataio
slug: sportsdataio-domain-security
source_filename: sportsdataio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sportsdata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  1 08:53:15 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: api.sportsdata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 02:38:25 2026 GMT\n  hsts: null\ndomains:\n- domain: sportsdata.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sportsdataio/refs/heads/main/security/sportsdataio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sports Data
- Statistics
- Live Scores
- Fantasy Sports
- Odds
- NFL
- NBA
- MLB
- NHL
- Soccer
---

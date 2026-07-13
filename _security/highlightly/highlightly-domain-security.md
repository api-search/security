---
api_specs:
- filename: highlightly-openapi.yml
  format: yaml
  label: Highlightly Matches & Fixtures API
  slug: matches-fixtures
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-openapi.yml
- filename: highlightly-openapi.yml
  format: yaml
  label: Highlightly Live Scores API
  slug: live-scores
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-openapi.yml
- filename: highlightly-openapi.yml
  format: yaml
  label: Highlightly Standings API
  slug: standings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-openapi.yml
- filename: highlightly-openapi.yml
  format: yaml
  label: Highlightly Statistics API
  slug: statistics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-openapi.yml
- filename: highlightly-openapi.yml
  format: yaml
  label: Highlightly Odds API
  slug: odds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-openapi.yml
- filename: highlightly-openapi.yml
  format: yaml
  label: Highlightly Highlights API
  slug: highlights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: highlightly.net
  spf: true
hosts:
- cert_expires: Aug 20 11:09:13 2026 GMT
  host: highlightly.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 11:09:13 2026 GMT
  host: sports.highlightly.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Highlightly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Highlightly, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Highlightly
provider_slug: highlightly
slug: highlightly-domain-security
source_filename: highlightly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: highlightly.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 11:09:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sports.highlightly.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 11:09:13 2026 GMT\n  hsts: null\ndomains:\n- domain: highlightly.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/security/highlightly-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Sports
- Sports Data
- Live Scores
- Odds
- Highlights
---

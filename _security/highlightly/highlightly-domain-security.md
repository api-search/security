---
api_specs:
- filename: highlightly-catalog-api-openapi.yml
  format: yaml
  label: Highlightly Catalog API
  slug: highlightly-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-catalog-api-openapi.yml
- filename: highlightly-highlights-api-openapi.yml
  format: yaml
  label: Highlightly Highlights API
  slug: highlightly-highlights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-highlights-api-openapi.yml
- filename: highlightly-matches-api-openapi.yml
  format: yaml
  label: Highlightly Matches API
  slug: highlightly-matches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-matches-api-openapi.yml
- filename: highlightly-odds-api-openapi.yml
  format: yaml
  label: Highlightly Odds API
  slug: highlightly-odds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-odds-api-openapi.yml
- filename: highlightly-standings-api-openapi.yml
  format: yaml
  label: Highlightly Standings API
  slug: highlightly-standings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-standings-api-openapi.yml
- filename: highlightly-statistics-api-openapi.yml
  format: yaml
  label: Highlightly Statistics API
  slug: highlightly-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-statistics-api-openapi.yml
- filename: highlightly-teams-api-openapi.yml
  format: yaml
  label: Highlightly Teams API
  slug: highlightly-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-teams-api-openapi.yml
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

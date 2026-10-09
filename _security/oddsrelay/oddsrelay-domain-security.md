---
api_specs:
- filename: oddsrelay-account-api-openapi.yml
  format: yaml
  label: OddsRelay Account API
  slug: oddsrelay-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oddsrelay/refs/heads/main/openapi/oddsrelay-account-api-openapi.yml
- filename: oddsrelay-discovery-api-openapi.yml
  format: yaml
  label: OddsRelay Discovery API
  slug: oddsrelay-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oddsrelay/refs/heads/main/openapi/oddsrelay-discovery-api-openapi.yml
- filename: oddsrelay-odds-api-openapi.yml
  format: yaml
  label: OddsRelay Odds API
  slug: oddsrelay-odds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oddsrelay/refs/heads/main/openapi/oddsrelay-odds-api-openapi.yml
- filename: oddsrelay-service-api-openapi.yml
  format: yaml
  label: OddsRelay Service API
  slug: oddsrelay-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oddsrelay/refs/heads/main/openapi/oddsrelay-service-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oddsrelay.io
  spf: true
hosts:
- cert_expires: Dec  3 09:57:23 2026 GMT
  host: oddsrelay.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Oddsrelay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OddsRelay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OddsRelay
provider_slug: oddsrelay
slug: oddsrelay-domain-security
source_filename: oddsrelay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oddsrelay.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 09:57:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: oddsrelay.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oddsrelay/refs/heads/main/security/oddsrelay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sports Betting
- Odds
- Sports Data
- Matched Betting
- Data Feeds
---

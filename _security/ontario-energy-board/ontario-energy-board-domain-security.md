---
api_specs:
- filename: ontario-energy-board-open-data-openapi.yml
  format: yaml
  label: OEB Open Data
  slug: oeb-open-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-open-data-openapi.yml
- filename: ontario-energy-board-rds-openapi.yml
  format: yaml
  label: OEB Regulatory Document Search (RDS)
  slug: oeb-regulatory-document-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-rds-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oeb.ca
  spf: true
hosts:
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: www.oeb.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: www.rds.oeb.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ontario Energy Board Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ontario Energy Board, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ontario Energy Board
provider_slug: ontario-energy-board
slug: ontario-energy-board-domain-security
source_filename: ontario-energy-board-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oeb.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.rds.oeb.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oeb.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/security/ontario-energy-board-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Canada
- Ontario
- Utilities
- Electricity
- Gas
- Green Button
- Smart Metering
- Energy Markets
- Regulator
- Open Data
- Grid
---

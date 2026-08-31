---
api_specs:
- filename: chargy-locations-api-openapi.yml
  format: yaml
  label: char.gy Locations API
  slug: chargy-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargy/refs/heads/main/openapi/chargy-locations-api-openapi.yml
- filename: chargy-tariffs-api-openapi.yml
  format: yaml
  label: char.gy Tariffs API
  slug: chargy-tariffs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargy/refs/heads/main/openapi/chargy-tariffs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: char.gy
  spf: true
hosts:
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: char.gy
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 20:09:39 2026 GMT
  host: help.char.gy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chargy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for char.gy, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: char.gy
provider_slug: chargy
slug: chargy-domain-security
source_filename: chargy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: char.gy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: help.char.gy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 20:09:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: char.gy\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chargy/refs/heads/main/security/chargy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United Kingdom
- EV Charging
- Electricity
- Utilities
- OCPI
- Charge Point Operator
- Open Data
- Roaming
- Tariffs
- Mobility
- Electrification
---

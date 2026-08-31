---
api_specs:
- filename: chargefox-fleets-api-openapi.yml
  format: yaml
  label: Chargefox Fleets API
  slug: chargefox-fleets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargefox/refs/heads/main/openapi/chargefox-fleets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chargefox.com
  spf: true
hosts:
- cert_expires: Sep 10 04:49:45 2026 GMT
  host: www.chargefox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: app.chargefox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chargefox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chargefox, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chargefox
provider_slug: chargefox
slug: chargefox-domain-security
source_filename: chargefox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chargefox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 04:49:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.chargefox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chargefox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chargefox/refs/heads/main/security/chargefox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Australia
- EV Charging
- Electricity
- Utilities
- OCPI
- Charge Point Operator
- Roaming
- Fleets
- Mobility
- Charging Sessions
- Electrification
---

---
api_specs:
- filename: ev-energy-api-v2-openapi.yaml
  format: yaml
  label: ev.energy v2 API
  slug: ev-energy-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ev-energy/refs/heads/main/openapi/ev-energy-api-v2-openapi.yaml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ev.energy
  spf: true
hosts:
- cert_expires: Oct 14 03:33:37 2026 GMT
  host: www.ev.energy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 12:05:53 2026 GMT
  host: developers.ev.energy
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: api.ev.energy
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ev Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ev.energy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ev.energy
provider_slug: ev-energy
slug: ev-energy-domain-security
source_filename: ev-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ev.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 03:33:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.ev.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 12:05:53 2026 GMT\n  hsts: false\n- host: api.ev.energy\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ev.energy\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ev-energy/refs/heads/main/security/ev-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Electric Vehicles
- EV Charging
- Smart Charging
- Utilities
- Sustainability
- Virtual Power Plant
- Demand Response
- Solar
- Home Energy
- Internet of Things
---

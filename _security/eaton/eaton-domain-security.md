---
api_specs:
- filename: smart-breaker-openapi.yml
  format: yaml
  label: Eaton Smart Breaker API
  slug: eaton-smart-breaker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/smart-breaker-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eaton.com
  spf: true
hosts:
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: www.eaton.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.em.eaton.com
  https: false
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: knowledgehub.eaton.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eaton Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eaton, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Eaton
provider_slug: eaton
slug: eaton-domain-security
source_filename: eaton-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eaton.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: null\n- host: api.em.eaton.com\n  https: false\n- host: knowledgehub.eaton.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: eaton.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/security/eaton-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Power Management
- Electrical
- Smart Breaker
- EV Charging
- Demand Response
- Data Center
- DCIM
- PDU
- UPS
- Utility
- Industrial
- Building
- Mobility
- AI Factory
- Energy
- IoT
- Sustainability
---

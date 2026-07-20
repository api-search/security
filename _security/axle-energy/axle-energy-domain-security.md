---
api_specs:
- filename: axle-energy-openapi-original.json
  format: json
  label: Axle API
  slug: axle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axle-energy/refs/heads/main/openapi/axle-energy-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: axle.energy
  spf: true
hosts:
- cert_expires: Aug 20 07:41:59 2026 GMT
  host: www.axle.energy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 12:54:20 2026 GMT
  host: api.axle.energy
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Axle Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axle Energy, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Axle Energy
provider_slug: axle-energy
slug: axle-energy-domain-security
source_filename: axle-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.axle.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 07:41:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.axle.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 12:54:20 2026 GMT\n  hsts: null\ndomains:\n- domain: axle.energy\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axle-energy/refs/heads/main/security/axle-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Energy
- Flexibility
- Virtual Power Plant
- Electric Vehicles
- Smart Charging
- Batteries
- Demand Response
- Grid
- Sustainability
---

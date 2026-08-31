---
api_specs:
- filename: carmd-openapi.yml
  format: yaml
  label: CarMD Vehicle API
  slug: carmd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carmd/refs/heads/main/openapi/carmd-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: carmd.com
  spf: true
hosts:
- cert_expires: Oct  4 20:04:32 2026 GMT
  host: carmd.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- host: api.carmd.com
  https: false
kind: domain-security
layout: security
method: probed
name: Carmd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CarMD, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CarMD
provider_slug: carmd
slug: carmd-domain-security
source_filename: carmd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carmd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 20:04:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: api.carmd.com\n  https: false\ndomains:\n- domain: carmd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carmd/refs/heads/main/security/carmd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automobiles
- Cars
- Diagnostics
- Vehicles
- Automotive
- OBD-II
- Agentic Commerce
- MCP
- E-Commerce
---

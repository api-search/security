---
api_specs:
- filename: scanverity-resolution-api-openapi.json
  format: json
  label: Scanverity Resolution API
  slug: scanverity-resolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scanverity-resolution-api/refs/heads/main/openapi/scanverity-resolution-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: scanverity.com
  spf: true
hosts:
- cert_expires: Nov 19 08:29:23 2026 GMT
  host: scanverity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Scanverity Resolution Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scanverity Resolution API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Scanverity Resolution API
provider_slug: scanverity-resolution-api
slug: scanverity-resolution-api-domain-security
source_filename: scanverity-resolution-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scanverity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 08:29:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scanverity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scanverity-resolution-api/refs/heads/main/security/scanverity-resolution-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Prediction Markets
- Resolution Risk
- Market Intelligence
- Due Diligence
- Webhooks
- OpenAPI
- Fintech
- Risk Analytics
- Polymarket
- Event Contracts
- Agent Ready
---

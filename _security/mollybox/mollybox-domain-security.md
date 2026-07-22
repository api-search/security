---
api_specs:
- filename: mollybox-arcflow-openapi.json
  format: json
  label: Arcflow API
  slug: arcflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mollybox/refs/heads/main/openapi/mollybox-arcflow-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mollybox.cn
  resolves_to: 101.132.184.190
  spf: false
hosts:
- host: www.mollybox.cn
  hsts: false
  http: true
  http_server: uvicorn
  https: false
  https_note: TLS/443 refuses connection (curl exit 7); service is HTTP-only
kind: domain-security
layout: security
method: probed
name: Mollybox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MollyBox, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: MollyBox
provider_slug: mollybox
slug: mollybox-domain-security
source_filename: mollybox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: 'dig + curl against www.mollybox.cn / mollybox.cn (2026-07-20)'\nhosts:\n  - host: www.mollybox.cn\n    https: false\n    https_note: 'TLS/443 refuses connection (curl exit 7); service is HTTP-only'\n    http: true\n    http_server: uvicorn\n    hsts: false\ndomains:\n  - domain: mollybox.cn\n    resolves_to: 101.132.184.190\n    dnssec: false\n    caa: []\n    spf: false\n    dmarc: false\nfindings:\n  - No HTTPS/TLS on the web/API host (port 443 refused); API is served over plaintext HTTP.\n  - No HSTS header.\n  - No DNSSEC on the mollybox.cn zone.\n  - No CAA records.\n  - No SPF record.\n  - No DMARC record.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mollybox/refs/heads/main/security/mollybox-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Consumer
- API
- Bookmarking
- Resource Capture
- Read It Later
- FastAPI
- Self-Hosted
---

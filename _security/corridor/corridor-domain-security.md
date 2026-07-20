---
api_specs:
- filename: corridor-openapi.yml
  format: yaml
  label: Corridor API
  slug: corridor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corridor/refs/heads/main/openapi/corridor-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: corridor.dev
  spf: true
hosts:
- cert_expires: Oct 16 01:09:25 2026 GMT
  host: corridor.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 07:40:21 2026 GMT
  host: docs.corridor.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: app.corridor.dev
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Corridor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Corridor, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Corridor
provider_slug: corridor
slug: corridor-domain-security
source_filename: corridor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corridor.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 01:09:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.corridor.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 07:40:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.corridor.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: corridor.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corridor/refs/heads/main/security/corridor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Application Security
- AI Coding
- Code Security
- Developer Tools
- Guardrails
- MCP
- Static Analysis
- DevSecOps
---

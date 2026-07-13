---
api_specs:
- filename: continue-dev-hub-ide-api-openapi.yml
  format: yaml
  label: Continue Hub IDE API
  slug: continue-hub-ide-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/continue-dev/refs/heads/main/openapi/continue-dev-hub-ide-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: continue.dev
  spf: true
hosts:
- cert_expires: Aug 29 10:40:12 2026 GMT
  host: www.continue.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: api.continue.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  9 22:04:19 2026 GMT
  host: docs.continue.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Continue Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Continue, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Continue
provider_slug: continue-dev
slug: continue-dev-domain-security
source_filename: continue-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.continue.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 10:40:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.continue.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: null\n- host: docs.continue.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  9 22:04:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: continue.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/continue-dev/refs/heads/main/security/continue-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Artificial Intelligence
- Developer Tools
- Code Assistant
- Open Source
- VS Code
- JetBrains
- CLI
- MCP
- Apache 2.0
---

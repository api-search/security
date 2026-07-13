---
api_specs:
- filename: theneo-api-openapi.yml
  format: yaml
  label: Theneo
  slug: theneo
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/theneo/refs/heads/main/openapi/theneo-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: theneo.io
  spf: true
hosts:
- cert_expires: Aug 16 18:54:05 2026 GMT
  host: www.theneo.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: api.theneo.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Theneo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Theneo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Theneo
provider_slug: theneo
slug: theneo-domain-security
source_filename: theneo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.theneo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 18:54:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.theneo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: theneo.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/theneo/refs/heads/main/security/theneo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Documentation
- Developer Portal
- Developer Tools
- Documentation Platform
- AI
- AI Co-Pilot
- MCP
- Platform
---

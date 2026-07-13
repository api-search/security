---
api_specs:
- filename: sideko-openapi.yml
  format: yaml
  label: Sideko API
  slug: sideko-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/openapi/sideko-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sideko.dev
  spf: true
hosts:
- cert_expires: Aug 30 06:51:19 2026 GMT
  host: www.sideko.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 23:10:51 2026 GMT
  host: docs.sideko.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 20:55:29 2026 GMT
  host: api.sideko.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sideko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sideko, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sideko
provider_slug: sideko
slug: sideko-domain-security
source_filename: sideko-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sideko.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 06:51:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sideko.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:10:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.sideko.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 20:55:29 2026 GMT\n  hsts: null\ndomains:\n- domain: sideko.dev\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/security/sideko-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CLI
- Documentation
- Mock Servers
- Platform
- SDKs
- API Tooling
- SDK Generation
- MCP Generation
- AI
- Hybrid Codegen
- OpenAPI Linting
---

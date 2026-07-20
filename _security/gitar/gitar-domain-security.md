---
api_specs:
- filename: gitar-openapi-original.json
  format: json
  label: Gitar External API
  slug: gitar-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitar/refs/heads/main/openapi/gitar-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gitar.ai
  spf: true
hosts:
- cert_expires: Oct  1 17:19:57 2026 GMT
  host: gitar.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: api.gitar.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gitar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gitar, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gitar
provider_slug: gitar
slug: gitar-domain-security
source_filename: gitar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gitar.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 17:19:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.gitar.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: gitar.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitar/refs/heads/main/security/gitar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Developer Tools
- Code Review
- CI/CD
- Code Quality
- AI
- Developer Productivity
- Automation
---

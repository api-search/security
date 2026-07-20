---
api_specs:
- filename: codag-openapi-original.json
  format: json
  label: Codag API
  slug: codag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codag/refs/heads/main/openapi/codag-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: codag.ai
  spf: true
hosts:
- cert_expires: Sep 12 02:23:37 2026 GMT
  host: codag.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 03:08:04 2026 GMT
  host: api.codag.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Codag Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Codag, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Codag
provider_slug: codag
slug: codag-domain-security
source_filename: codag-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codag.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 02:23:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.codag.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 03:08:04 2026 GMT\n  hsts: null\ndomains:\n- domain: codag.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codag/refs/heads/main/security/codag-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Developer Tools
- Logging
- Observability
- Log Compression
- AI Agents
- MCP
- LLM Tooling
- Debugging
- Y Combinator
---

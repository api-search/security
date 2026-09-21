---
api_specs:
- filename: babyblueviper-com-openapi.yml
  format: yaml
  label: invinoveritas API
  slug: invinoveritas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babyblueviper-com/refs/heads/main/openapi/babyblueviper-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: babyblueviper.com
  spf: false
hosts:
- cert_expires: Dec 17 15:08:57 2026 GMT
  host: babyblueviper.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 20:44:42 2026 GMT
  host: api.babyblueviper.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Babyblueviper Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for invinoveritas, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: invinoveritas
provider_slug: babyblueviper-com
slug: babyblueviper-com-domain-security
source_filename: babyblueviper-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: babyblueviper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 15:08:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.babyblueviper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 20:44:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: babyblueviper.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/babyblueviper-com/refs/heads/main/security/babyblueviper-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- Agent Verification
- Agent Governance
- MCP
- A2A
- Bitcoin Lightning
- x402
- Trading
- Cryptographic Proofs
- Agent Marketplace
---

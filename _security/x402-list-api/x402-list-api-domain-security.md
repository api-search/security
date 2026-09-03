---
api_specs:
- filename: openapi.json
  format: json
  label: x402 List API
  slug: x402-list-api
  spec_type: OpenAPI
  url: https://x402-list.com/api/v1/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: x402-list.com
  spf: true
hosts:
- cert_expires: Nov 12 17:55:13 2026 GMT
  host: x402-list.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: X402 List Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for x402 List API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: x402 List API
provider_slug: x402-list-api
slug: x402-list-api-domain-security
source_filename: x402-list-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: x402-list.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 17:55:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: x402-list.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/x402-list-api/refs/heads/main/security/x402-list-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- x402
- crypto
- '402'
- agentic-payments
- API directory
- registry
- AI agents
- blockchain
- developer tools
- uptime monitoring
---

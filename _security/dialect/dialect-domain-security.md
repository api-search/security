---
api_specs:
- filename: dialect-alerts-openapi.json
  format: json
  label: Dialect Alerts V2 API
  slug: dialect-alerts-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialect/refs/heads/main/openapi/dialect-alerts-openapi.json
- filename: dialect-blinks-openapi.json
  format: json
  label: Dialect Blinks API
  slug: dialect-blinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialect/refs/heads/main/openapi/dialect-blinks-openapi.json
- filename: dialect-markets-openapi.json
  format: json
  label: Dialect Markets & Positions API
  slug: dialect-markets-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialect/refs/heads/main/openapi/dialect-markets-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dialect.to
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: dial.to
  spf: false
hosts:
- cert_expires: Sep 15 02:01:17 2026 GMT
  host: www.dialect.to
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 16:33:32 2026 GMT
  host: docs.dialect.to
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 23:47:23 2026 GMT
  host: alerts-api.dial.to
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dialect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dialect, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dialect
provider_slug: dialect
slug: dialect-domain-security
source_filename: dialect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dialect.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 02:01:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.dialect.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 16:33:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: alerts-api.dial.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:47:23 2026 GMT\n  hsts: null\ndomains:\n- domain: dialect.to\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: dial.to\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dialect/refs/heads/main/security/dialect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Infrastructure
- Web3
- Blockchain
- Solana
- Notifications
- Messaging
- Alerts
- DeFi
- Payments
- Agents
- MCP
---

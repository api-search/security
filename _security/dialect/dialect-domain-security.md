---
api_specs:
- filename: dialect-blink-api-openapi.yml
  format: yaml
  label: Dialect Blink API
  slug: dialect-blink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialect/refs/heads/main/openapi/dialect-blink-api-openapi.yml
- filename: dialect-blink-data-table-api-openapi.yml
  format: yaml
  label: Dialect Blink Data Table API
  slug: dialect-blink-data-table-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialect/refs/heads/main/openapi/dialect-blink-data-table-api-openapi.yml
- filename: dialect-blink-lists-api-openapi.yml
  format: yaml
  label: Dialect Blink Lists API
  slug: dialect-blink-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialect/refs/heads/main/openapi/dialect-blink-lists-api-openapi.yml
- filename: dialect-blink-preview-api-openapi.yml
  format: yaml
  label: Dialect Blink Preview API
  slug: dialect-blink-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialect/refs/heads/main/openapi/dialect-blink-preview-api-openapi.yml
- filename: dialect-channels-api-openapi.yml
  format: yaml
  label: Dialect Channels API
  slug: dialect-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialect/refs/heads/main/openapi/dialect-channels-api-openapi.yml
- filename: dialect-inbox-api-openapi.yml
  format: yaml
  label: Dialect Inbox API
  slug: dialect-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialect/refs/heads/main/openapi/dialect-inbox-api-openapi.yml
- filename: dialect-markets-api-openapi.yml
  format: yaml
  label: Dialect Markets API
  slug: dialect-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialect/refs/heads/main/openapi/dialect-markets-api-openapi.yml
- filename: dialect-positions-api-openapi.yml
  format: yaml
  label: Dialect Positions API
  slug: dialect-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialect/refs/heads/main/openapi/dialect-positions-api-openapi.yml
- filename: dialect-send-api-openapi.yml
  format: yaml
  label: Dialect Send API
  slug: dialect-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialect/refs/heads/main/openapi/dialect-send-api-openapi.yml
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
- Notification
- Messaging
- Alerts
- DeFi
- Payments
- Agents
- MCP
---

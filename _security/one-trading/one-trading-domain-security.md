---
api_specs:
- filename: one-trading-fast-openapi.yml
  format: yaml
  label: One Trading Fast API
  slug: one-trading-fast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/one-trading/refs/heads/main/openapi/one-trading-fast-openapi.yml
- filename: one-trading-streams-asyncapi.yml
  format: yaml
  label: One Trading WebSocket Streams API
  slug: one-trading-websocket-streams-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/one-trading/refs/heads/main/asyncapi/one-trading-streams-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: onetrading.com
  spf: true
hosts:
- cert_expires: Sep 12 17:01:57 2026 GMT
  host: onetrading.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 00:01:42 2026 GMT
  host: docs.onetrading.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 23 14:31:58 2026 GMT
  host: api.onetrading.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: One Trading Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for One Trading, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: One Trading
provider_slug: one-trading
slug: one-trading-domain-security
source_filename: one-trading-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onetrading.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 17:01:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.onetrading.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  3 00:01:42 2026 GMT\n  hsts: false\n- host: api.onetrading.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 14:31:58 2026 GMT\n  hsts: null\ndomains:\n- domain: onetrading.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/one-trading/refs/heads/main/security/one-trading-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cryptocurrency
- Crypto Exchange
- Trading
- Derivatives
- Futures
- Financial Services
- Market Data
- WebSocket
- Fintech
---

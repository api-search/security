---
api_specs:
- filename: tradestation-api-openapi.yml
  format: yaml
  label: TradeStation API
  slug: tradestation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradestation/refs/heads/main/openapi/tradestation-api-openapi.yml
- filename: tradestation-streaming-asyncapi.yml
  format: yaml
  label: TradeStation Streaming API
  slug: tradestation-streaming
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradestation/refs/heads/main/asyncapi/tradestation-streaming-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tradestation.com
  spf: true
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: www.tradestation.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: api.tradestation.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: sim-api.tradestation.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tradestation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TradeStation, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TradeStation
provider_slug: tradestation
slug: tradestation-domain-security
source_filename: tradestation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tradestation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tradestation.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: null\n- host: sim-api.tradestation.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tradestation.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradestation/refs/heads/main/security/tradestation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Brokerage
- Cryptocurrency
- Finance
- Futures
- Market Data
- Options
- Stocks
- Trading
---

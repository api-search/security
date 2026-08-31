---
api_specs:
- filename: legendtrade-ws-asyncapi.yml
  format: yaml
  label: Legend WebSocket API
  slug: websocket
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/legendtrade/refs/heads/main/asyncapi/legendtrade-ws-asyncapi.yml
- filename: legendtrade-health-api-openapi.yml
  format: yaml
  label: LegendTrade Health API
  slug: legendtrade-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/legendtrade/refs/heads/main/openapi/legendtrade-health-api-openapi.yml
- filename: legendtrade-info-api-openapi.yml
  format: yaml
  label: LegendTrade Info API
  slug: legendtrade-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/legendtrade/refs/heads/main/openapi/legendtrade-info-api-openapi.yml
- filename: legendtrade-market-data-api-openapi.yml
  format: yaml
  label: LegendTrade Market Data API
  slug: legendtrade-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/legendtrade/refs/heads/main/openapi/legendtrade-market-data-api-openapi.yml
- filename: legendtrade-wallets-api-openapi.yml
  format: yaml
  label: LegendTrade Wallets API
  slug: legendtrade-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/legendtrade/refs/heads/main/openapi/legendtrade-wallets-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: legend.trade
  spf: false
hosts:
- cert_expires: Aug 24 17:53:52 2026 GMT
  host: www.legend.trade
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 17:53:52 2026 GMT
  host: docs.legend.trade
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: api.legend.trade
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Legendtrade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LegendTrade, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: LegendTrade
provider_slug: legendtrade
slug: legendtrade-domain-security
source_filename: legendtrade-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.legend.trade\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 17:53:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.legend.trade\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 17:53:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.legend.trade\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: legend.trade\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/legendtrade/refs/heads/main/security/legendtrade-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Defi
- Trading
- Cryptocurrency
- Perpetual Futures
- Social Trading
- Copy Trading
- Market Data
- Hyperliquid
- WebSocket
---

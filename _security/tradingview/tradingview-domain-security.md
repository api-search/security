---
api_specs:
- filename: tradingview-account-api-openapi.yml
  format: yaml
  label: TradingView Account API
  slug: tradingview-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-account-api-openapi.yml
- filename: tradingview-authorization-api-openapi.yml
  format: yaml
  label: TradingView Authorization API
  slug: tradingview-authorization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-authorization-api-openapi.yml
- filename: tradingview-broker-configuration-api-openapi.yml
  format: yaml
  label: TradingView Broker Configuration API
  slug: tradingview-broker-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-broker-configuration-api-openapi.yml
- filename: tradingview-data-integration-api-openapi.yml
  format: yaml
  label: TradingView Data Integration API
  slug: tradingview-data-integration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-data-integration-api-openapi.yml
- filename: tradingview-data-permissions-api-openapi.yml
  format: yaml
  label: TradingView Data Permissions API
  slug: tradingview-data-permissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-data-permissions-api-openapi.yml
- filename: tradingview-market-data-api-openapi.yml
  format: yaml
  label: TradingView Market Data API
  slug: tradingview-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-market-data-api-openapi.yml
- filename: tradingview-trading-api-openapi.yml
  format: yaml
  label: TradingView Trading API
  slug: tradingview-trading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-trading-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tradingview.com
  spf: true
hosts:
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: www.tradingview.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TradingView Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TradingView, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TradingView
provider_slug: tradingview
slug: tradingview-domain-security
source_filename: tradingview-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tradingview.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tradingview.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/tradingview/security/tradingview-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Charts
- Charting Library
- Financial Data
- Market Data
- Widgets
- Trading
- Fintech
- Embeddable Components
---

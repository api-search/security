---
api_specs:
- filename: stockgro-tradeview-intraday-model-openapi.json
  format: json
  label: TradeView Intraday Model API
  slug: stockgro-tradeview-intraday-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stockgro/refs/heads/main/openapi/stockgro-tradeview-intraday-model-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stockgro.club
  spf: true
hosts:
- cert_expires: Oct  5 14:07:43 2026 GMT
  host: www.stockgro.club
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 14:07:43 2026 GMT
  host: api.stockgro.club
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stockgro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StockGro, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: StockGro
provider_slug: stockgro
slug: stockgro-domain-security
source_filename: stockgro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stockgro.club\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 14:07:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.stockgro.club\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 14:07:43 2026 GMT\n  hsts: null\ndomains:\n- domain: stockgro.club\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stockgro/refs/heads/main/security/stockgro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Stock Market
- Investing
- Market Data
- Financial Education
- Fintech
- India
- Advisory
- Social Investing
---

---
api_specs:
- filename: stockdata-openapi.yml
  format: yaml
  label: StockData API
  slug: stockdata
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stockdata/refs/heads/main/openapi/stockdata-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: stockdata.org
  spf: true
hosts:
- cert_expires: Aug 22 20:42:26 2026 GMT
  host: www.stockdata.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 20:42:26 2026 GMT
  host: api.stockdata.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stockdata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StockData, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: StockData
provider_slug: stockdata
slug: stockdata-domain-security
source_filename: stockdata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stockdata.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 20:42:26 2026 GMT\n  hsts: false\n- host: api.stockdata.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 20:42:26 2026 GMT\n  hsts: null\ndomains:\n- domain: stockdata.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stockdata/refs/heads/main/security/stockdata-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Finance
- Financial Data
- Stock Market
- Market Data
- News
- Sentiment Analysis
---

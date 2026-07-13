---
api_specs:
- filename: alpha-vantage-openapi.yml
  format: yaml
  label: Alpha Vantage Market Data API
  slug: market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpha-vantage/refs/heads/main/openapi/alpha-vantage-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: alphavantage.co
  spf: true
hosts:
- cert_expires: Sep 15 01:12:12 2026 GMT
  host: www.alphavantage.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alpha Vantage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alpha Vantage, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Alpha Vantage
provider_slug: alpha-vantage
slug: alpha-vantage-domain-security
source_filename: alpha-vantage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alphavantage.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 01:12:12 2026 GMT\n  hsts: false\ndomains:\n- domain: alphavantage.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alpha-vantage/refs/heads/main/security/alpha-vantage-domain-security.yml
summary_line: TLSv1.3
tags:
- Fintech
- Market Data
- Stocks
- FX
- Crypto
- Commodities
- Economic Indicators
- Technical Indicators
- Fundamentals
- News
- Sentiment
- Free
---

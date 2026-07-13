---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: EOD Historical Data Financial API
  slug: financial-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/EodHistoricalData/EODHD-openapi/main/openapi.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: eodhd.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: eodhistoricaldata.com
  spf: true
hosts:
- cert_expires: Sep 24 11:27:55 2026 GMT
  host: eodhd.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  8 05:01:29 2026 GMT
  host: eodhistoricaldata.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Eod Historical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EOD Historical Data, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: EOD Historical Data
provider_slug: eod-historical
slug: eod-historical-domain-security
source_filename: eod-historical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eodhd.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 24 11:27:55 2026 GMT\n  hsts: false\n- host: eodhistoricaldata.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  8 05:01:29 2026 GMT\n  hsts: false\ndomains:\n- domain: eodhd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: eodhistoricaldata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eod-historical/refs/heads/main/security/eod-historical-domain-security.yml
summary_line: TLSv1.2
tags:
- Fintech
- Market Data
- Stocks
- ETF
- Fundamentals
- Options
- Forex
- Crypto
- Macroeconomic
- Technical Indicators
- News
- Sentiment
- Historical Data
---

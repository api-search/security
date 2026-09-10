---
api_specs:
- filename: openapi.json
  format: json
  label: 한국주식데이터 공개 데이터 API
  slug: 한국주식데이터-공개-데이터-api
  spec_type: OpenAPI
  url: https://aikstockdata.com/openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aikstockdata.com
  spf: false
hosts:
- cert_expires: Dec  4 08:46:54 2026 GMT
  host: aikstockdata.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aikstockdata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 한국주식데이터 (aikstockdata), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: 한국주식데이터 (aikstockdata)
provider_slug: aikstockdata
slug: aikstockdata-domain-security
source_filename: aikstockdata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aikstockdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 08:46:54 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: aikstockdata.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aikstockdata/refs/heads/main/security/aikstockdata-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- korea
- stock-market
- financial-data
- open-data
- dart
- kospi
- kosdaq
- konex
- filings
- equities
- mcp
- llms-txt
- openapi
---

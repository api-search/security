---
api_specs:
- filename: alltick-api-openapi.json
  format: json
  label: AllTick REST/HTTP Query API
  slug: alltick-resthttp-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alltick-api/refs/heads/main/openapi/alltick-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: alltick.co
  spf: true
hosts:
- cert_expires: Oct  5 03:46:06 2026 GMT
  host: en.apis.alltick.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 04:48:03 2026 GMT
  host: quote.alltick.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alltick Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AllTick API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AllTick API
provider_slug: alltick-api
slug: alltick-api-domain-security
source_filename: alltick-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.apis.alltick.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 03:46:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: quote.alltick.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 04:48:03 2026 GMT\n  hsts: null\ndomains:\n- domain: alltick.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alltick-api/refs/heads/main/security/alltick-api-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- financial-market-data
- real-time-data
- stock-market-data
- forex-data
- cryptocurrency-data
- commodities-data
- tick-data
- websocket-streaming
- fintech
- quantitative-trading
- market-data-api
- trading-halts
---

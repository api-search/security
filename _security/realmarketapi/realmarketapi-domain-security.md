---
api_specs:
- filename: realmarketapi-market-data-api-openapi.yml
  format: yaml
  label: RealMarketAPI Market Data API
  slug: realmarketapi-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/realmarketapi/openapi/realmarketapi-market-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: realmarketapi.com
  spf: true
hosts:
- cert_expires: Dec 30 02:21:45 2026 GMT
  host: realmarketapi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Realmarketapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RealMarketAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RealMarketAPI
provider_slug: realmarketapi
slug: realmarketapi-domain-security
source_filename: realmarketapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: realmarketapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 02:21:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: realmarketapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/realmarketapi/security/realmarketapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Market Data
- Real-Time
---

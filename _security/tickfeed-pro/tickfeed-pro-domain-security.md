---
api_specs:
- filename: tickfeed-pro-account-api-openapi.yml
  format: yaml
  label: tickfeed-pro Account API
  slug: tickfeed-pro-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickfeed-pro/openapi/tickfeed-pro-account-api-openapi.yml
- filename: tickfeed-pro-market-data-api-openapi.yml
  format: yaml
  label: tickfeed-pro market data API
  slug: tickfeed-pro-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickfeed-pro/openapi/tickfeed-pro-market-data-api-openapi.yml
- filename: tickfeed-pro-system-api-openapi.yml
  format: yaml
  label: tickfeed-pro System API
  slug: tickfeed-pro-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickfeed-pro/openapi/tickfeed-pro-system-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tickfeed.pro
  spf: true
hosts:
- cert_expires: Jan 12 13:21:19 2027 GMT
  host: tickfeed.pro
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tickfeed Pro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tickfeed-pro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: tickfeed-pro
provider_slug: tickfeed-pro
slug: tickfeed-pro-domain-security
source_filename: tickfeed-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tickfeed.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 13:21:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tickfeed.pro\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/tickfeed-pro/security/tickfeed-pro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Finance
- MarketData
- API
- Forex
- Gold
- MCP
---

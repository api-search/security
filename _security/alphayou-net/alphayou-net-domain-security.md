---
api_specs:
- filename: alphayou-net-alphayou-api-openapi.yml
  format: yaml
  label: alphayou-net Alpha You API
  slug: alphayou-net-alphayou-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphayou-net/openapi/alphayou-net-alphayou-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alphayou.net
  spf: true
hosts:
- cert_expires: Dec 20 02:25:13 2026 GMT
  host: alphayou.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Alphayou Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for alphayou-net, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: alphayou-net
provider_slug: alphayou-net
slug: alphayou-net-domain-security
source_filename: alphayou-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alphayou.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 02:25:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: alphayou.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/alphayou-net/security/alphayou-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- StockResearch
- TradingTools
- MarketAnalytics
- Alerts
---

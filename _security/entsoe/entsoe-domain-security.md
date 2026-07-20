---
api_specs:
- filename: 2s93JtP3F6
  format: yaml
  label: ENTSO-E Transparency Platform REST API
  slug: entso-e-transparency-platform-rest-api
  spec_type: Postman
  url: https://documenter.getpostman.com/view/7009892/2s93JtP3F6
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: entsoe.eu
  spf: true
hosts:
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: www.entsoe.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: transparency.entsoe.eu
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: web-api.tp.entsoe.eu
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Entsoe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ENTSO-E, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: ENTSO-E
provider_slug: entsoe
slug: entsoe-domain-security
source_filename: entsoe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.entsoe.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: transparency.entsoe.eu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: web-api.tp.entsoe.eu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: entsoe.eu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/entsoe/refs/heads/main/security/entsoe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- Electricity
- European Union
- Transparency
- Market Data
- Generation
- Transmission
- Load Forecasting
- Day-Ahead Prices
- Cross-Border Flows
---

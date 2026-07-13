---
api_specs:
- filename: cftc-cot-openapi.yml
  format: yaml
  label: CFTC Commitments of Traders SODA API
  slug: cftc-cot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commodity-futures-trading-commission/refs/heads/main/openapi/cftc-cot-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cftc.gov
  spf: true
hosts:
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: www.cftc.gov
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 19 02:51:28 2027 GMT
  host: publicreporting.cftc.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Commodity Futures Trading Commission Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Commodity Futures Trading Commission, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Commodity Futures Trading Commission
provider_slug: commodity-futures-trading-commission
slug: commodity-futures-trading-commission-domain-security
source_filename: commodity-futures-trading-commission-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cftc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: publicreporting.cftc.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 19 02:51:28 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cftc.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commodity-futures-trading-commission/refs/heads/main/security/commodity-futures-trading-commission-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CFTC
- Commitments of Traders
- Federal Government
- Financial
- Futures
- Open Data
- SODA
- Trading
---

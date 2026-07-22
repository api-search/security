---
api_specs:
- filename: xeneta-api-30-openapi.yml
  format: yaml
  label: Xeneta API
  slug: xeneta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xeneta/refs/heads/main/openapi/xeneta-api-30-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: xeneta.com
  spf: true
hosts:
- cert_expires: Sep 21 10:01:28 2026 GMT
  host: www.xeneta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 00:50:07 2026 GMT
  host: help.xeneta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: api.xeneta.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xeneta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xeneta, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Xeneta
provider_slug: xeneta
slug: xeneta-domain-security
source_filename: xeneta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.xeneta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 10:01:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.xeneta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 00:50:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.xeneta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: xeneta.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xeneta/refs/heads/main/security/xeneta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Freight
- Shipping
- Logistics
- Ocean Freight
- Air Freight
- Benchmarking
- Market Data
- Supply Chain
- Rates
- Emissions
---

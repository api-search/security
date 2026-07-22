---
api_specs:
- filename: rift-openapi.yml
  format: yaml
  label: Rift Router API
  slug: rift-router
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rift/refs/heads/main/openapi/rift-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: rift.trade
  spf: false
hosts:
- cert_expires: Oct  8 20:59:13 2026 GMT
  host: rift.trade
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rift, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Rift
provider_slug: rift
slug: rift-domain-security
source_filename: rift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rift.trade\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 20:59:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: rift.trade\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rift/refs/heads/main/security/rift-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Crypto Defi
- DEX Aggregator
- Cross-Chain
- Trading
- Swaps
- Bridge
- Best Execution
---

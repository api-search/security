---
api_specs:
- filename: pyth-hermes-openapi-original.json
  format: json
  label: Pyth Hermes (Pyth Core)
  slug: pyth-hermes-pyth-core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pyth/refs/heads/main/openapi/pyth-hermes-openapi-original.json
- filename: pyth-benchmarks-openapi-original.json
  format: json
  label: Pyth Benchmarks
  slug: pyth-benchmarks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pyth/refs/heads/main/openapi/pyth-benchmarks-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pyth.network
  spf: true
hosts:
- cert_expires: Oct  8 15:00:18 2026 GMT
  host: pyth.network
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pyth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pyth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Pyth
provider_slug: pyth
slug: pyth-domain-security
source_filename: pyth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pyth.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 15:00:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pyth.network\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pyth/refs/heads/main/security/pyth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto Web3
- Oracle
- Price Feeds
- Market Data
- DeFi
- Blockchain
- Financial Data
---

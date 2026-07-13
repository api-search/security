---
api_specs:
- filename: sei-cosmos-rest-api.yml
  format: yaml
  label: Sei Cosmos REST API (LCD)
  slug: sei-cosmos-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sei/refs/heads/main/openapi/sei-cosmos-rest-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sei.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: sei-apis.com
  spf: false
hosts:
- cert_expires: Sep 21 01:36:58 2026 GMT
  host: sei.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 12:10:05 2026 GMT
  host: docs.sei.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 17:30:59 2026 GMT
  host: evm-rpc.sei-apis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sei Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sei, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sei
provider_slug: sei
slug: sei-domain-security
source_filename: sei-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sei.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 01:36:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.sei.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 12:10:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: evm-rpc.sei-apis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 17:30:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sei.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: sei-apis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sei/refs/heads/main/security/sei-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain
- Layer 1
- EVM
- DeFi
- DEX
- Trading
- Cosmos
- Web3
---

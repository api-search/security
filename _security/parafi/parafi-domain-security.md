---
api_specs:
- filename: parafi-openapi.json
  format: json
  label: ParaFi Tech API
  slug: parafi-tech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parafi/refs/heads/main/openapi/parafi-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: parafi.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: parafi.tech
  spf: true
hosts:
- cert_expires: Aug 18 00:22:35 2026 GMT
  host: parafi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 22:21:32 2026 GMT
  host: parafi.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parafi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parafi, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Parafi
provider_slug: parafi
slug: parafi-domain-security
source_filename: parafi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parafi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 00:22:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: parafi.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 22:21:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: parafi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: parafi.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parafi/refs/heads/main/security/parafi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Blockchain
- Digital Assets
- Staking
- Validators
- Solana
- Ethereum
- Avalanche
- DeFi
- Market Data
---

---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: OKX Trading API
  slug: okx-trading-api
  spec_type: OpenAPI
  url: https://www.okx.com/docs-v5/en/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: okx.com
  spf: true
hosts:
- cert_expires: Sep 11 11:56:49 2026 GMT
  host: www.okx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: openapi.okx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 14:37:04 2026 GMT
  host: web3.okx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Okx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OKX, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: OKX
provider_slug: okx
slug: okx-domain-security
source_filename: okx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.okx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 11:56:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: openapi.okx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: null\n- host: web3.okx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:37:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: okx.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/okx/refs/heads/main/security/okx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cryptocurrency
- Exchange
- Trading
- Derivatives
- Spot Trading
- Futures
- Options
- Market Data
- Web3
- Blockchain
- Wallet
---
